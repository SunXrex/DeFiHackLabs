# OnChain Transaction Debugging: 1. Tools

Author: [SunSec](https://twitter.com/1nf0s3cpt)

當初我在學習鏈上分析時，很少相關教學文章，只能自己慢慢地收集資料從中挖掘如何分析到測試。 我們將推出一系列 Web3 安全的教學文章, 幫助更多人加入 Web3 安全，共創安全網路。

第一個系列我們將介紹如何進行鏈上分析到撰寫攻擊重現。

----
## 工欲善其事，必先利其器
在進入分析之前，我會分類列出一些常用工具，正確的工具可以幫助你做研究時更有效率。
### Transaction debugging tools
[Phalcon](https://phalcon.blocksec.com/) | [Tx.viewer](https://tx.eth.samczsun.com/) | [Cruise](https://cruise.supremacy.team/) |[Ethtx](https://ethtx.info/) | [Tenderly](https://dashboard.tenderly.co/explorer)

Transaction Viewer 這類工具是最常用的，可以幫助我們針對想要分析的交易 Transaction，以可視化列出函數呼叫的流程以及帶入的參數等。
每個工具大同小異，只差異在鏈的支援度不同，我個人是比較常用 Phalcon 和 Sam 的 Transaction Viewer，如果遇到不支援的鏈則會使用 Tenderly，Tenderly 支援最多鏈，但是可讀性就不是這麼方便，需要 Debug 慢慢分析。不過我最初在研究鏈上分析是先學習 Ethtx 和 Tenderly。

以 JayPeggers -Insufficient validation + Reentrancy 事件來當例子 [TXID](https://phalcon.blocksec.com/tx/eth/0xd4fafa1261f6e4f9c8543228a67caf9d02811e4ad3058a2714323964a8db61f6)
使用 Blocksec 開發的 Phalcon 工具來說明，下圖可以看到該交易的基本資訊和餘額變化，從餘額變化可以快速看出攻擊著大概獲利多少，以這個例子攻擊者獲利 15.32ETH。

![圖片](https://user-images.githubusercontent.com/52526645/210571234-402d96aa-fe5e-4bc4-becc-190bd5a78e68.png)

Invocation Flow 可視化函式調用流程: 可以讓我們知道這一筆交易調用流程和函式呼叫的層級，有沒有使用閃電貸、涉及了哪些項目、每的函式帶入的參數和原始參數等等

![圖片](https://user-images.githubusercontent.com/52526645/210572053-eafdf62a-7ebe-4caa-a905-045e792add2b.png)

換 Sam 的 Transaction Viewer 來看看 [TXID](https://tx.eth.samczsun.com/ethereum/0xd4fafa1261f6e4f9c8543228a67caf9d02811e4ad3058a2714323964a8db61f6)
跟 Phalcon 類似但 Sam 整合了許多小工具在裡面，如下圖的眼睛點下去可以看到 Storage 的變化。

![圖片](https://user-images.githubusercontent.com/52526645/210574290-790f6129-aa82-4152-b3e1-d21820524a0a.png)

點擊最左邊的 Call，可以把原始 Data 嘗試 Decode。

![圖片](https://user-images.githubusercontent.com/52526645/210575619-89c8e8de-e2f9-4243-9646-0661b9483913.png)

再來換 Tendery 來看看 [TXID](https://dashboard.tenderly.co/tx/mainnet/0xd4fafa1261f6e4f9c8543228a67caf9d02811e4ad3058a2714323964a8db61f6)
在 Tendery 介面上，一樣可以看到基本資訊，但在Debug的部分就不是可視化，需要一步一步 Debug 走下去，不過好處是可以邊 Debug 邊看程式碼。

![圖片](https://user-images.githubusercontent.com/52526645/210577802-c455545c-80d7-4f35-974a-dadbe59c626e.png)

到這邊就可以幫我們釐清大概這筆交易做了哪些事情，在還沒有開始寫 Poc 時，如果想要快速重放攻擊可以嗎? 可以! 可以使用Tendery 或 Phalcon，這兩個工具另外支援了模擬重現交易，在上圖右上角有一個按鈕 Re-Simulate，工具會自動幫你帶上該交易的參數值如下圖
從圖中的欄位可以依照需求任意改變如改block number, From, Value, Input data 等

![圖片](https://user-images.githubusercontent.com/52526645/210580340-f2abf864-e540-4881-8482-f28030e5e35b.png)

### Ethereum Signature Database

[4byte](https://www.4byte.directory/) | [sig.eth](https://sig.eth.samczsun.com/) | [etherface](https://www.etherface.io/hash)

在原始 Input data，前面 4bytes 為 Function Signature. 有時遇到 Etherscan 或分析工具無法解出來時，可以透過 Signature Database 來查看看可能是什麼 Function。

以下舉例假設我們不知道 0xac9650d8 是什麼 Function
![圖片](https://user-images.githubusercontent.com/52526645/210582149-61a6d973-b458-432f-b586-250c94c3ae24.png)

透過 sig.eth 查詢，可以看到這個 4 bytes signature 為 multicall(bytes[])
![圖片](https://user-images.githubusercontent.com/52526645/210583416-c31bbe07-fa03-4701-880d-0ae485b171f7.png)

### Useful tools

[ABI to interface](https://gnidan.github.io/abi-to-sol/) | [Get ABI for unverified contracts](https://abi.w1nt3r.xyz/) | [ETH Calldata Decoder](https://apoorvlathey.com/eth-calldata-decoder/)

ABI to interface: 在開發 Poc 時需要其他合約需要有 Interface 接口，可以透過這個工具幫你快速產生你要的接口。
先去Etherscan 把 ABI 複製下來，貼過去工具上就可以看到產生出來的 Interface。
[例子](https://etherscan.io/address/0xb3da8d6da3ede239ccbf576ca0eaa74d86f0e9d3#code)

![圖片](https://user-images.githubusercontent.com/52526645/210587442-e7853d8b-0613-426e-8a27-d70c80e2a42d.png)
![圖片](https://user-images.githubusercontent.com/52526645/210587682-5fb07a01-2b21-41fa-9ed5-e7f45baa0b3e.png)


ETH Calldata Decoder: 有時候想要解看看原始 Data 可以試試看 ETH Calldata Decoder，在前面介紹到 Sam 的工具就有支援 Raw data Decode。 

![圖片](https://user-images.githubusercontent.com/52526645/210585761-efd8b6f1-b901-485f-ae66-efaf9c84869c.png)

Get ABI for unverified contracts: 如果遇到未開源的合約，可以透過這個工具嘗試列舉出這個合約中存在的 Function Signature.
[例子](https://abi.w1nt3r.xyz/mainnet/0xaE9C73fd0Fd237c1c6f66FE009d24ce969e98704)

![圖片](https://user-images.githubusercontent.com/52526645/210588945-701b0e22-7390-4539-9d2f-e13479b52824.png)

### Decompile tools
[Etherscan-decompile bytecode](https://etherscan.io/address/0xaE9C73fd0Fd237c1c6f66FE009d24ce969e98704#code) | [Dedaub](https://library.dedaub.com/decompile) | [heimdall-rs](https://github.com/Jon-Becker/heimdall-rs)

Etherscan 內建有一個反編譯功能但可讀性偏差，個人比較常使用Dedaub，可讀性好一點，也是常常最多人DM 我問我都使用哪個工具反編譯。
可以看看這個MEV Bot [實例](https://twitter.com/1nf0s3cpt/status/1577594615104172033)
可以試試看解 [例子](https://bscscan.com/address/0x64dd59d6c7f09dc05b472ce5cb961b6e10106e1d#code)

![圖片](https://user-images.githubusercontent.com/52526645/210591478-6fa928f3-455d-42b5-a1ac-6694f97386c2.png)

第一課分享就先到這邊，想學更多可以參考以下影片。
---
## 學習資源
[samczsun's eth txn explorer and vscode extension](https://www.youtube.com/watch?v=HXgu239mPBc)

[Vulnerabilities in DeFi by Daniel V.F.](https://www.youtube.com/watch?v=9fcOffCg2ig)

[Tenderly.co - Debug Transaction](https://www.youtube.com/watch?v=90GN9Ut8LhU)

https://web3sec.xrex.io/
