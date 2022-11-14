# 🇬🇷 Options greeks

### **Delta**

**Delta** is a measure of option price’s sensitivity to a one-point move in asset’s price (mathematically it’s the first derivative of an option’s price): _ΔOptionPrice/$1(AssetPrice)_

### **Gamma**

**Gamma** is logically (it goes after delta), a second derivative. It denotes changes in delta per one point of asset’s price: _ΔDelta/$1(AssetPrice)_

### Theta

**Theta:** an immensely important greek. It’s how much an option changes in price per day, and it goes down as expiration moves closer. Below is a basic chart of an option’s value decaying.

![Option’s value decay due to theta. Source](https://miro.medium.com/max/875/1\*a4U4lYvCSZIycCJpi7d\_ig.png)

### Vega

**Vega** is option’s sensitivity to an underlying asset’s change in volatility. Usually, higher near the strike price recedes nearing expiration. A great visualization by QC is below:

![3D chart of an option’s vega changes respective to asset price and time to expiration. Source](https://miro.medium.com/max/875/1\*Bh6J8PAS82YidhwFqhjoLQ.png)

{% hint style="info" %}
Even more on option greeks at [QuantConnect](https://www.quantconnect.com/tutorials/introduction-to-options/the-greek-letters) and [Investopedia](https://www.investopedia.com/trading/using-the-greeks-to-understand-options/)’s excellent write-ups.
{% endhint %}
