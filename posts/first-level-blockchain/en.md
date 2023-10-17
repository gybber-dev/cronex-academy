---
title: "What is a first-level blockchain?"
description: "The first level of blockchain networks encompasses major blockchains like Bitcoin, BNB, and Ethereum, capable of processing transactions within their own networks. To address scalability challenges, second-layer protocols, such as the Lightning Network, have been developed to provide instant transactions without burdening first-level blockchains."
level: "beginner"
coverImage: "/assets/blog/first-level-blockchain/cover.png"
date: "2023-08-31T05:35:07.322Z"
time: 8
ogImage:
  url: "/assets/blog/first-level-blockchain/cover.png"
tags:
  - blockchain
---

## Introduction

The first level of blockchain networks encompasses the major networks such as Bitcoin, BNB, and Ethereum, along with their foundational infrastructure. These blockchains are capable of conducting and confirming transactions without the need to rely on other networks. However, as Bitcoin continued to evolve, it became clear that enhancing the scalability of first-level networks posed a complex challenge.

In response to this issue, developers devised second-layer protocols that are constructed on top of the underlying blockchains and rely on their security and consensus mechanisms. An example of such a second-layer protocol is the Lightning Network. It enables users to perform transactions within the network without the necessity of recording every transaction on the public blockchain.

The Lightning Network provides the ability for fast and instantaneous transactions among network participants, which helps reduce the load on the primary blockchain and enhances its scalability. Thus, second-layer protocols complement first-level blockchains by addressing scalability issues and improving the user experience.
<!-- banner_place -->

The terms "first level" and "second level" are crucial for understanding the architecture of different blockchains, projects, and developer tools. They help explain the connections between various blockchains and their supplementary layers.

Studying the different levels of blockchain allows us to comprehend how projects like Polygon and Ethereum interact with each other, or how the Polkadot blockchain operates in conjunction with its parachains. These terms serve as a key guide when exploring the intricate relationships and integrations among various blockchains and their associated solutions.
## What is the first level
The first-level networks represent the primary blockchains, such as BNB Smart Chain (BNB), Ethereum (ETH), Bitcoin (BTC), and Solana, which play a central role in their respective ecosystems. They are considered first-level blockchains because they process and finalize transactions within their own networks. Additionally, each of these blockchains has its native token used to pay fees for transactions and other operations within the network.

In addition to first-level networks, there are also off-chain solutions that represent second-level blockchains built on top of the primary blockchains. These second-layer protocols provide additional capabilities and enhance the scalability and functionality of first-level blockchains, extending their capabilities.

## First level scaling
The scalability issue is common for first-level networks like Bitcoin, which face limitations in processing a large volume of transactions. This is due to the use of the Proof of Work (PoW) consensus mechanism, which requires significant computational resources. While ensuring decentralization and security, PoW often slows down network performance during high loads, resulting in increased transaction confirmation times and fees.

Developers are actively seeking solutions to increase the scalability of first-level networks. Options include increasing block sizes to handle more transactions, changing the consensus mechanism (as in the case of the upcoming Ethereum 2.0 upgrade), and implementing sharding, which involves splitting the database.

However, implementing improvements for the first level faces challenges, as not all network participants agree on these changes. This can lead to disagreements and network forks (hard forks), as was the case with Bitcoin and Bitcoin Cash in 2017. Finding a unified solution that satisfies all parties remains a challenging task for blockchain developers.
### SegWit
One successful example of a scalability solution for first-level networks is the Segregated Witness (SegWit) protocol upgrade for Bitcoin. SegWit increased the network's throughput by optimizing the organization of data within blocks. It achieved this by removing digital signatures from transaction inputs, thus freeing up additional space in blocks for more transactions.

The SegWit upgrade was implemented through a backward-compatible soft fork. This means that even Bitcoin network participants who hadn't updated their nodes could still continue processing transactions, and their devices weren't disconnected from the network. Thus, SegWit improved Bitcoin's scalability without compromising security and while ensuring compatibility with existing network participants.
## What Is First-Level Sharding?
First-level networks refer to the primary blockchains like BNB Smart Chain (BNB), Ethereum (ETH), Bitcoin (BTC), and Solana that play a central role in their respective ecosystems. They are considered primary blockchains because they process and finalize transactions within their own networks. Additionally, each of these blockchains has its native token used for transaction fees and other operations within the network.

In addition to first-level networks, there are also off-chain solutions that represent second-level blockchains built on top of the primary blockchains. These second-level protocols provide additional capabilities and enhance the scalability and functionality of first-level blockchains, extending their capabilities.
## First Level and Second Level

The first level of blockchain has its own technological limitations that are not always easily overcome within the main network. For example, in the case of Ethereum, transitioning to the Proof of Stake (PoS) consensus mechanism was challenging and took many years of development.

Certain use cases for blockchain are also constrained due to first-level scalability issues. For instance, fast gaming on the blockchain requires high transaction throughput, and Bitcoin, with its extended transaction confirmation times, is not an optimal choice. However, leveraging the security and decentralization of the first level for gaming applications is still possible. To achieve this, one can build a second-level solution on top of the base network.

Creating a second-level solution allows overcoming the limitations of the first level and developing a more efficient and faster solution for a specific use case, such as gaming applications. Meanwhile, the security and decentralization of the first level remain intact, providing users with a more convenient and speedy blockchain experience.
### Lightning Network
The Lightning Network is a second-level solution built on top of the Bitcoin blockchain. It is designed to facilitate fast transactions outside the main network, reducing the load on the main network and speeding up transaction processing.

In the Bitcoin main network, during periods of high demand, transaction processing can take several hours due to the limited blockchain throughput. However, with the Lightning Network, users can make quick payments by only settling the final balance on the main network. This is achieved by consolidating multiple transactions into one final record, saving time and resources.
## Examples of first-level blockchains
Let's take a look at several examples of first-layer blockchains that represent diverse and unique solutions for decentralization, security, and scalability. These examples showcase the diversity of blockchain technologies, and they go beyond just Bitcoin and Ethereum. Each of these networks has its own characteristics and use cases, making them interesting and significant for various applications.
### Elrond
Elrond stands out as a first-layer blockchain network, founded in 2018, that distinguishes itself by harnessing sharding to amplify its performance and scalability. Through the innovative use of sharding, the Elrond blockchain demonstrates an impressive capacity to process an exceedingly high number of transactions per second, surpassing the 100,000 TPS mark. Elrond boasts distinctive features, including the implementation of the Secure Proof of Stake (SPoS) consensus protocol and the deployment of cutting-edge Adaptive State Sharding technology.

One of Elrond's most unique aspects is its Adaptive State Sharding capability, which grants the network the dynamic ability to partition and amalgamate shards in response to fluctuations in user activity. This sharding mechanism isn't confined to transaction processing but extends comprehensively across the entire network architecture, encompassing state storage and data management. This adaptability empowers Elrond to efficiently reassign validators among shards, effectively preventing potential misuse or centralization issues.

At the core of the Elrond ecosystem lies the EGLD token, serving as its native cryptocurrency. This token holds a multifaceted role, ranging from covering transaction fees and facilitating the deployment of decentralized applications (DApps) to incentivizing network validators. It's worth highlighting that Elrond has gone above and beyond by achieving Carbon Negative certification, an exceptional accomplishment. This status underscores the network's commitment to offsetting carbon dioxide emissions associated with its energy-efficient Proof of Stake (PoS) mechanism, making it an environmentally responsible blockchain platform.
### Harmony
Harmony is a first-layer blockchain that employs the Effective Proof of Stake (EPoS) consensus mechanism and integrates sharding technology. Its mainnet comprises four shards, each operating concurrently to generate and validate new blocks. Notably, each shard has its distinct block height, facilitating various transaction processing speeds.

In a bid to attract developers and users, Harmony embraces a cross-chain financial model. Robust bridges to Ethereum (ETH) and Bitcoin play a pivotal role in enabling token swaps across chains without the risks typically associated with such bridges. Harmony also has ambitious plans to expand the Web3 ecosystem through decentralized autonomous organizations (DAOs) and zero-knowledge proofs.

Harmony is gaining increasing popularity among users, as it becomes evident that the future of decentralized finance (DeFi) hinges on multi-chain and cross-chain capabilities. The network places a strong emphasis on developing NFT infrastructure, DAO tools, and interprotocol bridges.

The native token of Harmony, known as ONE, serves as the means to pay for transaction fees. It can also be staked for participation in the consensus mechanism and network governance. Validators on the Harmony network are rewarded for block creation and for collecting transaction fees based on their actions.
### Celo
Celo is a first-layer blockchain that emerged as a fork of Go Ethereum (Geth) in 2017, but with significant modifications, including the implementation of the Proof of Stake (PoS) mechanism and a unique addressing system. The Celo Web3 ecosystem offers diverse solutions, including DeFi, NFTs, and payment services, with more than a hundred million confirmed transactions. What sets Celo apart is that users can use their phone numbers or email addresses as public keys. The Celo blockchain can be easily run on standard computers without the need for specialized hardware.

The CELO token is a utility token used for transaction fees, network security, and rewards. In the Celo network, stablecoins such as cUSD, cEUR, and cREAL exist, generated by users of the blockchain itself. These stablecoins have a support mechanism similar to the one used by MakerDAO's DAI stablecoin. Interestingly, transactions using Celo stablecoins can be paid with other Celo assets.

Celo has developed a user-friendly addressing system and the use of stablecoins to increase network accessibility for new users who may be concerned about cryptocurrency market volatility.
### THORChain
THORChain is a public decentralized cross-chain exchange (DEX) built on a first-layer blockchain network using the Cosmos SDK. It utilizes the Tendermint consensus mechanism to verify transactions. THORChain's primary goal is to provide decentralized cross-chain liquidity without the need for pegging or wrapping assets. This makes the network attractive to cross-chain investors, as it eliminates the additional risk associated with pegging and wrapping coins.

THORChain functions as a custodian that controls the deposit and withdrawal of funds. This contributes to the creation of decentralized liquidity and eliminates the need for centralized intermediaries. The native token of THORChain, RUNE, is used for transaction fees, governance, security, and verification.

THORChain's automated market maker (AMM) model uses RUNE as the base pair, allowing users to exchange tokens for any other supported asset. This is similar to a cross-chain version of Uniswap, where RUNE serves as the settlement and security asset for liquidity pools.
### Kava
Kava is a first-layer blockchain that combines the speed and compatibility of Cosmos with support for Ethereum developers. The Kava network includes separate blockchains for the EVM development environment and the Cosmos SDK. Thanks to the support of IBC in the Cosmos blockchain, developers can deploy decentralized applications and ensure their seamless interaction between the Cosmos and Ethereum ecosystems.

Kava uses the Tendermint PoS consensus mechanism, which provides powerful scalability for applications in the EVM blockchain. The Kava Network, supported by KavaDAO, offers open on-chain developer rewards designed to reward the best projects in each ecosystem based on their usage.

Within the Kava network, there is the native token KAVA, which serves as a utility token and governance token, as well as the stablecoin USDX, pegged to the US dollar. KAVA is used for transaction fees and staking assets to achieve consensus in the network. Users can delegate their KAVA to validators added to staking to receive a share of the KAVA emission. Stakers and validators also have voting rights on governance proposals that determine network parameters.
### IoTeX
IoTeX, established in 2017, is a first-tier blockchain that distinguishes itself by its strong integration of blockchain technology with the Internet of Things (IoT). Its core principle revolves around granting users complete control over the data generated by their IoT devices and the ability to utilize secure decentralized applications (DApps), assets, and services. IoTeX's approach sets it apart from conventional blockchain platforms.

IoTeX's uniqueness lies in its innovative combination of hardware and software components. This fusion enables the development of pioneering solutions for efficient data management, with a strong focus on user privacy. Notably, IoTeX has introduced MachineFi, a groundbreaking system that allows users to derive digital assets from real-world data, emphasizing its distinctiveness in the blockchain landscape.

Additionally, IoTeX offers two notable hardware products, Ucam and Pebble Tracker. Ucam, an advanced home security camera, not only provides security features but also ensures privacy during surveillance, setting it apart from competitors. Pebble Tracker, an intelligent GPS tracker with 4G support, offers real-time tracking capabilities and monitors environmental data such as temperature, humidity, and air quality. These hardware innovations showcase IoTeX's commitment to practical IoT applications and stand as unique offerings.

IoTeX further differentiates itself by providing several second-layer protocols built atop its blockchain. These protocols empower developers to create custom networks that leverage IoT technology, facilitating efficient data sharing through the IoTeX blockchain. IoTeX's flexible architecture allows developers to easily establish new subchains tailored to specific IoT device requirements, showcasing its adaptability.

The native tokens of IoTeX, known as IOTX, serve diverse purposes, including covering transaction fees, participating in staking for network security, contributing to network governance, and validating transactions. IoTeX's multi-faceted approach to blockchain, IoT integration, and privacy-focused solutions positions it as a standout player in the blockchain domain, offering unique features and applications that cater to the needs of an IoT-driven future.

**In conclusion**, the modern blockchain ecosystem comprises various first-tier networks and second-tier protocols. At first glance, these networks and protocols may appear intricate, but with deeper exploration and understanding of their core principles, the blockchain structure becomes clearer. This knowledge proves particularly valuable when delving into new blockchain projects, especially those related to network interoperability and cross-chain solutions.