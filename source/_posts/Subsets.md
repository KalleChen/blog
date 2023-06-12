---
title: 演算法系列#10 Subsets
date: 2023-06-09
updated: 2023-06-09
tags: [algorithm]
categories:
  - 演算法
thumbnail: /Subsets/subsets.png
keywords: subsets, tree, algorithm, 演算法, 教學, leetcode
---

![](/blog/assets/subsets.png)

<!-- more -->

很多題目會要求我們對一堆 elements 來做排列或是組合，subsets 這個 pattern 就是使用類似 BFS 的方法來解決這類型的問題

這個 pattern 總共有以下這些步驟

如果題目給定一個 set [1, 5, 3]

1. 從一個空的 set 開始 [[]]
2. 將第一個 element 加到所有的 subsets 裡面並新增一個新的 [ [], [1] ]
3. 將第二個 element 5 重複上面的動作 [ [], [1], [5], [1, 5] ]
4. 不斷重複上面的動作


## 如何判斷

- 當題目要求你從一堆 element 裡面找出組合或是排列

## 題目

- Subsets With Duplicates (easy)
- String Permutations by changing case (medium)
