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

`ref()`

- Used to create reactive primitive values (numbers, strings, booleans, etc.).

- Access or modify the value via .value.

```js
import { ref } from 'vue';

const count = ref(0);
count.value++;
```

`reactive()`

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

## 5. Lesson Quiz (with Answers)

### Q1: What is the purpose of `ref()` in Vue 3?

- A. To define components  
- B. To make primitive values reactive  
- C. To loop through arrays  
- D. To bind HTML attributes

**Answer: B**

---

### Q2: What does `.value` do when using `ref()`?

- A. It returns a string version of the variable  
- B. It accesses the inner value of a ref-wrapped variable  
- C. It defines a new computed property  
- D. It triggers a re-render manually

**Answer: B**

---

### Q3: What kind of data is best used with `reactive()`?

- A. Boolean  
- B. String  
- C. Object or Array  
- D. Number

**Answer: C**

---

### Q4: Which of the following statements is TRUE?

- A. `ref()` and `reactive()` can be used interchangeably at all times  
- B. `reactive()` returns a Proxy and works well with objects  
- C. `ref()` is used to watch changes in templates only  
- D. `reactive()` is for read-only data

**Answer: B**

---

### Q5: In the Vue template, how do you display a `ref()` value?

```html
<!-- Choose the correct usage -->
<p>{{ counter }}</p>  
<p>{{ counter.value }}</p>  
<p>{{ ref(counter) }}</p>
```

**Answer: {{ counter }}**

> Note: Even though .value is required in JS, Vue template syntax unwraps it automatically.







