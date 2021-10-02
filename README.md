# Tornado.Cash 介绍

**\[Work in progress\]**

![](.gitbook/assets/image.png)

Tornado Cash 是一个 **完全去中心化** **非托管** **协议** 实现了加密世界的隐私交易。

作为一个去中心化协议，Tornado.Cash 的智能合约已经永久性地部署在了以太坊区块链上。它们无法被更改或篡改。因此，没有人 - 包括最初的开发者也无法修改或者关闭它们。所有治理和挖矿智能合约都由社区通过去中心化的方式部署。

作为一个非托管协议，用户在使用 Tornado.Cash 时，始终持有他们的加密货币。每次存入，用户都会收到私钥，因此可以完全控制自己的资产。

## 如何实现隐私？

Tornado Cash 通过切断发送方和接收方地址的链上关联来改善隐私性。它使用一个智能合约来接受 ETH 和其他代币的存入，并可以使用另一个地址来支取。

为了保护隐私，还有一些额外的操作，比如，使用一个全新的地址来支取资金，并用中继器支付交易费。 

 更多信息请参阅 [Tornado.Cash 如何工作?](how-does-tornado.cash-work.md) 和 [保持匿名的诀窍](tips-to-remain-anonymous.md).

## 哪里可以找到 Tornado.Cash？

该协议最初于2019年运行在**以太坊区块链**上。最近，它又于2021年部署在了**币安智能链**和 **Polygon** 上。

如今 Tornado.Cash 可以用于以下几种代币：

* 在以太坊上 : **ETH** _\(Ethereum\)_, **DAI** _\(Dai\)_, **cDAI** _\(Compound Dai\)_, **USDC** _\(USD Coin\)_, **USDT** _\(Tether\)_ & **WBTC** _\(Wrapped Bitcoin\)_
* 在币安智能链上: **BNB** _\(Binance Coin\)_.
* 在 Polygon 网络上: **MATIC** _\(Polygon\)_

![](.gitbook/assets/non-custodial-anonymous-transactions-on-ethereum-3-.png)

该协议同时包括了一个**匿名挖矿系统**，允许用户赚取其**治理代币**。得益于 TORN 代币，Tornado Cash 用户积极地参与改进该协议。社区对于 Tornado Cash 的演进和特性的改善有着很强的影响力。协议的参数和治理代币的分发完全由社区治理控制。

更多信息请参阅 [匿名挖矿](anonymity-mining.md) 和 [Tornado.Cash 代币](torn.md)。

## Tornado.Cash 如何运行？

[Tornado.Cash 的代码](https://github.com/tornadocash)是完全**开源的**。作为一个 DAO （去中心化自治组织），Tornado.Cash 治理和挖矿的智能合约由其社区部署。

该协议同时应用了 zk-SNARK，它允许零知识证明，使用户无需透露信息内容也能证明自己拥有它。这项技术的应用基于 **Zcash 团队在以太坊社区帮助下的开源研究**。为了设置 zk-SNARK 初始密钥， Tornado.Cash[ 可信设置社区 ](https://tornado-cash.medium.com/tornado-cash-trusted-setup-ceremony-b846e1e00be1)于2020年5月启动并记录了[ 1114名贡献者 ](https://tornado-cash.medium.com/the-biggest-trusted-setup-ceremony-in-the-world-3c6ab9c8fffa)。如此庞大的贡献者数量确保了不可能通过伪造零知识证明来危害协议。

用户界面由社区托管在 **IPFS** （InterPlanetary 文件系统）上，由此将数据被删除的风险降至最低。只要还有一名用户托管它，界面就能正常工作。 

 作者:[ @ayefda ](https://torn.community/u/ayefda)
