---
title: 演算法系列#5 Cyclic Sort
date: 2023-06-04
updated: 2023-06-04
tags: [algorithm]
categories:
  - 演算法
thumbnail: /Cyclic%20sort/cyclic_sort.png
keywords: cyclic sort, algorithm, 演算法, 教學, leetcode
---

![](/blog/assets/cyclic_sort.png)

<!-- more -->

這個方法主要處理 array 有關的問題，會一個一個數字瀏覽過去，並檢查每個數字的 index 是不是題目所需要的，如果這個數字不在他應該的 index 上，就利用 swap 的方式移動到正確的 index

## 如何分辨

- 問題裡面可能包括一個 sorted array
- 如果題目需要從一個 sorted array 裡面尋找一個 missing/重複/最小 的數字

## 題目

- Find the Missing Number (easy)
- Find the Smallest Missing Positive Number (medium)
