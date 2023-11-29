---
title: "Распространенные уязвимости в системах безопасности блокчейн-мостов"
description: "Common vulnerabilities in blockchain bridge security systems include weak on-chain validation and improper configuration, posing security risks and potential exploitation by malicious actors for attacks and fund withdrawals. Insufficient validation during on-chain processes and configuration errors can create opportunities for breaches and asset theft from the bridges."
level: "advanced"
coverImage: "/assets/blog/common-vulnerabilities-in-blockchain-bridge-security-systems/cover.png"
date: "2023-11-29T05:35:07.322Z"
time: 4
ogImage:
  url: "/assets/blog/common-vulnerabilities-in-blockchain-bridge-security-systems/cover.png"
tags:
  - blockchain
  - technology
  - security
---


## Introduction
A blockchain bridge serves as a protocol linking two distinct blockchains, facilitating their interaction. For example, if you possess bitcoins but aim to participate in DeFi operations within the Ethereum network, you can transfer your assets across the bridge instead of selling them.

These protocols are pivotal in establishing compatibility across the blockchain landscape. They operate by conducting various validations both on-chain and off-chain, which may pose certain security risks.

## The Importance of Blockchain Bridge Security
Blockchain bridges typically hold tokens that users move between different blockchains. As the use of cross-chain transfers grows, these bridges, often represented as smart contracts, accumulate significant volumes of tokens, making them an appealing target for hacking attacks.

Blockchain bridges themselves contain numerous vulnerabilities, given they are composed of various components. Bad actors might aim to attack these cross-chain applications to steal funds due to the substantial amount of assets stored within them.

According to CertiK estimates, in 2022, over $1.3 billion was lost due to attacks on blockchain bridges, accounting for 36% of the total losses for the year.

## Common Vulnerabilities in Bridge Security Systems
To ensure the reliability of bridges, it's essential to examine typical weak points and conduct thorough testing before their implementation. There are four main categories of vulnerabilities that most frequently pose risks to bridges.

### Weak On-Chain Validation
Transaction validation in regular blockchain bridges, especially those tied to specific DApps, is limited. In these bridges, core operations like mining and token transfers occur on centralized servers, while the checks are performed off-chain.

Other types of bridges use smart contracts to confirm messages and perform on-chain validation. When depositing funds onto a chain, the smart contract generates a signed message and appends it to the transaction. This acts as proof of deposit and verifies withdrawal requests. This process aims to protect the system from attacks like data replay and deposit information forgery.

However, even a minor vulnerability in the on-chain validation process can lead to serious attacks. For instance, if a Merkle tree is used to confirm transactions, a hacker might falsify these proofs, enabling them to create new tokens and send them to their account.

Some bridges utilize wrapped tokens: if a transaction fails verification, a malicious actor could direct wrapped tokens from the bridge to their address. This occurs due to the victim's approval requirement for fund transfers via the bridge contract and their withdrawal.

Moreover, many bridges require constant token approval from DApp users to save on fees. This raises risks as smart contracts gain access to a large number of tokens in the user's wallet, which could be exploited by attackers to steal assets.

### Weak Off-Chain Validation
Certain blockchain bridge systems conduct message validation from the blockchain using an internal off-chain server. The validation of transactions with deposits is particularly crucial.

Blockchain bridges with off-chain validation operate as follows:

1. Users utilize a DApp to deposit tokens into a smart contract on the original chain.

2. The DApp sends the transaction hash with the deposit to an internal server via an API.

3. The internal server verifies the received hash multiple times. If the signature is deemed authentic, the server adds the signature to the message and returns it to the user interface through an API.

4. The DApp verifies the received signature, allowing the user to withdraw their tokens from the target chain.

The role of the internal server lies in authenticating the deposit transaction and its signature to prevent potential attacks and risks for users. However, inadequate verification of the transaction structure or the contract address that initiated the operation could lead to the possibility of a hacker attack and the theft of tokens from the target chain.

### Incorrect Configuration
Weaknesses in configuration represent a pivotal point for most blockchain bridges, encompassing tasks such as compiling token and address lists, assigning signing authorities, and other crucial configuration tasks. Precise configuration of all parameters plays a critical role as even minor errors can lead to substantial financial losses.

In the blockchain industry's history, there have been instances where improper configuration allowed hackers to successfully bypass asset transfer verifications. In one such case, just days before the incident, the project team made protocol changes related to a variable responsible for standard approved message values. This alteration caused all messages to be automatically regarded as verified, enabling malicious actors to send forged messages and circumvent the verification process.

## Enhancing Bridge Security
The four key vulnerabilities outlined earlier expose weak points in the security of blockchain bridges and their associated ecosystems. There is no one-size-fits-all solution for these issues; each vulnerability requires an individual approach.

Providing unified recommendations to address errors in the verification process is quite challenging as each bridge has unique requirements. However, the primary advice is to conduct thorough vulnerability testing on bridges and ensure the reliability of the verification process.

Ultimately, special attention must be paid to meticulous threat assessments and a focus on the most common vulnerabilities in the security systems of blockchain bridges.

## Conclusion
Cross-chain bridges serve as significant repositories of assets, making them an attractive target for hackers and malicious actors. To safeguard against potential attacks, developers must rigorously assess the security of their bridges prior to deployment and engage external audit firms to ensure protection against possible breaches and threats. Bridges play a pivotal role in the blockchain space, and ensuring their security should be a paramount priority at all stages of development and in the creation of Web3 infrastructure.
