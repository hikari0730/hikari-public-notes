
# Introduction to Vue.js

Vue.js is a progressive JavaScript framework used to build user interfaces. It is designed to be incrementally adoptable and focuses on the view layer.

---

## What makes Vue unique?

- **Reactive Data Binding**
- **Component-based architecture**
- **Lightweight and flexible**
- Can be used for **single-page applications (SPA)**

---

## Hello Vue Example

```html
<div id="app">
  {{ message }}
</div>

<script>
const app = Vue.createApp({
  data() {
    return {
      message: 'Hello, Vue!'
    }
  }
})
app.mount('#app')
</script>
```



## Quiz 01 – Introduction to Vue.js

This is a short quiz to review the basics of Vue.js.

---

### Q1. What is Vue.js mainly used for?

- [ ] Backend development
- [x] Building user interfaces
- [ ] Database management

---

### Q2. Which of the following is a feature of Vue.js?

- [x] Reactive data binding
- [ ] Built-in SQL database
- [ ] Requires server-side rendering

---

### Q3. In the Vue example below, what will be shown in the browser?
```html
<div id="app">
  {{ message }}
</div>

<script>
const app = Vue.createApp({
  data() {
    return {
      message: 'Hello, Vue!'
    }
  }
})
app.mount('#app')
</script>
```
- [ ] Nothing, because Vue needs jQuery
- [ ] The text "{{ message }}"
- [x] Hello, Vue!
---

### Q4. What is the correct way to create a Vue app?
- [x] Vue.createApp({ ... }).mount('#app')
- [ ] new VueEngine()
- [ ] ReactDOM.render(...)

---
### Q5. What is the goal of Vue’s component system?
- [ ] Avoid using HTML and CSS
- [x] Build reusable UI elements
- [ ] Connect to MySQL databases
