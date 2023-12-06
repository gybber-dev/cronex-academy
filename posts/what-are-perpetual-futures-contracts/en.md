---
title: "What are perpetual futures contracts?"
description: "Perpetual futures contracts are a type of derivative that lacks a specific expiration date, allowing the holder to maintain the position for as long as necessary. They utilize underlying price indices formed based on the average asset price on spot markets, distinguishing them from regular futures contracts, which have a defined expiration date."
level: "advanced"
coverImage: "/assets/blog/what-are-perpetual-futures-contracts/cover.png"
date: "2023-12-06T05:35:07.322Z"
time: 5
ogImage:
  url: "/assets/blog/what-are-perpetual-futures-contracts/cover.png"
tags:
  - trade
  - economics
  - technology
---


## What is a futures contract?

A futures contract stands as an agreement committing to the purchase or sale of an asset at a predetermined price on a future date. Unlike spot market transactions, futures contracts operate under specific terms, including price and delivery date, without immediate asset exchange.

Uniquely, the futures market offers a trading platform for contracts dictating future asset prices without necessitating instant physical asset transfer. For instance, a gold futures contract might stipulate the future price per gram of gold but doesn't involve immediate physical gold exchange.

While some futures markets may involve actual goods delivery in the future, most contracts settle in cash. This means transactions conclude in equivalent monetary value without physically exchanging the asset. Furthermore, contract pricing may differ based on execution timing, reflecting variations between futures and spot market prices.

## Why do users trade futures?
Users are drawn to trading futures for several reasons. One of the key ones is the utilization for hedging and managing financial risks. Futures provide a tool to safeguard against potential losses resulting from asset price fluctuations.

Another appealing aspect is the opportunity for short exposure. Traders can speculate on an asset's price decline even without owning it, enabling them to profit from the asset's decrease in value.

Moreover, financial leverage is a significant factor. Users can open trading positions that exceed their available funds, allowing for increased potential profit or loss as asset prices fluctuate.

<!-- banner_place -->

## What is a perpetual contract?

A perpetual contract is a unique type of futures contract characterized by the absence of a specific expiration date. This allows maintaining a position for as long as necessary. Unlike regular futures, perpetual contracts use an underlying price index based on the average price of the asset on major spot markets and their trading volume.

Therefore, unlike regular futures, perpetual contracts often trade at a price close to or equal to the price on spot markets. However, the main difference lies in their execution method and the absence of a specific contract expiration date.

## What is initial margin?

The initial margin is the minimum amount needed to initiate a leveraged position. For example, if you're buying 1000 ETH coins with an initial margin set at 100 ETH (with a leverage of x10), your margin would be 10% of the total transaction value, serving as collateral for your position.

## What is maintenance margin?
The maintenance margin is the minimum deposit required to keep your trading positions open. If your margin falls below this level, you might receive a margin call to add more funds, or your trade will be automatically closed. Most exchanges offering margin trading follow this approach.

In simpler terms, the initial margin sets the amount when opening a position, while the maintenance margin ensures the positions remain open, adjusting according to the current market asset price and account balance (the collateral).

## What is liquidation?
Liquidation is the process triggered when the value of your collateral falls below the required maintenance margin level. This results in the automatic closure of your futures trading positions. The mechanism for liquidation can vary based on the exchange and market. In such cases, a fee is charged, and if the balance doesn’t cover the liquidation amount, the user might be declared bankrupt. Additional fees are incurred during the liquidation process, and to avoid this, positions can be closed beforehand or funds can be added to the collateral balance to prevent liquidation at the current market price.

## What is funding rate?
The funding rate represents periodic payments between buyers and sellers of contracts based on the prevailing rate. When the rate is positive, buyers pay sellers, and when it's negative, the reverse occurs.

This rate is derived from the interest rate and a premium linked to the difference between futures and spot market prices. There are no transfer fees since the payments occur directly between users.

When trading perpetual contracts at a premium compared to spot markets, long positions pay shorts due to the positive funding rate. This can lead to the closure of long positions and the opening of new shorts, potentially impacting the price.

## What is the mark price?
The mark price is an evaluation of the true value of a contract compared to its current trading price (the price of the last transaction). This assessment helps prevent unfair position liquidations, especially during high market volatility.

While the index price is linked to the asset's price in spot markets, the mark price represents the true value of the contract irrespective of the current market price. It's often used in profit and loss (PnL) calculations and is a critical factor in determining potential gains and losses.

## What is an insurance fund?
An insurance fund serves as a reserve to protect traders' balances from dropping below zero in unsuccessful trades and ensures payouts in case of losses. It acts as a safeguard, providing coverage for losses incurred during users' asset liquidation.

Let's illustrate this with an example. Consider trader Louise, who has $2000 in her account for trading 10:1 leveraged ETH contracts. She opens a position for 100 ETH at a price of $20 each. When the price of ETH drops to $18, her position is automatically closed, and her $2000 collateral is utilized.

If the system fails to close all positions and the price continues to drop, the insurance fund comes into play, covering losses until the remaining positions are closed. This ensures compensation for participants who have gone bankrupt. Without the insurance fund, Louise's balance not only drops to zero but may go into negative values.

However, typically, the position will be closed earlier when its maintenance margin falls below the required level. Liquidation fees contribute to the insurance fund, and remaining funds are returned to users.

Thus, the insurance fund uses collateral from liquidated traders to cover the losses of bankrupt traders. It grows when positions are liquidated to zero or negative balances and, in extreme cases where the system cannot close all positions, it covers potential losses.

## What is auto-deleveraging?
Auto-deleveraging refers to the automatic liquidation of funds, occurring only if the insurance fund ceases to function. Although rare, in such an event, successful traders might be compelled to cover losses incurred by less fortunate participants. Due to the high volatility of the cryptocurrency market and the provision of high leverage to clients, completely avoiding such a situation is impossible.

This is a measure taken if the insurance fund cannot cover the losses of bankrupt users. Typically, positions with the highest profits and leverage have a more significant impact. Platforms provide indicators to allow users to understand where their trades stand in the queue for automatic liquidation.

Cryptocurrency platforms take steps to minimize the risk of auto-deleveraging, employing various features. In the event of this mechanism being activated, fund liquidation occurs without commissions, and affected traders promptly receive notifications. Users also retain the ability to freely create new positions at any time.
