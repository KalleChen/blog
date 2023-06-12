---
title: 演算法系列#11 Binary Search
date: 2023-06-10
updated: 2023-06-10
tags: [algorithm]
categories:
  - 演算法
thumbnail: /Binary%20Search/binary_search.png
keywords: binary search, tree, algorithm, 演算法, 教學, leetcode
---

![](/blog/assets/binary_search.png)

<!-- more -->

當題目給你一個 sorted 的 array，linked-list 或是 matrix，並要求你從中找到特定的元素，那麼 binary search 是一個很好用的方法


1. 第一我們會先設定 start 跟 end 兩個點，並從這兩點中間找到 middle = (start + end) / 2
2. 檢查這個 middle 是否符合題目所需，如果是的話就直接回傳 middle
3. 檢查如果題目所需的數字小於 middle，那麼就將 end 設定成 middle - 1，並從第一步開始
4. 如果題目所需的數字大於 middle，將 start 設成 middle + 1，並從第一步開始

以下為一個簡單的範例

```javascript
let start = 0, end = elements.length - 1
while(start < end) {
	const middle = Math.floor((start + end) / 2)
	if (elements[middle] === target) return middle
	else if (elements[middle] > target) end = middle - 1
	else start = middle + 1
}
return start
```

## 題目

- Order-agnostic Binary Search (easy)
- Search in a Sorted Infinite Array (medium)
