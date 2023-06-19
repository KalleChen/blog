---
title: 演算法系列#12 Top K elements
date: 2023-06-11
updated: 2023-06-11
tags: [algorithm]
categories:
  - 演算法
thumbnail: /Binary%20Search/top_k.png
keywords: binary search, tree, algorithm, 演算法, 教學, leetcode
---

![](/blog/assets/top_k.png)

<!-- more -->

這個 pattern 多用於題目需要你找第 k 高/低的元素時

方法是用一個 heap 來存 k 個 element，並在搜尋的途中不斷的變更這個 heap，最後答案便是這個 heap 的 top

以下是這個方法的步驟

1. 將 k 個 element 插入到一個 min-heap 或是 max-heap
2. 接著開始一個一個瀏覽剩下的 element，當這個 element 小於/大於 heap 的 top 時，就將新的 element 跟現在的 top 對換，並且調整 heap

要注意的是調整 heap 所需要的時間複雜度是 O(logn)

## 如何判斷

- 當題目需要你找第 k 高/低 的元素時

## 題目

- Top ‘K’ Numbers (easy)
- Top ‘K’ Frequent Numbers (medium)
