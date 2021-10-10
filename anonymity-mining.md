# 匿名挖矿

匿名挖矿是一种提升隐私性激励措施，鼓励用户将资产长时间存放在池子，存入时间越长奖励越高。

_这个激励措施开始于2020年11月18日，并于2021年12月18日结束。_

任何人将所支持的代币存入匿名池，都会在每个区块收到固定比例的奖励，这些奖励将会以 TORN 的形式被申领。

### 匿名点数（AP）

_需要注意的是，由于手续费的原因，小额存款可能无法收获理想的 AP 奖励。_

一名社区成员创建的 [挖矿表格](https://torn.community/t/anonymity-mining-spreadsheet/720) 可以通过估算申领奖励的手续费，来计算每个池子各种金额的年化收益率（APY）。**强烈介意在投入挖矿前查看此资源并做好规划。** 在表格底部，你可以通过选择不同的工作表来查看各个池子的信息。

### 如何赚取 AP

1. 通过下拉菜单选择存入资金的种类和数量，再点击 "Connect" 和 "Deposit" 。

![](.gitbook/assets/m3fh0gl.png)

2. 记录号你的存款密语，并被备份在安全的地方，**不要把这个密语泄露给任何人，不然你可能损失你的资金和奖励。**

![](.gitbook/assets/vhustru.png)

3. 生成证明并提交交易。

4. 你的存款现在应该显示在了页面底部，你可以在这里查看它赚取了多少 AP；请记住，存款时间越长，你赚取的 AP 就越多。

![](.gitbook/assets/k6juetp.png)

_有效密语（没有取出）被显示为 “unspent”。_

### 如何申领 AP

1. 首先，你必须创建一个挖矿账户，并将这些凭证保存在链上以方便找回（需要发送一笔交易），**和存款密语一样，永远不要泄露你的挖矿恢复密钥给任何人** ，并将它备份在安全的地方。这个功能不支持支持硬件钱包，请保存好相关信息。

![](.gitbook/assets/lskzkgk.png)

2. 通过密语将资金提取至你想要的地址，并决定是否使用中继器（为了保持资金的匿名性，始终建议使用中继器），这将会是密语变成 “spent” 状态。

![](.gitbook/assets/aid86cj.png)

**记得始终保存好存款密语，即使已经将资金取出，它仍可以用来兑换 AP。**

![](.gitbook/assets/bpsqxxr.png)

3. 访问挖矿页面并输入你使用过的密语，你可能会遇到以下情形。

* **密语可以申领**：点击 “Claim reward” 按钮并提交交易，一旦交易确认，你的 AP 余额将会更新。

![](.gitbook/assets/e9jyqhu.png)

 

* **密语无法申领**：_“Warning: The note is not yet ready for anonymity mining. You can wait few days before trying again”_ -这表示 Merkle 树没有同步，需要一笔交易来更新。

![](.gitbook/assets/i6qtr0f.png)

更新树是一个昂贵的过程，**建议小额存款者等待大额矿工来更新树，这可能需要几天或者一周的时间。** 如果你想要查看和你相关的待定分支，点击 _“Show mining note information”_ 链接，这里你可以点击 “Update trees” 按钮，支付交易费来更新树。

![](.gitbook/assets/d8dmxjj.png)

### 如何兑换 AP

1. 切换到挖矿页面上的 “Swap” 界面，你可以在页面上的二级导航栏找到它。

![](.gitbook/assets/ahrjxbq.png)

2. 输入想要兑换的 AP 数量，或者选择 “Maximum” 兑换所有。输入后，将会显示当前 AP/TORN 汇率和最终奖励的数量。提供想要接收奖励的地址，生成证明并提交交易。

![](.gitbook/assets/wo55lao.png)

3. 如果上面的步骤都正确完成，TORN 将会发送到第2步所提供的地址。

### 完成

恭喜你成功参与了匿名挖矿！

始终建议在参与匿名挖矿前做好规划，用户还应注意 [AP/TORN 汇率](https://duneanalytics.com/luckyallocator/Daily-AP-TORN-Rate-v2) 取决于供需，因此，**兑换的人越多，汇率越高，兑换的人越少，汇率越低。** 

更多匿名挖矿的内容，请参考以下资源：

* [Tornado.Cash governance proposal article](https://tornado-cash.medium.com/tornado-cash-governance-proposal-a55c5c7d0703)
* [Tornado.Cash anonymity mining optimisation article](https://tornado-cash.medium.com/gas-price-claimed-anonymity-mining-a-victim-but-now-everyone-can-claim-ap-5441aaa32a1a) 
* [Anonymity mining explained \(technical\)](https://torn.community/t/anonymity-mining-technical-overview/15)

_审阅_ [_@sockawoo_](https://torn.community/u/sockawoo) _和_ [_@ethdev_](https://torn.community/u/ethdev)

_作者_ [_**@xgozzy**_](https://torn.community/u/xgozzy/summary)

