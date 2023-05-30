---
title: Preflop 進階
date: 2022-9-19
updated: 2022-9-19
tags: [Poker]
categories:
  - Poker
---

![](/blog/assets/preflop.webp)

<!-- more -->

上一章節講了我們在 preflop 的時候所需要的一些基本觀念，本章將延續上一章來介紹更進階的 preflop 觀念。

# Equity realization

這邊要再講一下 equity realization，我們都知道 equity realization 是會根據你的牌走不走得到 showdown 來決定的，而因此 OOP 會比 IP 更難實現 equity，因為位置的關係，IP 可以更好的做一些決定也更能走到 showdown，需要各位記住這點，因為接下來的觀念都會用到這個概念。

# SPR stack pot ration

定義上來講就是你身上的有效籌碼去除以底池，因此 SPR 越高，就是你身後的籌碼越多，越可以在後面做一些操作。

而這邊有個觀念就是，當 SPR 越高的時候，IP 的優勢越大，而 SPR 越低的時候，OOP 的劣勢越小。

因為 SPR 越低就代表大家越接近 all in，而越接近 all in 那麼位置的優勢就沒那麼大了，因為你就算有資訊跟後手優勢但你有效籌碼也沒辦法再做什麼操作了，基本上就是看雙方的 equity 來比大小。

因此，IP 越希望在 preflop 的時候 SPR 越大，這樣 postflop 才能善用自己位置的優勢，而 OOP 則相反。

# Defend 3 bet from IP

了解上面兩個觀念後我們來看，當我們在 IP 的時候要怎麼應對其他人的 3bet。

再有位置的時候我們為了不要讓 SPR 下降的太快，因此我們 call 的比率會較多，4bet 的較少。

且 4bet 的時候大多是選擇有 blocker(手上有A、K) 的情況，來阻擋對手的 5bet，因為我們 4bet 後最害怕的是對手的 5bet，除了 SPR 上升外，也會讓我們很難去做決定。

# Defend 3 bet from OOP

那來到 OOP，我們最希望的當然就是減少我們到 postflop 時的位置劣勢，因此我們更願意拿強牌來 4bet，以降低 SPR，然而我們 4bet 後最怕對手跟下來但是我們的手牌沒有足夠的 equity，因此 OOP 4bet 會優先選擇 equity 來讓對手 call。

# Cold 4 bet 冷4b

冷 4b 的意思是前面的人 3b 時自己還沒投過錢的時候，4bet。

通常 4b 代表超緊的範圍，因為你要同時面對兩個人(已經投錢)的範圍

而我們在 combo 的選擇上通常會選擇 blocker，因為要儘量阻擋對手的 5bet jam，這樣我們才比較好實現 equity。

然後因為我們 c4b 代表很緊的範圍，因此我們的 size 選的越小越好，因為當我們的 size 太大時，對手可以很好的蓋牌，且如果真的遇到 5bet，我們也可以直接蓋牌，不會損失太多的錢。

# 建立自己的範圍

講完 preflop 的策略後，最後我們來講一下要怎麼記得自己的表格跟 range

## 簡化策略

雖然我們看 GTO 上，我們有可能有些 combo 要玩 15%，有些 50%，但其實有些邊緣的 combo 我們是可以不玩的，相比 GTO 偏離帶來的 EV 損失，自己的策略失誤所帶來的 EV 損失是更為嚴重的，因此剛開始時可以先把策略簡化，讓自己可以容易執行。

## 如何調整 Range

上面講了我們要簡化自己的策略，因此我們有兩種最常見的辦法來簡化

首先我們看到 GTO Wizard solution 的簡化策略，可以先把外圍的邊緣 combo (不同花為主)放棄不玩，以及一些自己不太會處理的 combo 不玩，因為就算我們這些不玩，對手其實也很難去察覺這些微的差距

以上就是 preflop 的所有介紹，其實還有很多更深的策略以及觀念，但對於一個新手來說上面這些就已經需要很多時間來學習了，且對自己的 EV 也有很大的幫助，希望大家看完後都能更了解自己 preflop 該做的事情。
