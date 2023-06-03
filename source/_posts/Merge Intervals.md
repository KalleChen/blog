---
title: 演算法系列#4 Merge Intervals
date: 2023-06-03
updated: 2023-06-03
tags: [algorithm]
categories:
  - 演算法
thumbnail: /演算法系列#4 Merge Intervals/merge_interval.png
keywords: merge interval, algorithm, 演算法, 教學, leetcode
---

![](/blog/assets/merge_interval.png)

<!-- more -->

Merge Interval 通常用於處理重疊的區間，在很多關於區間的題目中，我們很常需要去處理兩個區間的合併與重疊

以下為處理區間時總共會遇到的 6 種情況


了解並分別解決這六種情況基本上就能處理題目所需要的問題了

## 如何分辨

- 當題目要求你輸出一個互斥區間的列表
- 當題目有出現“重疊的區間”

## 題目

- Intervals Intersection (medium)
- Maximum CPU Load (hard)
