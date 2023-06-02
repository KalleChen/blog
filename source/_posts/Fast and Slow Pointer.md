---
title: 演算法系列#3 Fast and Slow Pointer
date: 2023-06-02
updated: 2023-06-02
tags: [algorithm]
categories:
  - 演算法
thumbnail: /Fast%20and%20Slow%20Pointer/slow_fast.png
keywords: fast ans slow pointer, algorithm, 演算法, 教學, leetcode
---

![](/blog/assets/slow_fast.png)

<!-- more -->

這個最廣為人知的應該就是龜兔賽跑演算法了吧

如果你有看過 Joma [這集](https://www.youtube.com/watch?v=pKO9UjSeLew)的話應該印象很深 

有點類似 Two Pointer 的變形版，主要是使用兩個 Pointer 並且用不同的速度來做移動

最常是用來檢查一個 linked list 或是 array 有沒有循環圈


例如上圖這張利用了兩個 Pointer 一個前進一格，一個前進兩格，因為兩者前進的速率不同，我們就可以知道，如果這個 linked list 有循環的話，那麼這兩個 Pointer 就一定會相遇，由此來證明這個 linked list 是否有循環

## 額外補充

另外如果還想要進階的知道這個循環的起始點的話也有方法，假設兩個 Pointer 相遇的點為 X，循環起點為 S，從頭到 S 的距離為 a，從 S 到 X 的距離為 b，從 X 到尾的距離為 c

![](/blog/assets/abcxs.png)

那麼我們就可以知道 slow pointer 的行進距離為 a + b，而 fast pointer 的行進距離為 a + b + c + b = a + 2b + c
列出等式 2(a + b) = a + 2b + c => a = c
因此我們再設兩個 pointer，一個從頭一個從 X，等速率前進，當這兩個 pointer 相遇時，就是這個循環的起點，因為 a = c

## 如何分辨

- 通常題目所需要的會跟是否有循環有關
- 需要知道一個 linked list 確切的長度

## 題目

- Linked List Cycle (easy)
- Palindrome Linked List (medium)
- Cycle in a Circular Array (hard)
