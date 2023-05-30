---
title: 演算法系列#1 Sliding Window 滑動視窗
date: 2023-05-31
updated: 2023-05-31
tags: [algorithm]
categories:
  - 演算法
---

![](/blog/assets/sliding-window.png)

<!-- more -->

前陣子在準備面試，又花了不少時間刷 leetcode 跟演算法，但這次比起之前照數字慢慢往下刷，我試了用別人以各種演算法整理而出的題目來刷。
因此整理了一些比較常見的演算法概念跟怎麼來辨別這些題目應該用哪些演算法，有沒有什麼線索可以依據之類的，也為了未來哪天又要開始刷題的我
希望透過這個系列可以幫助各位在準備的過程中有比較清晰的方向

sliding window 是從第一個陣列開始，開始一個一個元素往右移
並根據題目的問題來調整你的 window size
而在有些情況下，這個 window size 是不會變的

## 如何分辨是否該使用 sliding window
- 這個問題的輸入是一串 linear 的資料結構，例如 linked list， array，string
- 題目要求尋找 longest/shortest substring，subarray，或是一個特定的數值

## 題目
- Maximum sum subarray of size ‘K’ (easy) 
- Longest substring with ‘K’ distinct characters (medium) 
- String anagrams (hard)
