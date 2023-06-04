---
title: 淺談瀏覽器事件機制 Event Bubbling, Event Capturing, Event Delegation
date: 2023-06-04
updated: 2023-06-04
tags: [前端, 瀏覽器]
categories:
  - 技術科普
thumbnail: /淺談瀏覽器事件機制Event Bubbling, Event Capturing, Event Delegation/js_event.png
keywords: js, browser, event
---

![](/blog/assets/js_event.png)

<!-- more -->

# Event Bubbling

指的是當一個元素觸發了某個事件，例如 click，那麼這個事件被此元件的 event handler 處理後會接著傳給此元素上層的父元素中的 Event handler，並接著再傳給上層元素，直到最上層

```html
<form onclick="alert('form')">
  <div onclick="alert('div')">
    <p onclick="alert('p')">
    </p>
  </div>
</form>
```

例如上面這裡，加入 p 元素被點擊時，會依序執行 p -> div -> form 各自的 onclick function

而如果想要阻止 event bubbling 的話，可以使用 `event.stopPropagation()` 這個方法

### event handler

這邊要特別介紹一下什麼是 `event handler`
這是一個非同步的執行或回調函式，用來處理 DOM element 上的各個事件

而其中 `event.target` 本身指的是觸發的物件本身，如果需要取得綁定此 event handler 的元素則可以使用 `event.currentTarget` 或是 `this` 

像是上面點擊 `p` 的 `form` 的 event handler 裡面的 `target` 就會是 `p` 而 `currentTarget` 就會是 `form`

# Event Capturing

與 Event Bubbling 相反，當事件發生在某個 DOM element 上時，會從最上層的 parent 開始執行各自的 Event handler，直到抵達觸發的 element 時

一樣舉上面的例子，點擊 `p` 後順序就會變成 form -> div -> p

而如果想要設定為 event capturing，可以在 `addEventListener` 的第三個參數設定為 true（預設為 false）

```javascript
form.addEventListener('click', handler, true)
```

# Event Delegation

當如果有很多 element 都有一樣的 Event handler 時，可以利用 Event Bubbling 的特性，再它們的共同父級元素新增 event handler，這樣就不需要每個元素都各自設定自己的 event handler 了


```html
<ol id="list">
  <li data-num="1"><em>1</em></li>
  <li data-num="2"><em>2</em></li>
  <li data-num="3"><em>3</em></li>
  <li data-num="4"><em>4</em></li>
</ol>
```

例如以上，我們就可以只在 `ol` 上設定 evnet handler 就好

```javascript
list.addEventListener('click', e => {
  const li = e.target.closest('li')
  if (!li || !list.contains(li)) return

  alert(li.dataset.num)
})
```

需要注意的是，我們需要檢查觸發這個時間的 target 是不是在這個 list 裡面

同理，我們也可以利用元素的 attribute 來設定各種需要相同 handler 的元素，並且直接在 document 上新增 event listener 就好，例如 counter 之類的東西

# References

- https://shubo.io/event-bubbling-event-capturing-event-delegation/
