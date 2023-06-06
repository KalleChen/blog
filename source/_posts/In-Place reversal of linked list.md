---
title: 演算法系列#6 In-Place Reversal of linked list
date: 2023-06-05
updated: 2023-06-05
tags: [algorithm]
categories:
  - 演算法
thumbnail: /In-Place%20reversal%20of%20linked%20list/inplace_reverse.png
keywords: in-place reverse, algorithm, 演算法, 教學, leetcode
---

![](/blog/assets/inplace_reverse.png)

<!-- more -->

在很多問題中，我們很常被問到將一個 linked list 做 reverse，並且要求我們必須符合 in-place，也就是不使用額外的記憶體空間，因此就有了這個 pattern

![[Screenshot 2023-06-06 at 3.33.07 PM.png]]

我們會設置兩個 pointer，一個 current 指向當前的 node；一個 previous 指向前一個 node

過程會是將當前 node 的 next 指向 previous，並將 current 指向當前 node 原本的 next，previous 指向當前 node

以下為範例

```javascript
// head 是這個 linked list 的頭
let current = head, previous = null 
while (current) {
	const temp = current
	current = temp.next
	temp.next = previous
	previous = temp
}
```

這樣就是一個簡單的 in-place reverse

## 如何分辨

- 當你被要求 reverse 一個 linked list 並且不能使用額外的 memory 時

## 題目

- Reverse a Sub-list (medium)
- Reverse every K-element Sub-list (medium)
