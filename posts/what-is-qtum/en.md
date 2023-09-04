---
title: "What is QTUM"
level: "intermediate"
coverImage: "/assets/blog/what-is-qtum/cover.png"
date: "2023-09-01T05:35:07.322Z"
time: 6
ogImage:
  url: "/assets/blog/what-is-qtum/cover.png"
tags:
  - altcoin

---


# Introduction
From the moment Bitcoin was introduced, blockchain technology has made significant strides. Numerous top-tier platforms now incorporate innovations that extend well beyond Bitcoin's initial framework. The Qtum development team has amalgamated the advancements of Ethereum and Bitcoin to give rise to a distinctive project. This article delves into the most captivating facets of the Qtum blockchain.


# What is Qtum

Qtum (pronounced as "quantum") is a blockchain network founded in 2016 by Ashley Houston, Neil Mahi, and Patrick Dai. In 2017, it conducted an Initial Coin Offering (ICO) that raised $15.6 million for the project. Subsequently, in September of the same year, its own mainnet was launched. The core idea behind Qtum is to combine elements from the Ethereum (ETH) and Bitcoin (BTC) networks. The project's team adopted the concept of Unspent Transaction Outputs (UTXO) from the Bitcoin network and merged it with the capabilities of Ethereum's smart contracts, aiming to harness the advantages of both blockchain platforms.

# How Qtum Works

The Qtum network comprises four main components:

1. The Unspent Transaction Outputs (UTXO) model from the Bitcoin network.
2. The Solidity programming language for smart contracts.
3. The Account Abstraction Layer (AAL) technology.
4. The Proof of Stake (PoS) consensus mechanism.
5. Qtum developers adapted Bitcoin's client software to form the transaction base of the network. This blockchain is compatible with the Ethereum Virtual Machine (EVM) and uses the Solidity programming language.

This approach allows for the easy migration of code and DeFi (Decentralized Finance) projects from Ethereum to the Qtum platform. Additionally, the network is secured by a specialized Proof of Stake (PoS) consensus mechanism designed to address critical security concerns.

# What is UTXO

UTXO (Unspent Transaction Output) is a widely used concept in the world of cryptocurrencies. Transactions in cryptocurrency networks consist of input and output data. For example, to send 1 BTC, you need to use a UTXO as input, which becomes a new UTXO as the output after the transaction. Used UTXOs are marked as spent, while the new ones become available for use.

Imagine you want to send 0.6 BTC. In reality, this amount could consist of two UTXOs: 0.4 BTC and 0.2 BTC, left over from previous transactions. To send 0.3 BTC, you might need to split a 0.4 BTC UTXO into two: 0.3 BTC for the recipient and 0.1 BTC for yourself. Thus, you spend 0.4 BTC and create two new UTXOs – 0.3 BTC and 0.1 BTC.

This system may seem unconventional, but it has its advantages:

Prevention of double spending through the tracking of output data status.
Parallel processing of transactions, as each transaction has independent output data.
While Ethereum uses an account model similar to a bank account, which maintains a shared state of balances in the network.

# What is Account Abstraction Layer

Account Abstraction Layer (AAL) is a technology used in the Qtum network to address the challenge of implementing smart contracts in blockchains based on the UTXO model. In these blockchains, unlike traditional balance-based networks where smart contracts can use addresses or final balances, smart contracts with UTXO must determine which Unspent Transaction Outputs (UTXOs) to utilize. This can be complex and inconvenient, especially for internal transactions between contracts.

The Account Abstraction Layer (AAL) technology solves this issue by abstracting the Ethereum account system from its technical implementation, allowing UTXO transactions to create and execute smart contracts. AAL processes the results and adapts them for the UTXO model.

Thanks to the AAL technology, Qtum can easily adapt updates from Ethereum and Bitcoin networks. For example, when Ethereum added support for non-fungible tokens, the Qtum network could quickly integrate this update. Additionally, through AAL, Qtum can leverage technologies like Lightning Network, Segregated Witness (SegWit), and Taproot, which were significant upgrades in the Bitcoin network.


# What is Proof of Stake
Proof of Stake (PoS) stands as a distinctive consensus mechanism within blockchain networks, enabling participants to authenticate and append new blocks to the chain according to the volume of coins they possess. Unlike the conventional Proof of Work (PoW) method, where participants (miners) engage in resolving intricate mathematical problems to forge blocks and claim rewards, PoS grants the privilege of block addition and reward allocation to coin owners who "stake" their holdings.

In the realm of blockchain innovation, Mutualized Proof of Stake (MPOS) surfaces as a one-of-a-kind consensus mechanism meticulously crafted by the Qtum team. Its primary objective is to erect barriers against fraudulent spam attacks by rendering them more intricate to execute and elevating the associated costs. MPOS functions by redistributing block creation rewards among contributors, with a portion of these rewards earmarked for future use. These rewards are divided equitably between the present validator and the preceding nine validators. Additionally, a segment of the rewards is retained by the system until a specified block count is reached. These measures introduce a level of complexity that serves as a deterrent against precise calculations and orchestrations in potential fraudulent attacks.

# What is offline staking
Offline staking, introduced by the Qtum network in August 2020, represents a novel mechanism allowing QTUM holders to engage in staking without the need to lock up their coins. Instead, users merely specify their wallet address. This enables them to retain their coins in their wallet and use them as they see fit. Offline staking encompasses two distinct categories of participants: super stakers (validators) and delegates.

To initiate offline staking, a delegate sends their wallet to a super staker via a smart contract and negotiates commission terms. Once the super staker agrees, they add the delegate's UTXO to the staking pool. Upon successful block verification, the super staker distributes a portion of the rewards to delegates and collects a fee.

This approach to delegation empowers delegates to earn passive income in the form of QTUM without being bound to a smart contract. They can also leverage offline solutions such as hardware wallets. Meanwhile, super stakers earn rewards for block creation and charge fees for staking, while delegates can generate income passively, even if their wallet remains disconnected from the network.

# QTUM 
QTUM is the official cryptocurrency of the Qtum platform, distributed among network participants using a consensus mechanism. QTUM holders can use this cryptocurrency for the following purposes:

Paying transaction fees on the network. Similar to Ethereum, QTUM utilizes a gas fee model, where users pay fees for transaction processing.
Participating in the Qtum network governance protocol by voting on proposals. This allows users to influence network parameter changes, such as block size or transaction fees. During periods of high demand, the system can reduce gas costs and increase the block size to accommodate up to 1100 transactions per second for processing primary transactions. Additionally, second-layer solutions like Lightning Network can be used for further scalability if needed.
Participating in staking by depositing coins as delegates or super stakers. For every block created, delegates and super stakers receive rewards. Qtum periodically doubles rewards using a method similar to Bitcoin's halving. This strategy aims to limit the supply of QTUM, but full implementation will take decades. At this stage, stakers receive rewards primarily in the form of transaction fees.

**In conclusion,** it can be said that Qtum is an innovative blockchain designed to address issues associated with the Proof of Work (PoW) mechanism by implementing a modified version of Proof of Stake (PoS). The platform utilizes smart contracts, decentralized applications (DApps), and is based on the Unspent Transaction Output (UTXO) model. At a time when many platforms are exploring new methods to solve problems, Qtum is building its ecosystem by leveraging the existing advantages of blockchains. Considering Qtum as an alternative allows for a more thoughtful decision-making process, based on its diverse range of applications and capabilities.
