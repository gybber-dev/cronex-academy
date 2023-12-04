---
title: "Introduction to Confidential Transactions"
description: "Confidential transactions are an innovative mechanism in cryptocurrencies, ensuring the concealment of transmitted data and participants' addresses within the network. This method contributes to elevating the level of transaction confidentiality and anonymity."
level: "advanced"
coverImage: "/assets/blog/introduction-to-confidential-transactions/cover.png"
date: "2023-12-04T05:35:07.322Z"
time: 4
ogImage:
  url: "/assets/blog/introduction-to-confidential-transactions/cover.png"
tags:
  - cryptocurrency
  - security
  - technology
---

## Introduction
The efficient functioning of a blockchain heavily relies on the transparency of the system. Each node within the network can store a copy of the blockchain and verify its compliance with the rules. In various decentralized ledgers, users have the ability to access online block explorers to seek information regarding blocks, transactions, and addresses.

However, the confidentiality of this structure is far from perfect. In systems like Bitcoin, every transaction is linked to its predecessor. It's crucial to note that coins are technically not interchangeable, as each one can be traced back to specific transactions. While it's impossible to prevent the sending of bitcoins, the network might refuse to process a transaction if it detects that the used address was previously blacklisted.

In the worst-case scenario, the lack of interchangeability can significantly impact the fundamentals of the entire system. New coins might hold greater value, while older ones, considering their history, could be less appealing for use.

The confidentiality of Bitcoin is often overstated. Not only coins but also users are traceable. The cryptocurrency's mechanism involves the use of pseudonyms (public addresses instead of names), yet this approach isn't without its flaws. Sophisticated analysis methods can accurately link addresses, creating clusters in an attempt to de-anonymize network participants.

One of the proposed enhancements was the implementation of confidential transactions to achieve real privacy in conducting operations.

## What are confidential transactions?
Confidential Transactions (CT) is a concept first proposed by Blockstream's CEO, Adam Back, in 2013, later augmented by ideas from Bitcoin developer Gregory Maxwell. The essence of these transactions lies in concealing the information regarding the transferred amount from all participants in the network except the two parties directly involved in the transaction.

<img src="/assets/blog/introduction-to-confidential-transactions/confidential-transaction.png" alt="Confidential transactions" />
Confidential transactions

Under normal conditions, when transactions are visible to everyone, nodes can easily verify that the amount received by one party does not exceed the sent amount. For instance, if Louise intends to send 0.3 BTC to John, she takes an unspent output (e.g., 1 BTC), sends 0.3 BTC to John, and retains the remaining 0.69 BTC for herself (factoring in the mining fee).

However, with confidential transactions, where the amount is not viewable by other network participants, verification becomes more complex. How does one ensure that an unknown number equals or exceeds the sum of other unknown numbers? This challenge remains intricate in the context of confidential transactions, necessitating specialized encryption methods and mathematical techniques to facilitate verification without revealing specific amounts.

## Overview of the Utilized Cryptography

To ensure data confidentiality, encryption plays a vital role. However, traditional methods are akin to storing information in a safe: the data becomes inaccessible until retrieved. For implementing confidential transactions, a digital safe is necessary, housing concealed content while allowing its properties to be verified by external entities.

Homomorphic encryption, also known as Pedersen commitment, plays a pivotal role in this concept. This encryption type enables third parties to operate on encrypted data without disclosing its content, presenting numerous practical applications.

A conventional hash can be utilized to lock data that you wish to reveal later. For instance, if you organize a social media contest where participants must guess your preferred exchange to win a prize of 0.01 BTC, you could provide a hashed string pointing to a specific input, concealing the actual value. This aids participants in verifying the authenticity of their answer after the results are announced.

However, this approach doesn’t assure absolute reliability. Participants can iterate through possible options, hashing various inputs in search of matches. To mitigate the likelihood of such attacks, a blinding factor—random data—is added to the information before hashing.

Pedersen commitment allows merging data while maintaining confidentiality. This method is used in transaction processes, where commitments are created before fund transfer, verified to confirm data correctness upon reception.

<img src="/assets/blog/introduction-to-confidential-transactions/formula.png" alt="C(BF1 + D1) + C(BF2 + D2) = C(BF1 + BF2, D1 + D2) where BF — blinding factor, аnd D — data" />
where BF — blinding factor, and D — data

Despite involving several steps and utilizing elliptic curve cryptography, the core idea remains: during transactions, commitments are aggregated and verified to ensure input-output data consistency, facilitating transaction verification without revealing specific amounts.

## What Can Confidential Transactions Achieve?

Confidential transactions offer a mechanism to conceal input and output data within a transaction, ensuring a higher level of privacy within the blockchain system. If such functionality were integrated into the Bitcoin protocol, it would significantly enhance privacy levels. Input and output data would become inaccessible for general scrutiny, and blockchain records would be obfuscated, while still allowing nodes to verify transaction authenticity. This heightened level of confidentiality would enable bitcoins to become more interchangeable, as the history of each coin unit wouldn't be revealed through blockchain analysis.

However, the integration of confidential transactions into the Bitcoin protocol currently appears unlikely. Additional functionality would increase transaction sizes, resulting in greater network load considering the limited block space. Furthermore, it would necessitate the consensus of a majority of participants to make changes to the protocol's code, which is a complex and challenging task.

Such changes might be subject to discussion and consideration in the future, but at present, implementing confidential transactions in Bitcoin seems improbable due to technical and structural constraints, as well as the requirement for broad support from the community and network participants.

## Summary
Confidential transactions, integrated into other cryptocurrencies and Bitcoin sidechains, serve to ensure a high level of privacy and confidentiality. For instance, Monero combines confidential transactions with ring signatures to achieve coin anonymity and fungibility. The technology of confidential transactions is also employed in sidechains like Liquid and MimbleWimble to enhance confidentiality.

While confidential transactions offer various advantages, including heightened privacy, their implementation comes with technical complexities. Scalability and throughput issues in the cryptocurrency realm pose significant limitations. Large transaction volumes associated with confidential mechanisms could strain the network and lead to scalability challenges.

Nevertheless, proponents of privacy in cryptocurrencies argue that concealing transaction amounts and participant addresses is crucial for ensuring coin fungibility. They believe it's necessary for a cryptocurrency to function as money, possessing fungibility properties and providing a high level of privacy for users.
