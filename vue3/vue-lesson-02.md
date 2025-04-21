---
title: Lesson 2 - Reactive Data in Vue 3
language: en
level: beginner
tags: [vue3, ref, reactive, data binding]
status: done
---


# Lesson 2: Reactive Data in Vue 3

## 1. What is Reactivity?

Vue’s reactivity system allows the view (DOM) to automatically update when the data changes. This is the core of Vue.


---

## 2. ref() and reactive() in Vue 3

ref()

- Used to create reactive primitive values (numbers, strings, booleans, etc.).

- Access or modify the value via .value.

```js
import { ref } from 'vue';

const count = ref(0);
count.value++;

reactive()
```

- Used to create reactive objects or arrays.

- You can access properties directly, no need for .value.

```js
import { reactive } from 'vue';

const user = reactive({
  name: 'Alice',
  age: 25
});

user.age++;
```

---

## 3. Using Reactive Data in Templates

```html
<div id="app">
  <p>Counter: {{ count }}</p>
  <button @click="increment">+1</button>
</div>
```

```js
import { createApp, ref } from 'vue';

createApp({
  setup() {
    const count = ref(0);
    const increment = () => count.value++;

    return { count, increment };
  }
}).mount('#app');
```

---

## 4. Important Notes

- ref() values need .value in JavaScript, but **not in templates**.

- reactive() is good for objects, but cannot be destructured directly (it breaks reactivity).

- You can use toRefs() or computed() to preserve reactivity when destructuring.

---

## Lesson Quiz

1. **What is the main purpose of ref() in Vue 3?**

   - A. To store functions

    - B. To create reactive primitive values

    - C. To define components

    - D. To access DOM nodes

      ✅ Answer: B



2. **Which of the following statements is TRUE about reactive()?**

A. It only works with primitive values

B. It requires .value to access properties

C. It makes objects reactive

D. It does not update the view
✅ Answer: C








