---
title: '区块链培训小结'
date: '2017-10-09'
categories:
  - 培训
tags:
  - 培训
---

# 区块链的由来

区块链思想最早出现在大名鼎鼎的**比特币开源项目**中，比特币项目的诞生和发展过程，借鉴了来自数字货币，密码学，博弈论，分布式系统，控制论等多个领域的技术成果，可谓博采众家之长于一身。 以前只有比特币和比特币技术一说，后来由于大家对比特币价格波动原因，所以(2014年)将比特币底层技术称之为**区块链**。

# 区块链是什么

- 狭义地说，区块链就是**比特币的底层技术**；比特币则是区块链最大、最成功的应用。
- 从技术上看，区块链是由许多对等节点组成，通过共识算法保证区块数据和交易数据的一致性，从而形成一个统一的**分布式账本**。
- 从价值层面上看，区块链是记录价值、传递消息和**价值本身转移**的一个可信账本。

# 区块链的组成部分

**block** + **chain** = **blockchain**

区块链可以通俗地看做是将块以链式结构形成的。那么具体的内部结构分如下三个结构：

- 交易(**transaction**): 一次对账本的操作，导致账本状态的一次改变，如添加一条转账记录
- 区块(**block**): 记录一段时间内发生的所有交易和状态结果，是对当前账本状态的一次共识
- 链(**chain**): 由区块按照发生顺序串联而成，是整个账本状态变化的日志记录

![区块链组成结构](/images/区块链组成结构.png)


## 比特币地址生成过程

![](/images/bitcoinAddress.png)

```
Private key:  40073635e80aaad35d9481d49388fc6fb1f55a260c9eba36e03c62b123eb7dac

Public key:  04e6644feb28ca531c7a65035a9c0adc05eeec0c68fbae723bc97131942d9150d319fddf610eacfc208adcc8320046f0bc66e66396b343daf4a18b657e16fb5d92

Wif:  5JJV6UWWFEGd8r8HV5L5y2rkaYMJy5JUSc5ULQ6ocx1M41dhy2c

Address:  1E5WwpwWdUBXXiqDX9xb2HjWybCUX96cCR

Signed:	483045022100bf6a53f9524fac95b26a1fa9af423f1c5a1a6cf9a80e0b8c961c212f741189d802203fa8ff9606ed2c277a5a8f137535c3dcd4163f9a53ce3bac922724cc917b712201 4104e6644feb28ca531c7a65035a9c0adc05eeec0c68fbae723bc97131942d9150d319fddf610eacfc208adcc8320046f0bc66e66396b343daf4a18b657e16fb5d92
```

## 交易


![Bitcoin_tx_example](/images/Bitcoin_tx_example.png)


## UTXO理解

比特币的UTXO是中本聪一个很了不起的发明。UTXO 代表 Unspent Transaction Output， 表示未花费的输出。

在比特币里面没有帐户，也没有余额的概念，仅有被所有者锁住的一个一个UTXO.

## 比特币脚本系统

比特币脚本系统是一个图灵非完备的简单系统。但是正是这个简单系统完成了比特币的价值转移。

![scriptSig1](/images/scriptSig1.png)
