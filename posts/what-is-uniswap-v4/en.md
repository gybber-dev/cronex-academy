---
title: "What is Uniswap V4?"
description: "Uniswap V4, последняя версия децентрализованной биржи (DEX), предлагает расширенные функции, такие как настраиваемые пулы ликвидности через хуки, повышая эффективность торговли. Однако, при использовании этой платформы, пользователи могут столкнуться с сложностью и потенциальными комиссиями за газ, связанными с ее открытой и гибкой архитектурой."
level: "advanced"
coverImage: "/assets/blog/what-is-uniswap-v4/cover.png"
date: "2023-10-19T05:35:07.322Z"
time: 4
ogImage:
  url: "/assets/what-is-uniswap-v4/t/cover.png"
tags:
  - altcoin
---


## Introduction
In June 2023, the Uniswap platform released a draft version of Uniswap V4's code, outlining new features in the decentralized exchange (DEX) protocol.

Among the new features are hooks that provide enhanced liquidity pool customization and the Singleton technology, which improves cross-pool liquidity efficiency. Additionally, native ETH token trading pairs will be reintroduced into the protocol.

Uniswap V4 is expected to offer a range of advantages, including extended customization, increased efficiency, reduced gas fees, and advanced trading strategies.

Among the potential drawbacks of Uniswap V4 are withdrawal fees and licensing restrictions that limit the use of Uniswap's source code.

## What Is Uniswap?
Uniswap stands as a decentralized exchange (DEX) built on the Ethereum blockchain. It facilitates the exchange of various digital assets using an Automated Market Maker (AMM) model, which eliminates the need for a traditional order book.

The platform's origins trace back to 2018 when Ethereum developer Hayden Adams created Uniswap. The inspiration for this innovation came from Vitalik Buterin, a co-founder of Ethereum, who introduced the concept of implementing an AMM on the blockchain.

As time progressed, Uniswap established itself as a frontrunner in the DEX market, boasting superior trading volumes and more robust liquidity compared to other DEX platforms. In 2023, it retains its leading position in terms of trading volume, liquidity, and active user base.

Uniswap has undergone multiple iterations. In 2020, Uniswap V2 was unveiled, followed by Uniswap V3 in 2021. June 2023 marked the release of a preliminary version of the Uniswap V4 code, introducing substantial enhancements to the platform. Understanding these changes is essential for staying current with the platform's development, while also considering the features of earlier Uniswap iterations.

<!-- banner_place -->

## Features of Uniswap V1:
Uniswap V1, the first version of the platform, was introduced in November 2018 as a pilot project to test its concept. Its primary innovation was the Constant Product Market Maker (CPMM) model.

Uniswap V1 departed from the traditional order book system and instead allowed token holders to provide their tokens to liquidity pools for trading pairs (e.g., ETH/DAI) in exchange for a share of the fees collected from users of these pools.

Uniswap V1 enabled the exchange of ERC-20 tokens among themselves and with Ether (ETH). The token swap process involved two steps:

Swapping the first token (ERC-20) for Ether (ETH).

Swapping Ether (ETH) for the second token (ERC-20).

These two steps were necessary because Uniswap V1 smart contracts supported only direct liquidity pools between ERC-20 tokens and Ether (ETH).

Despite being a revolutionary step, Uniswap V1 had its drawbacks. Its pricing algorithms were not entirely efficient and could be exploited for arbitrage, and significant slippage occurred in large transactions.

## Features of Uniswap V2:
To address the shortcomings of Uniswap V1, Uniswap V2 was developed and released in May 2020, introducing several significant improvements. Uniswap V2 implemented direct token swaps, reducing slippage and improving capital efficiency.

Additionally, Uniswap V2 introduced the functionality of flash swaps. This feature allowed users to withdraw funds from liquidity pools and use them at their discretion. However, they were required to return the withdrawn amount (with a fee) within the same transaction. This mechanism created new opportunities for arbitrage and revenue generation without the need for initial capital investments.

Uniswap V2 also introduced the concept of Time-Weighted Average Prices (TWAP), enabling other decentralized applications to safely and freely utilize price data from Uniswap.

## Features of Uniswap V3:
Uniswap V3 was launched in May 2021 with the aim of addressing challenges related to efficient capital utilization and liquidity concentration, which were relevant issues in the DeFi space at the time. This version introduced innovative features such as concentrated liquidity and multiple fee tiers to provide users with greater control and flexibility in managing their assets within liquidity pools.

The introduction of Non-Fungible Liquidity (NFL) in Uniswap V3 was especially relevant, as it allowed liquidity providers to obtain NFTs representing their share in liquidity pools, providing a new way to interact with DeFi assets.

Additionally, the integration with Optimism, a second-layer scaling solution on Ethereum, was seen as a vital step in mitigating high gas fees, making Uniswap V3 more accessible and cost-effective for users, which was a pressing concern for the DeFi community.

Please note that the DeFi landscape is continuously evolving, and there may have been further developments and improvements in Uniswap and the broader DeFi ecosystem beyond September 2021.

## Advantages of Uniswap V4

Uniswap V4 offers several significant advantages, including:

1. Enhanced Customization: The introduction of hooks provides developers with greater flexibility to create innovative liquidity pools with customizable trading functions.

2. Improved Efficiency: The implementation of hooks, the Singleton contract, and flash accounting makes transaction routing more efficient, resulting in faster and more cost-effective operations.

3. Gas Fee Reduction: The new features in Uniswap V4 offer the potential for further gas fee reductions, making the protocol more accessible to users.

4. Increased Income for Liquidity Providers: Dynamic fee structures enable liquidity providers to have more active control over their pools and the potential to increase their earnings.

5. Advanced Trading Strategies: New features like time-weighted average price (TWAP) market making, limit orders, and dynamic fees provide experienced traders with tools to execute advanced trading strategies that were previously unavailable.

## Uniswap V4 has several potential drawbacks:

Fee Structure: Uniswap V4 employs two distinct fee mechanisms, including swap fees and withdrawal fees, which might increase the cost of using the protocol for users. Uniswap governance can also decide whether to levy charges on specific pools.

Licensing Restrictions: Uniswap V4 is released under the Business Source License 1.1, which imposes limitations on the commercial and production use of the source code for a specified period. This restriction could lead to criticism from parts of the community that desire more open access to the source code.

## Conclusion
The decentralized exchange (DEX) market is in a constant state of evolution, and Uniswap stands as one of the leading platforms in this space. With the release of Uniswap V4, the protocol has undergone significant changes, introducing new capabilities and improvements.

However, it's worth noting that the open and flexible architecture of Uniswap V4 may present complexities for ordinary users, requiring a deeper understanding of how liquidity pools and new hooks function. Before engaging with this platform, conducting thorough research and gaining a comprehensive understanding of its operations is essential.
