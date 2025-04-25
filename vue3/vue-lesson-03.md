---

lesson-03-events.md

---
title: "Lesson 3: Handling Events in Vue 3"
lang: en-zh
level: beginner
tags: [vue3, events, click, methods]
lesson: 3
status: in-progress
emoji: "⚡"
---

# Lesson 3: Handling Events in Vue 3  
**第三課：Vue 3 中的事件處理**

---

## 1. 使用 @click 綁定事件  
**Binding Events with `@click`**

Vue 提供簡潔的方式將 DOM 事件（如點擊）綁定到元件的方法上。

> Vue provides a concise way to bind DOM events (like clicks) to component methods.

```js
<template>
  <button @click="sayHello">Click Me</button>
</template>

<script setup>
function sayHello() {
  alert("Hello from Vue!")
}
</script>
```

---

### 2. 方法定義與使用

**Defining and Using Methods**

可以在 <script setup> 或 Options API 中定義方法，並於模板中透過事件呼叫。

> Define methods in <script setup> or Options API and call them in the template using event bindings.

---

### 3. 傳遞參數到事件方法

**Passing Parameters to Event Handlers**

你可以傳遞參數給方法，只需用小括號包住。

> You can pass parameters to the method using parentheses.

```js
<template>
  <button @click="greet('Hikari')">Greet</button>
</template>

<script setup>
function greet(name) {
  alert(`Hello, ${name}!`)
}
</script>
```

---

## 4. 使用 $event 獲取原始事件物件

**Using $event to Access Native Event Object**

可以透過 $event 或 (e) 抓取原生事件物件。

```js
<template>
  <button @click="handleClick($event)">Click Me</button>
</template>

<script setup>
function handleClick(e) {
  console.log('Event type:', e.type)
}
</script>
```

---

## Quiz: Lesson 3 — Handling Events

**測驗：第三課 — 事件綁定**

### Q1. 下列哪一個寫法可以正確綁定點擊事件？

A. @click="sayHello" 
B. v-on:click="sayHello" 
C. onClick="sayHello()" 
D. click="sayHello" 

Answer: ✅ A, ✅ B


---

### Q2. 若要在事件中傳遞一個參數 "Vue"，下列哪個寫法是正確的？

A. @click="sayHi('Vue')" 
B. @click="sayHi = 'Vue'" 
C. @click="sayHi: 'Vue'"
D. @click="sayHi{'Vue'}"

Answer: ✅ A


---

Q3. $event 在 Vue 中的用途是什麼？

A. 傳遞布林值給子元件
B. 存取原生 DOM 事件物件
C. 宣告一個反應式變數
D. 選擇 CSS 元素

Answer: ✅ B


---

Tips

使用 @click="method" 是最常見的事件綁定方式。

若要操作 DOM 或獲取點擊位置，可以使用 $event。

不要直接操作 DOM，應儘量透過資料驅動方式操作。


---

這就是 Lesson 3 的完整內容！  
若你需要中英對照雙欄表格、學習地圖更新、或是製作 PDF 版本筆記，我也可以幫你完成。

準備好進入 Lesson 4 嗎？

