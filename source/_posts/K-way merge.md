---
title: 演算法系列#13 K-way Merge
date: 2023-06-12
updated: 2023-06-12
tags: [algorithm]
categories:
  - 演算法
thumbnail: /K-way%20merge/k-way.png
keywords: binary search, tree, algorithm, 演算法, 教學, leetcode
---

![](/blog/assets/k-way.png)

<!-- more -->

當題目要求我們將 k 個 sorted array 合併成一個時就可以用這個方法
這個方法主要是使用 heap 來儲存接下來要插入的 element

以下為這個 pattern 的步驟
1. 將所有 array 中所有第一個 element 都插入一個 min/max heap
2. 將這個 heap 的 top 抽出來並放到新的 array 裡面
3. 從被拿出的 list 裡面將第一個元素加入 heap
4. 重複 2.3 的動作

## 如何分辨

- 題目給了你 sorted arrays
- 題目要求你合併 arrays

## 題目

- Merge K Sorted Lists (medium)
- K Pairs with Largest Sums (Hard)
