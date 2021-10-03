# Tornado.Cash 如何工作？

**\[Work in progress\]**

在开始 Tornado.Cash 教程之前，下面是关于该协议功能的概述。

### Tornado.Cash 功能概述

为了实现隐私，Tornado.Cash **使用智能合约从一个地址接收代币存入并允许通过另一个地址支取**。这些智能合约像一个池子使所有存入的资产混合在一起。

一旦资金通过一个全新的地址从这些池子里取出，发送方和接收方的链上联系就被切断了。被支取的数字资产因此实现匿名化。

当一个用户把资金放入池子（也就是存入），就会生成一个密语。这个密语像私钥一样可以使用户访问到这些资金。有了密语，用户可以使用不同的地址 - 无论新的还是旧的，来支取这些资金。

这种协议的效果取决于池子中的用户数量，用户数越多越好。当然为了提升隐私和匿名性，用户必须牢记一些基本规则：

*  存入和支取操作之间要有一定的时间间隔。
*  在取回资产前，等待几笔交易，以使池子里的资金充分混合。

_更多建议请参阅 [保持匿名的诀窍](tips-to-remain-anonymous.md)。_

### Contribution of zk-SNARK & hashing process

Tornado.Cash use Zero-Knowledge Succinct Non-Interactive Argument of Knowledge \(also called zk-SNARK\) to verify & allow transactions.

To process a deposit, Tornado.Cash generates a random area of bytes, computes it through the [Pederson Hash](https://iden3-docs.readthedocs.io/en/latest/iden3_repos/research/publications/zkproof-standards-workshop-2/pedersen-hash/pedersen.html) \(as it is friendlier with zk-SNARK\), then send the token & the 20 mimc hash to the smart contract. The contract will then insert it into the Merkle tree.

To process a withdrawal, the same area of bytes is split into two separate parts: the **secret** on one side & the **nullifier** on the other side. The nullifier is hashed. This nullifier is a public input that is sent on-chain to get checked with the smart contrat & the Merkle tree data. It avoids double spending for instance.

Thanks to zk-SNARK, it is possible to prove the 20 mimc hash of the initial commitment and of the nullifier without revealing any information. Even if the nullifier is public, privacy is sustained as there is no way to link the hashed nullifier to the initial commitment. Besides, even if the information that the transaction is present in the Merkle root, the information about the exact Merkle path, thus the location of the transaction, is still kept private.

Deposits are simple on a technological point of view, but expensive in terms of gas as they need to compute the 20 mimc hash & update the Merkle tree. At the opposite, the withdrawal process is complex, but cheaper as gas is only needed for the nullifier hash and the zero-knowledge proof.

_Written by_ [_@ayefda_](https://torn.community/u/ayefda)\_\_

