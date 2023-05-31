---
title: 演算法系列#2 Two Pointer or Iterators
date: 2023-06-01
updated: 2023-06-01
tags: [algorithm]
categories:
  - 演算法
keywords: two pointer, algorithm, 演算法, 教學, leetcode
thumbnail: /演算法系列#2 Two Pointer or Iterators/two-pointer.png
---

![](/blog/assets/two-pointer.png)

<!-- more -->

two pointer 的使用通常是透過兩個指標並根據一定的情況下來移動各個指標，直到達到題目所要的目標
以上圖為例，我們要從一個 sorted array 裡面找到兩個數字相加綜合為 6 的組合，最好的辦法就是設定兩個 pointer 一個從頭一個從尾，當這兩個 pointer 相加的數字超過目標數時，就代表我們的右指標要往左移，也就是減少兩個數字的綜合，相反的則是移動左指標
最常用的方法是設定一個 `left` 一個 `right`的 pointer，並利用 `while` 迴圈直到符合目標或是兩個 pointer 以無法再移動下去

## 如何分辨

- 這個方法通常用於處理一個 sorted array 或是 linked list，例如你需要每個 element 跟其他的 element 做比較時

## 題目

- Squaring a sorted array (easy)
- Triplets that sum to zero (medium) 
- Comparing strings that contain backspaces (medium)
