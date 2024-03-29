---
title: Zettelkasten 筆記法筆記法
date: 2021-08-13 20:47:10
updated: 2021-08-13 20:47:10
tags: [Note taking]
categories:
	- 工具分享
keywords: zettekasten, 卡片盒筆技法, 筆記, 教學
thumbnail: https://miro.medium.com/max/1838/0*bgEPxNyQ4tI7F8vs.png
---

![](https://miro.medium.com/max/1838/0*bgEPxNyQ4tI7F8vs.png)

 <!-- more -->

## 為什麼要記筆記

筆記對於我們而言不外乎就是為了幫助記下我們當前無法記載腦好海裡面的知識，或是為了怕日後我們以為可能會忘記的內容，在日後可以有效的找回自己之前所學過的東西。因此，筆記對於我們來說可以稱作為我們的第二大腦。

然而，我們真的能夠有效的使用這些所記下來的知識嗎？開始思考這些問題後，我發現以前不管是在學校還是自己學習所記下的筆記中，幾乎沒有一個筆記在現在能夠再次為我所用，或是讓我再去找到該資料。也就是說，之前所記下的知識，如果現在已經忘記的話，幾乎就等於消失了，就算我現在正需要某個之前紀錄過或學過的知識，我也幾乎不可能再回去那堆筆記裡面找我所需要的那一段筆記，這不就表示，之前的筆記到現在其實都沒有用了，甚至當下所做的幾乎都是白工，原本的目的是能夠當作我們的第二大腦的筆記為什麼會毫無作用？

[[Why manage your knowledge is important]]

## 傳統做筆記的方法有什麼問題

### 共用性太低

我舉一個我自己的例子，我在開始學習網頁前端的時候，學到一點是，整個網頁上每樣東西都是一個元件，例如按鈕、表格、輸入視窗，有些元件有可能會在 A 頁面使用到，B 頁面也使用到，那我們就可以把這些重複的元件放在一個地方，當有需要的時候就把他們 import 進來，這樣就不需要又重新寫一次這個元件所需要的 html tag、樣式，以此來更方便的整理程式碼，也提高生產效率。

![](https://raw.githubusercontent.com/diegohaz/reuse/master/branding/graphic.png)

然而我們現在寫筆記的方式，卻像是我把 A 頁面的內容都寫在同一份檔案裡，B 頁面如果也有一些同樣內容時，我們卻也只能再重複一次，把這些相同的內容寫在 B 檔案。比如說現在課程在教第一章，裡面有提到許多名詞定義或是觀念，然而我們卻時常把這些內容都寫在一起，並把他們歸類在 xxx 第一章，而下次我們又遇到某個第一章所講道德觀念時，我們卻沒辦法把第一章那個時候寫下的東西拿過來給我們使用。

### 視角太過狹隘

一樣據剛剛的例子，當我們把某些觀念寫在第一章裡面，這些內容其實就變相的綁在一起了，導致當我們在思考其他看似跟第一章的內容沒關係的事情時，我們很難去把某些在第一章的觀念與當前所思的事有所連結，這也是我覺得為什麼有時候有人對於一個問題時能夠想到我沒想到的，但我明明也知道有這個方法。

### 跟我們的大腦儲存資訊的方式不一樣

![](https://graphstream-project.org/media/img/randomWalk.png)

我們的大腦其實就像一個 [graph](https://blog.chairco.me/posts/2017/05/algorithm%20directed%20acyclic%20graph.html) 一樣，每個知識點其實就是一個單獨的 node，這些 node 與其他的 node 有所連結，最後所形成的這張圖，就是代表了我們的認知。所以，其實每個知識點幾乎是沒有階層性與區隔的，都在同一個平面上，然而我在整理筆記時卻時常用把筆記分類成 A、B、C，甚至再往下到 1.a 1.aa ...，這種整理方法除了跟我們大腦的思考方式不太一樣外，我們也下意識的把這些知識做分類了，然而知識的分類基本上不太可能可以清楚的分類出A、B、C，如果換個角度，可能也可以分類成正方形、三角形、圓形，也就間接的讓我們的思考有被分類框架限制的感覺。

[[How our brain works for knowledge]]

## 對於儲存知識庫類型的筆記應該要有的樣子

### 1. 每個筆記只有一個想法或觀念

我們必須把每個知識都拆成一小個 node，而每一個 node 就是一張筆記，這除了能夠讓筆記的共用性提高外，也可以讓你在寫筆記的時候只專注在一件事情上面，而不是還要意思思考其他的想法，這麼做可以更加的了解當前這個想法，深度也會比較深。

### 2. 筆記之間可以做雙向連結

如同上面所講，每個筆記其實就只是單獨的一個想法而已，而我們的知識就是建立在這些單一想法們之間的連結，連結的越多，在看一件事情的時候就有更多的角度來思考。

### 3. 可以把這些筆記之間的連結做圖像化

這可以幫助我們從高點鳥瞰這些筆記，比起單獨的看一個一個的筆記，把這些筆記變成一個巨大的 graph，可以更清楚的了解每個筆記之間的連結，更全面的思考方式。

[[How to take note and manage them like our brain does]]

## Zettelkasten 是什麼

講了那麼多，終於才提到了標題所提的，Zettelkasten 筆記法到底是什麼。這邊我就不過多的描述者是誰發明的，怎樣怎樣的，我主要想談的是這個方法的概念，以及我怎麼利用它來達成上面的目標。

首先，Zettelkasten 基本上會有三種的筆記類型，Fleeting note, literature note, permanent note。

- Fleeting note：
這種筆記最主要的目的是幫助你記下當前所想到的想法或是再看一本書時覺得特別重要的句子，這類型的筆記不一定要寫的很詳細，也不太需要特別去整理架構什麼的，就如同字面上所說，他就只是紀錄一些想法而已，而且我們之後會對這些想法再做整理，然後封存。這種筆記可以隨便記在你方便的地方，可以是手機上隨便的記事本，也可以是真實的筆記本。

- Literature note：
這類型的筆記有點像是 reference 的感覺，當你讀完一本書或是看完一篇文章或影片，你可以把這隻影片所講的內容用你的語言重新整理一次，也可以從 Fleeting note 裡面去找你那時候所標記的內容或是想法，因此筆記會看起來像是，xxx書名，作者：xxx，...... 裡面的內容，這樣。這種筆記主要是幫你保存這個來源的大致上內容，讓你下次如果又想到這個來源時，可以直接從這裡找到所需要的內容。

- Permanent note：
再來是 Zettelkasten 的核心，也是達成我們的目的中最重要的一種，Permanent note，顧名思義就是你希望永久保存的筆記，這種筆記的特點是，標題會是一個想法，那這個筆記裡面的內容就只會講到標題所提到的想法，那其餘有關連的想法就使用雙向連結的方式去連結。例如假設我現在有個筆記是「如何xxx才能xxx」，裡面就提到了有ABC三種方法，那就可以把這個筆記連結到另一張的筆記「ABC之間的差別」，接著再往下繼續連結。最後所形成的筆記網路就會成為你的知識。
那要怎麼開始寫 Permanent note 呢？其實就是直接使用前面提到的兩種 note，你可以在你的每一天，抽出一點時間來看一下你今天的 fleeting note 上面的想法，並從中找出你覺得有意思的想法，或是從 literature note 裡面找出你覺得想討論的點或是自己的看法，並且把者每個想法都寫成一張一張的筆記，就可以創造出一些你的初始知識點了。
這樣就完了嗎？不，Permanent note 的來源不一定只能限定於 fleeting note 或 literature note，你可以透過新加入的筆記，與現有的筆記做比較或是拿起來一起討論，形成新的筆記，接著這些筆記可能就可以再跟其他的筆記做結合，形成另一個新的筆記。

發現了嗎，這種方法可以然你不去透過接觸新的知識，而是透過你現有的知識，來生成屬於你自己的知識，而這些連結就會是你自己獨有的，別人或許想不到的知識點。

那除了三種筆記外也可以自己再多加比如說 Mapping note，這種筆記就會類似一種集合的概念，假設我今天想要研究如何提高生產力，那我就可以開一個新筆記叫「如何提高生產力」，而這張筆記的內容就是一堆跟生產力有關的筆記的連結。

而為了達到這些目的，Zettelkasten 也有一些規則需要遵守
1. 首先是 Permanent note 一定要是一個想法就一張，儘量不要同時在一張筆記上提到兩種想法
2. Literature note 跟 permanent note，盡量用自己的語言寫下來，尤其是 Permanent note，如果知識 copy/paste 你看的書或影片，那麼有可能你其實根本就沒有真的了解它，用自己的語言寫，除了能讓你檢視自己究竟了解多少外，也可以讓10年後看到這張筆記的你，不會看不懂你到底在工三小。

[[Zettelkasten note taking]]

## 現有的筆記工具

![](https://cosmonaut-storage.s3.amazonaws.com/846877108225678_hero-image.png)

除了 Fleeting note 以外，Literature 與 Permanent note 盡量使用可以達到雙向連結，且有提供 graph 圖像化功能的工具，像我自己在使用的是 Obsidian 這個工具，除了他是免費的外，他的檔案也是單純的一個一個 markdown 檔，直接存在本地的，容易備份外也不怕哪天這個軟體掛了你之前所記下來的筆記也都不見了。

那其他像 Roam Research 等這種工具我沒用過所以就不提了。那假設你是一個工程師且有在使用 VScode 的話，我推薦一個 extension [Foam](https://foambubble.github.io/foam/) 他可以讓你直接在 VScode 裡面做到 markdown 雙連結以及圖像化的表示，不過我自己用下來還是覺得 Obsidian 好用一點。


## 結論

其實這種筆記法就像是一種更複雜的心智圖而已，把一般心智圖上的每個 node 轉換成每個筆記，並且更複雜的把他們連在一起。

我覺得這個方法最有價值的點是，我可以很容易的從我現有的筆記中去產生新的想法，並且一直迭代下去，有點像是更有系統化的 brainstorming，且長期保持的話，可以培養習慣用不同的想法去看待一件事情。

以上就是我自己對於 Zettelkasten 這種筆記方法的理解，網路上也有很多其他人的解釋，也有不同的作法，但是大概念是一樣的，只要概念相同，不同的作法所產生的效果都是一樣的，只需要找到自己最舒服的那種方式就好了。

有時間的話可能再來寫一下我 Obsidian 是怎麼做的。
