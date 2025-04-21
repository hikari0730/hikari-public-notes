⁶# Vue.js Lesson 2: Vue Instance & Data Binding

## Objective
Understand how the Vue instance works and how to bind data using the `{{ }}` syntax.

---

## Explanation

In Vue, a **Vue instance** is the foundation of every Vue application. It connects your data (model) to the DOM (view).

When you create a new Vue app using `Vue.createApp({...})`, you can define:

- `data`: the properties you want to show or use
- `methods`: functions you want to use
- `template`: or reference to HTML with Vue directives

Vue uses **reactive binding**, meaning that when your data changes, the DOM updates automatically.

---

## Code Example

### HTML

```html
<div id="app">
  <h2>{{ message }}</h2>
</div>
```

### Javascript (Vue 3)

```js
const app = Vue.createApp({
  data() {
    return {
      message: "Hello Vue!"
    }
  }
});

app.mount("#app");
```

When message changes, the text inside `<h2>` also updates instantly.

---

### Quick Quiz

**Q1.** What does {{ message }} do in Vue?

**Q2.** How do you initialize a Vue instance and mount it to the DOM?

**Q3.** True or False: When a Vue data property changes, the DOM stays the same.

**Q4.** Fill in the blank:

```js
const app = Vue.createApp({
  _____() {
    return {
      greeting: "Hi!"
    };
  }
});
```

---

Answers / Hints

**A1.** It binds the message data property to the DOM.

**A2.**
```js
const app = Vue.createApp({...});
app.mount('#id');
```

**A3.** False – Vue updates the DOM reactively.
**A4.** data


---
