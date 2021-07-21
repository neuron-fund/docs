# Vote locking

## What is Vote Locking?

Vote-locking is a modified form of governance staking. Governance voters lock their governance tokers to participate in voting. This prevents governance attacks and aligns incentives between voters and long-term holders.

### What is AXON?

AXON is Neuron Capital's governance token, and is used, as a real-life neuron uses axon, for connections and signal transduction. You can vote-lock your NEURs for AXONs in order to:

1. Participate in voting, both [off-chain and on-chain](https://www.notion.so/Governance-401e79aea5c746b19a59cb059c9712d4) \(1 AXON = 1 vote\)
2. NEUR farm **weight voting rights**, AXON holders get to vote on the farm gauges for NEUR emissions.
3. Receive up to **2.5x** [**boost**](https://www.notion.so/Reward-boosts-bad8ca0f89f34dc5b014cf03cf20c61d) **in NEUR rewards** \(click for a more in-depth explanation and some formulas!\)
4. Receive **50% of the protocol's revenue**, distributed in weekly NEURs ⇒ [Profit sharing](https://www.notion.so/Profit-sharing-12e824c7e8284e6d81c9709483fe920c)

See [here](https://www.notion.so/Locking-NEUR-for-AXON-19c17b434df745b9a13a60be0e2a2785) for a guide on interacting with AXON on the UI.

### How is AXON balance calculated?

AXONs represent your balance of NEURs that have been vote-locked, weighed for the time remaining in the lock. The longer the time remaining in the lock, the more AXON you will have for the same amount of locked NEURs:

![](../.gitbook/assets/image%20%285%29.png)

The number of AXONs and subsequently voting power **decrease linearly over time**. Basically if you've locked 1000 NEURs for a year, your voting power over time will look like that, slow but steady:

![](../.gitbook/assets/chart.svg)

## How is my boost calculated?

Boost calculation is a function with several parameters, more info on it here.

You can find the current DAO voting power and boosting coefficient at this page

A calculator is on the way \(by the way\)!

## What if I provide liquidity in multiple pools?

Your voting power applies to all gauges but may produce different boosts based on how much liquidity you are providing and how much total liquidity the pool has.

## What happens if more people vote lock?

If other liquidity providers vote lock more NEUR, your boost will stay what it was when you applied it. If you abuse this, another user can kick and force a boost update to take you down to your real boost.

## How often does my boost records voting power changes?

Your voting weight decreases over time but your boost will take notice of your decreasing voting power at certain checkpoints like withdrawing, depositing into a gauge or minting CRV.

For example if you start at 1000 AXON and your voting power decreases to 800 AXON, your boost will still use your original voting power of 1000 AXON until a user checkpoint.

## How can I apply my boost?

After creating or adding to your lock, you need to click the apply boost button to update your boost on each of the gauge you're providing liquidity in. Your boost can also be updated by depositing or withdrawing from a gauge.

## How to know my boost is active?

If your boost is showing then it is active.

If you have locked but your boost isn't showing then you need to apply it.

