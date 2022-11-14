# Pool strategies

Neuron Pools run two options strategies to generate yields:

1. **Covered call** - this pool writes out of the money covered calls;
2. **Put selling** - this pool writes out of the money collateralized puts.

### Covered Call strategy

The covered call strategy is a unique option strategy where you earn yield for selling _potential upside_ of an asset. For example, if you are willing to give up potential upside of ETH going above $25k by the end of the year, you can get paid 2% in yield for selling a $25k call option. This is over 10x the yield you can earn by supplying ETH on Compound.

In the unlikely case that ETH goes to $29k, you're up in USD yet giving up those potential $4k — still a favorable scenario for one because he/she only risks getting exercised when ETH skyrockets.

![](https://lh3.googleusercontent.com/5gdSViVsUtOVWa2qYWD3\_T28w84yD3EEqyKrzkUmN--Kyn0obIpMRRJmGlY9hfVakayL6QJeOy2MF8BB8TmjpRjTGu0ZNon4qbus7YisVmRYwxEJyo6mdGvxXqsDIaCcNZFEy-vjFT5t)

### Short Put strategy

Short put is virtually the same with a little quirk - the pool is selling out of money put options **secured by a collateral** to secure premium; payoff diagram is the same.

{% hint style="info" %}
If covered call gets assigned, the asset (e.g. WETH) gets "sold"; if assignment happens running a short put strategy - collateral is swapped for the asset at the strike price.&#x20;

So, say, if an ETH put option has a strike price of $25k, and ETH drops to $23k on expiry - a user may suffer a loss of $$Price_{Current}-Price_{Strike}+Premium_{Option}$$, with **option's premium offsetting** (and sometimes even **exceeding**) the adversary price difference.
{% endhint %}
