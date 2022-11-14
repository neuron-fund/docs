---
description: >-
  A more in-depth explanation of yield-bearing nature of Neuron pools,
  strategies used and the auction process.
---

# Technical Architecture

### Neuron pools scheme

![](<../../.gitbook/assets/Option pool (1).png>)

Option Pools rely on **** [neuron-options.md](../neuron-options.md "mention")**,** noTokens (Neuron Option Tokens). noToken is a ERC20 token representation of an option contract, with each having a strike price and expiry.&#x20;

{% hint style="info" %}
Owning a noToken is functionally equivalent to owning an option contract. This gives the token holder the right to redeem some amount of the underlying asset if the strike price is hit.
{% endhint %}

In order to run an options-writing strategy, the Option Pool needs to be able to **mint** and **short noTokens**.&#x20;

1. User deposits tokens to the Neuron Pool.
2. Option Pool sends the token to the Option Wrapper contract, and here the magic happens:
3. Wrapped token is used as the collateral in Neuron Options contract to mint noTokens.
4. noTokens are sent back to the Option Pool contract to be used in **option strategies**,
5. while tokens are transferred to LPs for **additional LP yield.**

{% hint style="warning" %}
The Pool's collateral will be locked until the expiry of the noToken. This collateral is used to pay off noToken holders in the case that the options expire in the money.
{% endhint %}

Choosing the strike price is automated by Neuron Option pool. The options are sold weekly through an on-chain [batch auction](https://coinmarketcap.com/alexandria/glossary/batch-auctions).

### Batch auction

In collaboration with option market makers taking part in the auction, below is a diagram of how an options sale is conducted:

![Option sale cycle](<../../.gitbook/assets/Options lifecycle.png>)

{% hint style="success" %}
The net result of this process is that Neuron Option Pools receive premiums in return for writing the noTokens. It means that the **Pool's balance will likely expand over time** as premiums are collected and compounded.
{% endhint %}
