# 💹 Option pricing basics

![An infographic on an option’s premium composition. Source](https://miro.medium.com/max/874/1\*v-kfmKeVWyB\_q3mvwdC18A.png)

Don’t mind the typo in the risk-free rate (oops, now you’ve seen it), WSMojo’s done an awesome job at explaining the constituents! So, while intrinsic value is the difference between the strike price and the underlying asset price, the extrinsic part is the option’s “real”, almost-tangible value comprised of its time and volatility values.

Think of it the following way — you’re either buying **an insurance policy** or selling it (as an insurance company); time value would be the **length of your policy**, and your **coverage** will be \~volatility value. So, you’re invested in the **ability to make a choice now or in the future** (but only if you’re American! Not an offense, please refer to option styles above).

If something can be calculated at scale, it needs an input and an output. Options got this in spades, and the most popular way of price calculation (option pricing, as such) is the **Black-Scholes-Merton equation**, [described in great detail by CFI.](https://corporatefinanceinstitute.com/resources/knowledge/trading-investing/black-scholes-merton-model/) It’s not for the math-uninitiated (albeit not the most complex one), here’s a sneak peek:

![BSM formula. Source](https://miro.medium.com/max/676/1\*ofUfr0NYA6v9HTtbIL-WbA.png)
