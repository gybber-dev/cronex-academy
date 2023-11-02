---
title: "What is Solana (SOL)?"
description: "Solana is a blockchain network designed to provide fast transactions and high throughput to facilitate the widespread adoption of cryptocurrencies and blockchain technology. It employs innovative solutions to increase speed, including Proof of History (PoH) and parallel transaction processing. Users can utilize SOL, the native token of Solana, to pay for transaction fees and interact with smart contracts."
level: "intermediate"
coverImage: "/assets/blog/what-is-solana/cover.png"
date: "2023-11-02T05:35:07.322Z"
time: 7
ogImage:
  url: "/assets/blog/what-is-solana/cover.png"
tags:
  - altcoin
 
---


## Introduction
Limited scalability is a significant issue confronting blockchain technologies. This means that as these networks gain popularity and usage, they often encounter constraints in transaction processing speed and confirmation. Solana's primary objective is to overcome these limitations while upholding a high degree of security and decentralization.

Solana, a blockchain founded by Anatoliy Yakovenko from Solana Labs in 2017, introduces a fresh approach to transaction verification. Well-known challenges faced by prominent projects like Bitcoin and Ethereum encompass sluggish transaction processing, high transaction fees, and substantial energy consumption. In order to tackle these issues, Solana implements innovative techniques, such as Proof of History (PoH) and parallel transaction processing, facilitating the handling of thousands of transactions per second (TPS).

## How Solana Operates
Solana is a third-generation blockchain that utilizes the Proof of Stake (PoS) consensus algorithm. To achieve high throughput, fast transactions, and low fees, Solana implements a range of innovative solutions:

- Proof of History (PoH) is a method of time verification that bypasses the need for conventional timestamps.

- Parallel transaction processing allows for the concurrent handling of multiple transactions.

- Tower BFT (Byzantine Fault Tolerance) is an optimized version of practical BFT designed to work with PoH.

- Turbine is a protocol for block propagation.

- Gulf Stream is a protocol for transaction forwarding without using a mempool.

- Sealevel enables parallel execution of smart contracts.

- Pipelining is used for optimizing block verification.

- Cloudbreak is a horizontally scalable account database.

Thanks to these innovations, the Solana network exhibits high performance, capable of generating blocks in just 400 milliseconds and processing thousands of transactions per second. In comparison, creating a block in the Bitcoin network takes around 10 minutes, and in Ethereum, it's approximately 15 seconds.

SOL token holders can participate in staking within the PoS consensus algorithm. Using a compatible cryptocurrency wallet, they can delegate their tokens to validators who process transactions in the network. If successful, validators pay a portion of the staking rewards to token holders, incentivizing them and delegates to act in the network's best interests.

## Uniqueness of Solana
The uniqueness of Solana is evident in its commitment to providing low fees, high throughput, and widespread transaction adoption through a range of innovations.

### Proof of History
One of the key aspects that makes Solana unique is its use of the Proof of History (PoH) method. In the context of cryptocurrency transactions, establishing the sequence of events is crucial. For example, in the Bitcoin network, transactions are grouped into blocks, each with a unique timestamp. This requires each node to conduct a time-consuming verification of blocks and compare information with other nodes, slowing down the block confirmation process. Solana employs an innovative approach called Proof of History (PoH) to address this issue.

In Solana, all events and transactions are hashed using the SHA256 hash function. This hash function takes input data and produces a unique result that is nearly impossible to predict. Importantly, the result of hashing one transaction is used as input data for the next, creating a sequential chain of hashes. This facilitates the creation of a clear and verifiable sequence of transactions that validators can add to a block without relying on timestamps.

The hashing process also takes a certain amount of time, allowing validators to easily determine how much time has passed since the previous transaction. By placing transactions in the chain of hashes, validators process and transmit less information in each block. Using the hashed version of the latest transaction state significantly reduces block confirmation time.

Proof of History (PoH) is not a consensus mechanism but rather a way to reduce the time required to confirm the order of transactions. This method, in combination with Proof of Stake, simplifies the selection of the next validator for a block, as nodes require less time to verify the order of transactions, ultimately speeding up the network process.

### Low commissions
Solana charges extremely low fees, with an average transaction processing cost of just $0.00025. These low fees significantly enhance the accessibility of Web3 for users because in other networks, high gas fees substantially increase the expenses associated with each transaction.

### Energy efficiency
Due to the efficient use of time and resources by Solana nodes and the absence of mining, making it distinct from Proof of Work networks, Solana has emerged as one of the most energy-efficient blockchains. The Solana Foundation, a non-profit organization, plays a vital role in funding and supporting the Solana network. It consistently carries out third-party audits to evaluate Solana's energy usage and compares these figures to those of other blockchain projects, along with their average energy consumption. The most recent report, as of September 2022, presents the following energy consumption statistics:


| Action                                                 | Consumption                                                                                                                  |
|--------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------|
| One Solana transaction                                 | 508 Дж                                                                                                                      |
| One Google search                                      | 1080 Дж |
| One transaction in Solana (not related to voting)      | 3290 Дж |
| One transaction in Ethereum (after merger)             | 144 036 Дж |
| Fully charging iPhone 13 battery                       | 44 676 Дж   |
| Mining one bitcoin                                     | 5 005 764 000 Дж  |
|Average annual energy consumption among cohabitors in the United States | 38 574 000 000 Дж | 


## What is SOL
SOL is the native utility token of the Solana network, known for its unique features. What sets SOL apart is its deflationary model, which involves the burning of tokens. SOL is primarily used for covering transaction fees and interacting with smart contracts on the Solana blockchain. SOL holders can also engage in staking and take on the role of validators within the network. Similar to Ethereum, Solana provides the capability to create smart contracts and various blockchain projects.

SOL adheres to the SPL protocol, which serves as the token standard for the Solana blockchain, much like ERC-20 in the Ethereum ecosystem. SOL token has two main functions:

1. Facilitating the payment of fees associated with transactions and operations involving smart contracts on the Solana network.

2. Enabling token staking within the Proof of Stake consensus mechanism.

These unique features make SOL a powerful and versatile asset within the Solana ecosystem.

## Solana Ecosystem
The Solana ecosystem has significantly expanded since its mainnet beta launch in 2020. By December 2022, it boasted 21,255 repositories created by developers within the Solana network on GitHub, and it had amassed a user base of eight million.

Distinguished companies have also declared their integration with Solana. Discord, for instance, enabled users to link their Solana wallets to their profiles, while ASICS harnessed the Solana Pay payment system for selling a limited collection of shoes.

Solana's rapid transaction processing and high throughput have rendered it an appealing choice for various facets of the Web3 space, encompassing the following domains:

NFTs (Non-Fungible Tokens): Solana has been nurturing its NFT ecosystem with its swift transaction processing and cost-effective fees. As of December 2022, over 150,000 users had generated more than 22.7 million NFTs on Solana. Prominent NFT projects within the Solana realm include Degenerate Ape Academy, Okay Bears, and Solana Monkey Business. Additionally, projects affiliated with Meta, such as Facebook and Instagram, lend support to NFTs on the Solana network.

Payments: The Solana Pay protocol provides a user-friendly and easily accessible payment infrastructure, facilitating transactions that can be finalized in mere seconds. Eleven out of sixteen projects engaged in the Stripe gateway, which allows the conversion of fiat to cryptocurrencies, were constructed upon the Solana network.

Gaming: As of December 2022, Solana accommodated 15 gaming projects, with plans in motion to increase this number to 37 by March 2023.

DeFi (Decentralized Finance): Solana-based DeFi ventures accrued over $150 million in earnings throughout 2022, thanks to their swift transaction processing capabilities. Prominent projects include OpenBook, a community-managed order book, and the Jupiter Aggregator.

DAOs (Decentralized Autonomous Organizations): The introduction of novel tools spurred the rise in popularity of DAOs on the Solana network. A total of 8,489 DAO proposals were presented, with participation from 34,484 individuals in voting.

Mobile Platforms: In June, the introduction of Saga marked the first mobile phone to leverage the Solana Mobile Stack. This development established the Solana ecosystem as a frontrunner in cryptocurrency project development for mobile devices, with developers receiving the inaugural Saga phones in December 2022.

## The future of Solana
The future of Solana holds a multitude of exciting developments and enhancements. At the Breakpoint conference organized by the Solana Foundation in 2022, several projects were presented that are expected to roll out in the coming months and years:

1. Firedancer: Jump Crypto is developing new open-source software for Solana, including a second client-validator. This validator will be capable of processing transactions at a rate of 1.2 million TPS (as of November 2022 test environment figures). This means that Solana will be able to further increase its throughput.

2. Mobile Devices: Public sales of Saga phones are scheduled for 2023. In January 2023, Solana Mobile will also launch the Solana DApp Store, a DApp application store oriented towards Web3, with no transaction fees.

3. Network Upgrades: Various solutions have been implemented to enhance the network's performance, including the QUIC protocol, Quality of Service (QoS) based on the total staked amount, and commission markets. Solana Labs co-founder Anatoly Yakovenko has also presented his vision for network improvements.

These innovations and developments will enable Solana to continue its growth and strengthen its position in the world of blockchain technology.

## Conclusion
Solana, which entered the world of blockchain technology in 2020, is steadily progressing and evolving into a reliable and resilient ecosystem. It currently enjoys widespread popularity among blockchain projects and users, and its future holds the promise of further growth and development.


