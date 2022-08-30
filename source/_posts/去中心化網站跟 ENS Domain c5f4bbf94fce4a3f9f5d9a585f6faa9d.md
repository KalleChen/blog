---
title: 去中心化網站跟 ENS Domain
date: 2022-08-24
tags: [web3]
categories:
  - Tutorial
  - Web3
---

![](https://s3.eu-central-1.amazonaws.com/curaze-web-prod/photos/shares/WEB3-WEB2.0-WEB1.0.png)

<!-- more -->

# 去中心化

## 什麼是去中心化？

如果有在關注區塊鏈的應該對於去中心化已經有一定的瞭解了，簡單的來講就是你的資料或者是服務，不是由一個單一的設備或者是團體來維護的，而是由各個網民共同維護持有的，相對於中心化來說，擁有更透明，無法竄改等優點。

## 什麼是 IPFS？

IPFS 中文星際文件系統，是一個分布式 web，點對點的傳輸協議，簡單來說每個 IPFS 的使用者都是一個節點，而每個節點都會儲存一些其他人丟在這個 IPFS 網路的檔案資料，每當我們上傳檔案上去時，IPFS 會算出一個我們這個檔案的 CID，並且每次要瀏覽這個檔案時會需要透過這個 CID 去搜尋，當別人透過這個 CID 來瀏覽我們的檔案時，也會下載一部分到他的節點，這樣不僅幫我們備份了這個檔案，當其他人也透過這個 CID 來查找時，也會去其他有這個檔案的節點搜尋，進而提升查找速度。

## 那網頁怎麼去中心化？

對於一個傳統的靜態網頁來說，其實整個網頁可以簡化成三個檔案，HTML、CSS、JS，只需要這三種檔案就可以直接開啟一個簡單的靜態網頁了，不需要有什麼背景程式在跑，也就是說只要有一個地方可以放上這些檔案，並且讓其他人可以瀏覽就可以弄成一個網頁了，像是大家熟悉的 github page 就是用這種方法的。

那麼只要將這個靜態網頁的檔案放在 IPFS 上，接著透過這個 CID 來查找，就能製作出一個簡單的去中心網站了。

這邊推薦一個幫你維護 IPFS 節點的網站 [Pinata](https://app.pinata.cloud/)，只需要將你的檔案放上去，之後就可以透過 CID 來瀏覽了。

![Screen Shot 2022-08-10 at 3.39.33 PM.png](/blog/assets/Screen_Shot_2022-08-10_at_3.39.33_PM.png)

# ENS Domain

然而如果每次要跟別人分享你的網站都需要透過 CID 來查找的話總是不方便的，像是原本的中心化網站也不是直接給你網站的 ip 位置，而是透過 DNS，來讓大家更好的去到你的網站頁面，那麼去中心化也有類似的服務，那就是 ENS (Ethereum Name Service)

ENS 的運作方式類似於 DNS，也是像 [google.com](http://google.com) 這樣簡單的網域名稱，只是結尾都是 .eth 並且需要使用 ETH 購買。

首先我們要去 ENS Domain 的官網 [https://app.ens.domains/](https://app.ens.domains/) 並且連結你的錢包(這邊就不做錢包的教學了，總值就是開一個 ERC20 的錢包並且連接)，接著就可以搜尋你想要的名稱了，每個名稱的價位可能都不一樣(取決於長度，越短可能會越貴)，並且如果目前這個名稱已被買起來的話就需要去看看擁有者有沒有在 opensea 上販售了。選好後就是一連串的註冊跟付款，要注意註冊的時候也會收 gas 費用。

![Screen Shot 2022-08-10 at 3.40.09 PM.png](/blog/assets/Screen_Shot_2022-08-10_at_3.40.09_PM.png)

成功購買後就可以進入這個網域的編輯頁面了，ENS 可以做的事情其實不只是像 DNS 的使用方法一樣，他也可以當作你錢包導入名稱，也有其他可以設定上傳的東西，像是你的 NFT 頭像之類的，但這邊就不多介紹了，我們要注意的是 CONTENT 這個欄位，這裡就是可以把你那一長串已經放在 IPFS 上面的網站的 CID 放上來的，各式是 ipfs://CID，成功並且儲存後，就可以透過 [https://ensname.eth](https://ensname.eth) 來進入你的網站了，但如果本身瀏覽器沒有直接支援 ENS 的話，就會需要在後面加一個 link [https://ensname.eth.link](https://ensname.eth.link) ，這樣一個簡單的去中心化網站加上 ENS Domain 就完成了。

![Screen Shot 2022-08-10 at 3.40.52 PM.png](/blog/assets/Screen_Shot_2022-08-10_at_3.40.52_PM.png)

像我就幫自己做了一個簡單的 link tree 的去中心化網站 [https://kallechen.eth.link/](https://kallechen.eth.link/)

# 結論

其實去中心網頁跟 ENS 到目前為止還沒有到有什麼真的很實用的地方，但有一個自己的 ENS Domain 並且可以跟朋友炫耀還是一件很酷的事情。
