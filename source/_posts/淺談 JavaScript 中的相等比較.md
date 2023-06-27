---
title: 淺談 JavaScript 中的相等比較
date: 2023-06-27
updated: 2023-06-27
tags: [js]
categories:
  - 技術科普
thumbnail: /淺談 JavaScript 中的相等比較/equal.png
keywords: seo,網站優化
---

![](/blog/assets/equal.png)

<!-- more -->

相信大家在第一次學 javascript 的時候都有出現過一個疑問是問什麼 javascript 在做相等比較時大家都是用三個等於符號 `===` 而不是像其他語言一樣用兩個 `==` 就好了呢，只被告知說每次遇到要相等比較時用 `===` 就好了，或是用了 `==` 卻出現了無法解釋的 bug

因此這篇文章想來跟大家介紹在 javascript 中，各種的相等比較法以及其區別

## 鬆散比較 ==

首先先來介紹只用了兩個等於的鬆散比較，在 javascript 中，`==` 在比較前，會強制轉換型別與值，我們這裡直接舉一個例子

```javascript
1 == '1'
```

通常在其他語言中，這樣的比較會是 `False` 的，畢竟連型別都不同了，一個是數字一個是字串，然而在 javascript 中，這樣的比較卻會是 `True` ，因為 javascript 在比較前將兩者的型別都調整成一樣了，像上面這個例子，javascript 會把字串調整成數字並做比較。

```javascript
null == undefined
0 == false
```

接著再舉兩個例子，可以猜猜看這兩個的結果會是什麼

答案是兩個都是 true，在鬆散比較中，`null`，`undefined` 都會是一樣的，而 `false` 被轉換成數字後會變成 `0`

而正因為這樣的機制，導致我們在直觀上很難判斷，因此我們幾乎不會使用鬆散比較，以免出現一些我們不好處理的 bug

## 嚴格比較 ===

跟鬆散比較相比，嚴格比較不會強制的轉換型別與值，也因此如果是不同型別的，將會直接回傳 `false`。
這就是平常我們在其他語言中 `==` 一樣的效果，所以在大部分情況下，建議都是使用嚴格比較的。

然而秧歌比較還是會有特殊的情況，例如以下

```javascript
+0 === -0 // true
NaN === NaN // false
```

在某些數學情況下，`+0` 跟 `-0` 是不一樣的，但我們平常其實不需要考慮這些
而 NaN 在 javascript 中用來表示那些無解的數學解，例如負無窮加正無窮，而在嚴格比較中，NaN 不等於任何值，因此也不等於資深自身。

## 同值比較 Object.is

同值比較在使用上基本上跟嚴格比較是相同的，而不一樣的是，在上面所說的嚴格比較的特殊情況時會是相反的結果

```javascript
Object.is(+0, -0) // false

Object.is(NaN, NaN) // true
```

而注意的是雖然是用 Object 但這個方法不管是不是 Object 都是可以放進來使用的

## 結論

以上就是這次關於 JavaScript 中相等比較的各種方式與特點，希望各位看完後能夠更認識與知道為什麼平常都是使用 `===` ，而不是因為大家都這麼用所以就用了。

## References

- https://developer.mozilla.org/zh-TW/docs/Web/JavaScript/Equality_comparisons_and_sameness
- https://www.explainthis.io/zh-hant/interview-guides/javascript/js-equality
