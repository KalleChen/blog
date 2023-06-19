---
title: 演算法系列#14 Topological sort
date: 2023-06-13
updated: 2023-06-13
tags: [algorithm]
categories:
  - 演算法
thumbnail: /Topological%20sort/topological.png
keywords: binary search, tree, algorithm, 演算法, 教學, leetcode
---

![](/blog/assets/topological.png)

<!-- more -->

這個 pattern 是當題目要求你 sort 有 dependencies 關係時的 element 時的方法，dependencies 的意思比如 A 需要在 B 之後才能出現，因此排序時我們就不能將 A 排在 B 之前

以下為 topological sort 的步驟

1. 瀏覽所有的 vertices 並計算每個元素的 in-degrees 數值，初始為 0，用 HashMap 儲存，每個 vertices 的子元素的 HashMap 都要 +1，這樣就完成了初始化
2. 接著將這個 HashMap 中 in-degrees 為 0 的元素提出來（也就是沒有排序在其他元素後方的元素），並將他們加入到一個 sources queue
3. 將 sources queue 中的元素加到要輸出的 sorted list 裡，並將所有此元素的子元素的 in-degree 數值 -1，如果 in-degree 變 0 了，就將他們加到 source queue 中
4. 重複 3 的動作

## 如何分辨

- 題目需要處理 graph 並且沒有 cycle 的問題
- 題目有特定的 sorted order 條件

## 題目

- Task scheduling (medium)
- Minimum height of a tree (hard)
