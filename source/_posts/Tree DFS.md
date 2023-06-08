---
title: 演算法系列#8 Tree DFS
date: 2023-06-07
updated: 2023-06-07
tags: [algorithm]
categories:
  - 演算法
thumbnail: /Tree%20DFS/tree_dfs.png
keywords: dfs, tree, algorithm, 演算法, 教學, leetcode
---

![](/blog/assets/tree_dfs.png)

<!-- more -->

與 BFS 相反，是以深度為優先的搜尋方式，會先搜尋其中一個 children 並且持續往下搜尋，直到到底了再搜尋另一個 children

主要會使用 `recursion` 或是 `stack` 的方式來實作

在執行一個非 leaf node 時主要會思考兩件事

1. 是否要執行當前 node 並且決定執行的時間點，一個是現在執行（pre-order），一個是在兩個 children 之間執行（in-order），最後一個則是在兩個 children 執行完後執行（post-order）
2. 對兩個 children 執行 recursive call

```javascript
// 以下為 recursion 方法執行 DFS
const dfs = (node) => {
	if (node === null) return
	// ... do what you want to the current node
	dfs(node.left)
	dfs(node.right)
}
dfs(root)
```

## 如何分辨

- 當題目需要你用 in-order，pre-order，post-order 時
- 當題目需要你尋找會在 leaf 附近的目標時

## 題目

- Sum of Path Numbers (medium)
- All Paths for a Sum (medium)
