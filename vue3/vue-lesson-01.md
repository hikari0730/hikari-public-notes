---
title: "Vue 3 Lesson 1: Introduction and Installation"
author: "HIKARI"
date: 2025-04-21
tags: [Vue 3, JavaScript, Frontend]
description: "Learn the basics of Vue 3 including what it is, how to install it, and basic syntax."
---

# Vue 3 Lesson 1: Introduction and Installation

## What is Vue?

Vue is an **advanced JavaScript framework** focused on building user interfaces.

- It uses a **virtual DOM** for optimized performance.
- It follows a **progressive enhancement** model.
- Highly flexible and easy to integrate with existing projects.

---

## Installation and Getting Started

### Option 1: Using CDN

```html
<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
```

### Option 2: Using Vue CLI

```bash
npm install -g @vue/cli
vue create my-vue-app
cd my-vue-app
npm run serve
```

### Start a Simple Vue App

**HTML Template**

```html
<div id="app">
  {{ message }}
</div>
```

**JavaScript**
```js
<script>
  const { createApp } = Vue;

  createApp({
    data() {
      return {
        message: "Hello, Vue 3!"
      };
    }
  }).mount("#app");
</script>
```

---

## Key Syntax Overview

### Template Binding

```html
<p>{{ message }}</p>
```

### Data Display and Binding

Data defined in the data() function will automatically update the DOM when changed.


---

## Quick Quiz

### Q1: What is Vue mainly used for?

A. Server-side logic  
B. Building user interfaces  
C. Backend API development  
D. Database management  

**Answer:** B. Building user interfaces

---

### Q2: What is the purpose of createApp() in Vue 3?

A. To install Vue plugins  
B. To mount the Vue devtools  
C. To initialize and mount a Vue application  
D. To define computed properties  

**Answer:** C. To initialize and mount a Vue application


---

### Q3: What does {{ message }} do in a Vue template?

A. Runs a JavaScript alert  
B. Inserts static HTML  
C. Binds data to the DOM  
D. Defines a CSS class  

**Answer:** C. Binds data to the DOM


---


