
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
