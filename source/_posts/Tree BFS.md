---
title: 演算法系列#7 Tree BFS
date: 2023-06-06
updated: 2023-06-06
tags: [algorithm]
categories:
  - 演算法
thumbnail: /Tree%20BFS/tree_bfs.png
keywords: bfs, tree, algorithm, 演算法, 教學, leetcode
---

![](/blog/assets/tree_bfs.png)

<!-- more -->

這是一個用 BFS 瀏覽一棵樹的方法，最簡單的理解方式就是他會從樹的頭開始一層一層的往下搜尋

主要會使用 `queue` 的方法，通過把下一層的 node 放進 queue 裡，不斷 iterating 這個 queue 直到 queue 為空

以下為實作方法

```javascript
const queue = [root]
while(queue.length) {
	const currentNode = queue.shift()
	// do waht you want from currentNode

	// push next level nodes to queue
	queue.push(currentNode.left, currentNode.right)
}
```

## 如何分辨

- 當題目要求你在搜尋樹時是用 level-by-level 一層一層的方式進行時

## 題目

- Binary Tree Level Order Traversal (easy)
- Zigzag Traversal (medium)
