# Lesson 2: 九種常見的 Web3 駭客攻擊與詐騙手法

Author: [XREX Security Team](http://xrex.io/)

社群 [Discord](https://discord.gg/3y3d9DMQ)

同步發表: [XREX](https://tw.xrex.io/web3-%E8%B3%87%E5%AE%89%E6%95%99%E6%88%B0%E6%89%8B%E5%86%8A-%E4%BD%A0%E4%B8%8D%E5%8F%AF%E4%B8%8D%E7%9F%A5%E7%9A%84%E5%8D%80%E5%A1%8A%E9%8F%88%E5%A8%81%E8%84%85%E6%89%8B%E6%B3%95%E8%88%87%E8%A9%B1%E8%A1%93-544253a90edb)

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211229121-fe1ec629-038d-492e-833c-5c30f66bc15e.png" alt="Cover" width="80%"/>
</div>

Web3 是近幾年來的搜尋關鍵字，在許多新聞報導、國際會議、產業研討會以及金融創新相關的討論，都可以看到 Web3 的討論，圍繞在區塊鏈以及加密貨幣帶來的創新與突破；於此同時，也因為相關技術仍處於早期，濫用的情況頻傳，很多人對於 Web3 世界中的詐騙、洗錢和駭客攻擊充滿恐懼。本文從 Web3 概念的討論開始，由加密貨幣平台 XREX 的資安團隊由淺入深地了解 Web3 世界中的資安觀念，解析駭客手法，並提供讀者務實的建議，用以保護自己的個資和數位資產。

### 什麼是 Web3？
1990 年代開始，網路慢慢地深入人類生活的各個層面，從日常生活到政治經濟，一直到我們的學習方法、通訊方式、交友模式與對時空距離的概念，都受到網路這個新興科技的影響。過去 30 年來，全球數十億人都成為全球資訊網中的一員。然而，沈浸於以網路為基礎的強大 IT 設施的同時，我們也正面臨極大的挑戰與入侵。少數科技巨頭壟斷了網路產業，也同時也壟斷了權力，可以單方面決定允許什麼、不允許什麼。

「網路＋電腦」是 Web1.0 的時代，「網路＋移動式裝置」則是 Web2.0。在 Web1.0 與 2.0 的時代，科技巨頭提供服務的同時，也一手掌握用戶產生的數據、資訊、內容，也就是俗稱的「中心化」結構。

Facebook 的言論審查制度、Google 的搜尋演算法、Spotify 向創作者抽取高達 30% 的獲利、線上遊戲停止營運後虛寶價值就歸零等等，都是我們在日常生活中，最貼近也最常見的案例。創造內容的用戶難以獲得分潤，也不掌握任何所有權，甚至在不知情的狀況下被利用，被刻意投放的資訊與廣告影響認知與決策，這些都是 Web1.0 與 Web2.0 所製造出來的問題，這也催生了 Web3 的時代。

Web3 技術被視為解決 Web1.0 與 Web2.0 產生的最佳解答。Web3 的基礎是區塊鏈技術，因為區塊鏈技術原生的「去中心化」結構，具有不可篡改性、公開透明性與開放源碼的天性，無論是內容還是權力，都不再是由大型科技公司與平台一手壟斷，而是由使用者建立、運營和擁有。自 2008 年中本聰發表比特幣白皮書以來，我們逐步想像並踏入 Web3 的世界，秉持著去中心化精神，我們已經看到比特幣、以太坊、NFT、DeFi，一直到現在的 Move-to-earn 爆紅的 STEPN，都是 Web3 的新嘗試、新實驗， 透過不同項目的實踐，將數位自主權交還給用戶，在實現用户共同建立、共同治理的同時，用户也可以分享平臺的價值與利潤。

當然，所有科技在發展演進的過程中，會帶來益處，也同時可能會被濫用而造成問題。現在聽到加密貨幣，很多人的第一個反應就是洗錢與詐騙，當區塊鏈具備去中心化特性的同時，也意味著用戶必須承擔保管資產和身份的絕對責任，一旦用戶遭駭或遭詐騙，沒有任何機構或實體可以擅自更改區塊鏈的紀錄，這也讓許多犯罪集團蠢蠢欲動。

XREX 資安團隊撰寫本文，整理多個 Web3 世界中常見的攻擊手法與慣用話術，讓我們認識不肖份子和駭客的攻擊手法與慣用話術，在區塊鏈建構的 Web3 世界中，學習保護自己的資料與加密貨幣資產。

### Web 3 安全事件損失數據
根據知名區塊鏈安全公司慢霧科技 (SlowMist) 監測數據顯示，從 2012 年到 2022 年 6 月，整個區塊鏈生態系存在至少 787 起被駭事件，損失金額超過 267 億美元。

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211229334-b29c3d1e-cbb3-4bc7-9a0e-ca9eecb19f8a.png" alt="Cover" width="80%"/>
</div>
<p align="center"">圖片來源 / 慢霧科技</p>

根據美國聯邦貿易委員會 (Federal Trade Commission, FTC) 的研究，2021 年至 2022 年第一季，美國就有 46,000 人回報遭到加密貨幣金融欺詐，損失價值超過 10 億美元的加密貨幣。值得注意的是，這項數據並未統計全球數據，也只紀錄了有報案的數據，這也代表還有很多不在檯面上的案件，是我們難以確知的受害人數與損失金額。

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211229526-4d70241a-3995-43af-8a90-128f96cda250.png" alt="Cover" width="80%"/>
</div>
<p align="center"">圖片來源 / 美國聯邦貿易委員會</p>

### 駭客想要的是什麼？
<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211229545-7f6987e1-01ec-42e3-b47d-73aeb766806f.png" alt="Cover" width="80%"/>
</div>

駭客的目的與想要得到的東西，如上圖所示，可以簡化成以下四大類別：

* 加密資產
* 錢包層
* 轉帳權
* Web2.0 憑證

駭客的各種攻擊手段，都是為了嘗試取得以下任一資訊，取得不法獲利：

1. 取得使用者擁有的硬通貨，例如：比特幣、以太幣等強勢加密貨幣或高價的 NFT。最常見也最經典的手法，就是「給 1 塊錢，返還 10 塊錢」投資贈禮騙局。
2. 取得加密貨幣錢包的機密資訊，例如：錢包私鑰、註記詞，或錢包密碼。
3. 取得在智能合約上，使用者轉移資產的核准授權，後續再將使用者的虛擬資產轉道別的錢包。
4. 取得使用者在 Web2.0 的憑證資訊，例如：在加密貨幣交易所的帳號與密碼。

在進入 Web3 的世界時，可以怎麼保護自己的個資以及資產呢？所謂知己知彼，百戰百勝，我們必須清楚地認知到，不管是在 Web1.0、Web2.0，還是在 Web3 的世界裡，都是有風險的，我們可以透過了解常見威脅與攻擊的手法，防止被騙或捲入不法行為。同時，也訓練自己保持良好的資安意識與習慣，隨時提高警覺，不易遭到詐騙或入侵。最後則是在每次按下滑鼠確認之前，勇於質疑，只要有一絲懷疑與不確定，就應該再次確認。

以下，XREX 收集整理了九種常見的 Web3 攻擊手法，教您如何辨識攻擊與詐騙，守護自己的資料與資產安全：

### 九種常見的 Web3 攻擊手法
### 一、憑證釣魚攻擊 (Credential Phishing Attack)
憑證釣魚攻擊，簡而言之就是駭客假冒網站，像是假冒交易所的登入頁面或假冒空投解鎖頁面，使用者誤認為是官方網頁，就輸入自己的帳號與密碼，立刻就被駭客竊走帳密資訊。

駭者會使用 Social-Engineer Toolkit (SET) 或 Goclone 等工具，把正牌網站的前端設計和佈局，原封不動地直接複製到本地伺服器，再另外註冊跟官網相似的網域名稱，並掛上對應的 SSL 憑證。許多使用者因為一時不察，就很容易上鉤。

除了需要特別注意網址的真實性外，也要特別小心所有的通訊管道，因為只要是能與使用者溝通的方式，都有可能成為攻擊途徑，例如：電子郵件、社群媒體、手機簡訊、Telegram 假客服等等。

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211229629-cb4ddbeb-9c4d-4b5d-b8d7-247497cf2de0.png" alt="Cover" width="80%"/>
</div>

<p align="center"">圖 1. 1 / 駭客透過 Email 向使用者發送虛假的 Coinbase 帳號遭鎖定通知</p>

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211229665-32e2122f-1815-48d4-9888-217796ae9c70.png" alt="Cover" width="80%"/>
</div>

<p align="center"">圖 1.2 / 若是點擊 View Accounts，用戶會被導向至釣魚域名 coinbaseclouds.link</p>

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211229703-b40864c3-1efd-4a76-bf6a-642d2c5fab4b.png" alt="Cover" width="80%"/>
</div>
<p align="center"">圖 1.3 / 攻擊者透過簡訊發送釣魚連結，將受害者導到行動裝置版釣魚網站</p>

憑證釣魚攻擊對駭客而言是一個低成本而高報酬的方式，因為發送10 萬封釣魚信件成本僅需幾十塊美金，但只要有一到兩個人上鉤，可能就足以讓駭客回本，甚至得到極高的不法獲利。

如何防範憑證釣魚攻擊呢？XREX 建議您：

1. 將常用網站入口加入書籤或我的最愛，避免誤入釣魚網站
2. 使用 Lastpass、NordPass 或 Keeper Security 等密碼管理器，為不同網站、不同帳戶設定不同密碼，才不會因為一組帳密被盜，駭客就可以發動所謂的「撞庫攻擊」，登入所有不同的帳戶。從資安角度建議，每組密碼應具有至少 10 個字元，其中包括至少 一個大寫字母、一個小寫字母、一個數字和一個特殊符號。
3. 在瀏覽器安裝防詐騙插件，例如：Netcraft Extension、PeckShieldAlert 或 MetaShield，自動檢測釣魚網站。
4. 發現可疑網站即時回報，共同守護去中心化生態系的安全。

### 二、Google 廣告釣魚詐騙
Google 廣告釣魚詐騙與憑證釣魚攻擊類似，駭客偽造虛假的交易所登入頁面、虛假空投解鎖頁面，並註冊與官網相似網域名稱與掛上對應的 SSL 憑證。不同的是，駭客會在 Google 廣告上關鍵字競價，使自己的網站 SEO 排名高於官方網站，也就是當使用者透過搜尋引擎搜尋時，很容易在看見官方網站之前，就誤擊進入假的網站。

下圖我們用最近非常火紅的 move-to-earn 項目 STEPN 為例，在 Google 上輸入 stepn，出現的搜尋結果前四名，都是花錢下廣告的假網站。

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211229744-f713a89d-8b8b-4483-b62e-3903578394d4.png" alt="Cover" width="80%"/>
</div>
<p align="center"">圖 2.1 / 在 Google 搜尋 stepn，可以看到 Google 廣告充斥著釣魚詐騙</p>

如何防範 Google 廣告釣魚詐騙呢？XREX 建議您：

1. 在搜尋關鍵字點擊搜尋結果時，格外注意令人起疑的網域。
2. 將常用網站入口加入書籤或我的最愛，避免誤入釣魚網站。
3. 在瀏覽器安裝防詐騙插件，例如：Netcraft Extension、PeckShieldAlert 或 MetaShield，自動檢測釣魚網站。
4. 發現可疑網站即時回報，共同守護去中心化生態系的安全。
5. 
### 三、假客服釣魚攻擊 (Fake Customer Service)
駭客會在 Telegram、Discord 等通訊軟體上建立假帳號，將顯示名稱、自我介紹、頭像更改為和官方群組客服人員或管理員相同，假冒是項目方並以空投登記、服務滿意度調查等各種名字，大量私訊使用者引誘其回覆。

使用者若是上鉤，駭客再透過其他名目，例如：實名驗證的門檻不符、錢包地址需要驗證等要求使用者提供帳號與密碼，或要求使用者將加密貨幣轉至指定錢包地址，才可以解鎖帳號。

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211229845-3e2b0b5d-0119-482d-b5f7-ffd8cdbf2c3a.png" alt="Cover" width="80%"/>
</div>

<p align="center""> 圖 3.1 / 駭客假冒項目方的客服帳號，將自我介紹改為官方客服的用戶名稱，藉此混淆視聽。 </p>

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211229868-6dffd02a-e904-44de-920e-d121423f5c4c.png" alt="Cover" width="60%"/>
</div>
<p align="center"">圖 3.2 / 假冒的客服人員，要求用戶發送 0.01 BTC 到特定錢包地址才能解鎖</p>

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211229912-896ad74a-f1fd-4f1d-9829-db7511e4843e.png" alt="Cover" width="80%"/>
</div>
<p align="center"">圖 3.3 / 駭客假冒為項目方，宣稱要向使用者發送免費空投</p>


如何防範假客服釣魚攻擊呢？XREX 建議您：


1. 請勿相信 Telegram 或其他社群平台的陌生私訊，官方人員絕對不會突然私訊使用者，更也不會要求以訊息發送帳密資訊。
2. 涉及機敏資訊的協助需求，如: 存提款、實名驗證、帳號安全等等，請透過官方網站列出的支援管道聯繫。
3. 強化 Telegram 個人隱私設定，設置「僅我的聯絡人可將我加入群組」，可參考下方步驟完成設定。

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211229998-9af973c9-b8ad-45e9-86c6-095f7197192b.png" alt="Cover" width="80%"/>
</div>
<p align="center""> 圖 3.4 / Telegram 「僅我的聯絡人可將我加入群組」的設置方式 </p>

談到這裡，我們已經討論了 Web3 的定義、國際統計的駭客入侵事件總數與 Web 3 安全事件損失數據、駭客的意圖及目標，以及三種攻擊手法和防範建議。接下來，我們還將繼續解析更多 Web3 攻擊與詐騙方式。繼續閱讀文章

### 四、社群媒體免費贈送詐騙

我們每天都會使用的各種社群媒體，例如：在 Facebook、Instangram、Twitter 等等，都是駭客常用的工具。駭客會在社群媒體註冊假帳號或盜用其帳號，偽冒知名企業、政治與各領域知名人士的身份，發文宣稱要送出加密貨幣，例如：「向我發送 1 顆以太幣，我將返還 10 顆以太幣給你」，引誘看見貼文的人上鉤。

去年底，印度總理莫迪擁有超過七千萬人追蹤的推特帳號被盜，駭客就[發文宣稱有免費的比特幣，要大家快來搶](https://style.yahoo.com.tw/%E5%8D%B0%E5%BA%A6%E7%B8%BD%E7%90%86%E8%8E%AB%E8%BF%AA%E6%8E%A8%E7%89%B9%E8%A2%AB%E7%9B%9C-%E7%99%BC%E6%96%87%E7%A8%B1-%E5%85%8D%E8%B2%BB%E6%AF%94%E7%89%B9%E5%B9%A3%E5%BF%AB%E4%BE%86%E6%90%B6-064006132.html)，因為是擁有藍勾勾認證的帳號，又是印度總理，很容易讓人信以為真，但是只要點擊貼文中的連結，就會面臨資安風險。

這些社群媒體上的貼文，引誘其他人去點擊特定連結，或是發送加密貨幣到特定地址以換取更多加密貨幣，這些都只是駭客用來吸金的話術。更可怕的是，在受害者向駭客索討受騙金額時，駭客還可能以「需要再向我發送 30% 手續費」等說法，再次行騙。

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211230171-17d583da-5a16-465c-8d86-caaa362a86b4.png" alt="Cover" width="50%"/>
</div>
<p align="center"">圖 4.1 / 駭客利用假冒的粉絲專頁，分享其他帳號的大頭貼照，吸引帳號擁有者的注意 </p>

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211230190-a41ddceb-534e-4ded-b3c9-72c7d7abfd4f.png" alt="Cover" width="60%"/>
</div>
<p align="center""> 圖 4.2 /假冒帳號在本尊的推文底下留言，並且立刻安排多個假帳號附和、按讚 </p>

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211230198-fd4340e7-af43-4aa4-bc91-932c97715303.png" alt="Cover" width="60%"/>
</div>
<p align="center""> 圖 4.3 / 駭客直接盜用官方認證帳號，騙取使用者信任 </p>


如何防範免費贈送詐騙呢？XREX 建議您：

1. 多方驗證消息來源，請勿聽信任何免費贈送的廣告。
2. 對於免費贈幣、以一換十這種「好得不真實」的活動，必須三思。
3. 必須謹記，去中心化金融不存在反悔操作，錢轉出去就回不來了。
4. 對任何轉帳或授權有關的錢包應用程式彈出式視窗，保持謹慎。

### 五、龐氏騙局 — 高報酬投資詐騙
「龐氏騙局」是大家經常聽見的名詞，但究竟什麼是龐氏騙局呢？基本上，龐氏騙局的運作模式是以投資為名，以高額回報誘騙受害者投資。龐氏騙局通常第一眼看，會覺得與普通證券基金的模式無異，但在龐氏騙局中，投資回報事實上是來自後面加入的投資者，而不是公司自身盈利。

龐氏騙局最初發生於 20 世紀初的美國，吸引第一批投資人之後，不斷再拉入更多投資人將資金投入項目。實際上，項目並沒有盈利，而是將後期投資人的資金變成了早期投資人的利息，今天我們經常聽到的「資金盤」或「老鼠會」，就是龐氏騙局的各種變體。

如何判斷龐氏騙局呢？龐氏騙局的常見特徵是模糊不清的經濟模型，也就是項目本身很難運作也不知其獲利來源，卻可以承諾投資人明顯不合理的高收益報酬率，從以下的平台與對話截圖就是實例。

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211230305-0e6c25ac-0535-4757-83e9-8257d1797a7e.png" alt="Cover" width="80%"/>
</div>
<p align="center"">圖 5.1 / 平台提供日收益率達到 2.72% 的理財產品，相當於年化報酬率 1000%，極不合理  </p>

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211230329-e19be2f8-1b71-47ab-bac7-dc85b71efdb8.png" alt="Cover" width="80%"/>
</div>
<p align="center"">圖 5.2 / 平台宣稱自動提單套利、預判指標與分析師與內線消息老師，引誘使用者投資  </p>

如何防範龐氏騙局詐騙呢？XREX 建議您：

1. 建議使用擁有牌照、合法合規且背後團隊清晰的交易所，例如 XREX 在美國、加拿大立陶宛、愛沙尼亞與台灣，都完成相關的登記、反洗錢規定以及許可，同時也正在申請新加坡與杜拜的執照。
2. 勇於質疑，對於平台提供的消息與資訊必須再次驗證其真實性，不讓詐騙集團打模糊戰，例如: 套利與挖礦是否正相關、分析師履歷真實性等等。
3. 思考報酬率是否合理、是否偏離市場行情，切忌 FOMO (Fear of missing out)。

### 六、項目方捲款跑路 Rug Pull
項目方捲款跑路又稱「拉地毯」(Rug Pull)，是加密貨幣中的一種詐騙形式。Rug Pull 一詞泛指項目方募集了資金之後就放棄經營項目，同時在發行代幣衝上一定價格時，短時間內拋售項目方手中的發行代幣，一瞬間使投資人擁有的發行代幣變得分文不值。

近年來最著名的，就是在 Netflix 韓國原創劇集《魷魚遊戲》掀起全球風潮，結果出現了一個利用戲劇噱頭發行的代幣魷魚幣（SQUID)，短短一星期內漲幅數十萬倍，卻又一瞬間崩盤，投資人血本無歸又無處求償。

Rug Pull 也可能發生在未經過資安審計的智能合約上，項目方可以透過在代幣合約裡留下後門，並在募集資金之後操控代幣供應量。

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211230424-27cf4410-5afb-4fd2-96c4-4e32626721f5.png" alt="Cover" width="60%"/>
</div>
<p align="center""> 圖 6.1 / 非 Netflix 官方或《魷魚遊戲》劇組團隊發行的魷魚幣 (Squid Coin)，七天內代幣價格從 $0.01 衝到 $2861，又一瞬間崩跌至 $0.0008  </p>


如何防範項目方捲款跑路 Rug Pull 呢？XREX 建議您：

1. 挑選項目時，必須要先了解項目團隊的 Linkedin、研究項目的白皮書等資訊。一個正常的項目，白皮書的內容絕對不是空泛的，其中也必須包含、長期目標、項目所解決的問題、背後技術說明，以及團隊真實性等等。
2. 大部分的項目會使用中心化或去中心化交易所進行募資，可以觀察項目代幣是否被前幾名去中心化交易所認證，並且透過鏈上數據分析，觀察項目代幣的交易量、流動性狀況。
3. 確認智能合約是否有經過多家資安公司審查，以及審計報告是否有開源。
4. 觀察社群媒體對該項目的討論熱度，是否有機器人炒熱流量。

### 七、助記詞釣魚 Seed Phrase Phishing
助記詞 (Seed Phrase) 通常是 12 到 24 組的英文單詞，設計原意是方便讓用戶管理錢包私鑰，當使用者忘記私鑰時，助記詞可用來恢復私鑰，並讓使用者重新訪問錢包。我們可以想像錢包私鑰就像是註冊在 Medium 帳號密碼，當你忘記密碼時，網站通常會提供「忘記密碼」的功能，欲恢復密碼會需要驗證註冊郵件信箱以及 Email 與一次性密碼 (​​one-time password, OTP)。

註記詞的設計用意是能夠透過密碼學達成「恢復密碼」的功能，所以只要任何人得到你的助記詞，就有權限訪問你的加密資產。

![image](https://user-images.githubusercontent.com/52526645/211230520-fd21d858-41f0-44f4-ab4e-7035891d86cd.png)
<p align="center""> 圖 7.1 / 一個售價明顯低於市場行情的假 OpeaSea NFT 市集，在交易時要求使用者輸入助記詞 </p>

如何防範助記詞釣魚呢？XREX 建議您：

1. 永遠不要洩漏助記詞，助記詞只會用來恢復錢包，沒有其他用途。
2. 請妥善保管助記詞，會需要輸入助記詞的應用程式，一律是詐騙。
3. 發現可疑網站即時回報，共同守護去中心化生態系的安全！

### 八、假冒錢包與插件
假冒的錢包或錢包插件，會套用正版錢包的介面與設計，讓用戶誤以為是項目官方的網站，但駭客實際上在假冒錢包與插件的後端程式碼偷設後門，駭客可竊取錢包的助記詞 (Seed Phrase)來盜取使用者的資產。

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211230556-fcc7e217-4c6d-43c4-9900-b52261f145f2.png" alt="Cover" width="80%"/>
</div>

<p align="center""> 圖 8.1 / 假造的 MetaMask 瀏覽器插件下載。圖片來源 / Objective-See  </p>

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211230566-532e4abe-628f-4b37-b6a3-a7a70bd751ed.png" alt="Cover" width="80%"/>
</div>

<p align="center""> 圖 8.2 / 偽冒的 AppStore 要求使用者下載描述檔，安裝後即可從不受信任的來源下載具有後門的 MetaMask。圖片來源 / Objective-See  </p>

如何防範假冒錢包與插件，避免安裝可疑行動應用程式呢？XREX 建議您：

1. 永遠不要在越獄裝置或已 Root 裝置使用加密貨幣。
2. 一定要從官方來源，如：Apple AppStore 或 Google Play Store 下載行動應用程式。
3. (僅限蘋果 iOS) 不要安裝或信任來源不明的描述檔，這可能會使你在無意間安裝惡意程式。

### 九、批准授權詐騙 Approval Scam
除了讓受害者主動轉帳資產給駭客這類「傳統詐騙」以外，在智能合約中，可以設定使用者是否要授予 ERC20 Token 轉帳權給某地址。ERC20 Approve 的設計原意，是為了讓智能合約有權動用使用者的資產，舉例來說，使用者授予某套利合約轉帳權限，套利合約就可動用使用者的資產，在去中心化交易所自動地進行搬磚套利。

然而 ERC20 Approve 這樣的設計，也成為駭客濫用的工具。駭客透過釣魚手法，讓使用者在無意間簽署批准轉帳授權的交易，當使用者未嚴格確認自己所簽署的交易內容就送出時，駭客即可取得受害者錢包的資產轉移權，透過 ERC20 Token 合約的 transferFrom 功能，將受害者的資產轉移至自身錢包。

近期最知名案例，就是[台灣歌壇天王周杰倫的 NFT 無聊猿遭盜](https://www.blocktempo.com/jaychou-bayc3738-hacked/)，以及[駭客濫用 NFT 平台 OpenSea 發動新型態詐騙，先是隨機空投用戶，之後故意在平台上炒高價格，出價引誘受害者至釣魚網站](https://www.blocktempo.com/exploring-the-latest-nft-scam/)。

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211230654-97a22421-c6a0-425c-96dc-8c0117e2065d.png" alt="Cover" width="60%"/>
</div>
<p align="center""> 圖 9.1 / 駭客在研討會上張貼虛假的 QRCode，宣稱可領取免費會場 NFT，將用戶引導至釣魚網站</p>

<div align=center>
<img src="https://user-images.githubusercontent.com/52526645/211230665-c28bc5dc-a714-4071-a241-84f5b534735c.png" alt="Cover" width="60%"/>
</div>
<p align="center""> 圖 9.2 / 駭客宣稱可以領取免費的 NFT，但交易內容實際為使用 setApprovalForAll 函式，授予駭客轉帳權限</p>

如何防批准授權詐騙呢？XREX 建議您：

1. 不小心授權給不明地址時，請即時撤銷權限，避免進一步損失。
2. 執行交易前請確認交易內容，避免執行到意料之外的操作。
3. 發現可疑網站即時回報，共同守護去中心化生態系的安全！
4. 定期檢視地址授權狀況，為不明地址撤銷權限，以下三個是常用工具：
* https://etherscan.io/tokenapprovalchecker
* https://revoke.cash
* https://approved.zone/

### 結語
Web3 概念與應用還在相對早期，其去中心化的特性，確實可以為人類世界帶來巨大的變革，尤其是在金融領域。但於此同時，平台以及用戶也必須清楚地知道，Web3 世界中還是暗藏了許多風險，必須要時刻謹記並加以防範。

本文是 XREX 資安團隊，針對近期常見的 Web3 攻擊手法與話術整理的介紹，希望可以協助更多人認識到自己與惡的距離，並隨時保持警覺，以免落入圈套。
