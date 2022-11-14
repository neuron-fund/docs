# Strike selection

To further reduce the risk of our options getting exercised, we can sell call options that expire sooner rather than later, because of how difficult it is to predict how ETH could perform over a longer time frame. Our initial pools will sell _weekly_ call options, meaning we can adjust our expectation of ETH’s price on a weekly basis. This also has the nice side effect of letting us **compound our premiums more frequently**.

Weekly options are the best for one more reason - theta (one of option's "greek" parameters, basically $$Change_{OptionPrice}/Change_{Time}$$ ) decay is highest with short-term options, so our **time-premium collecting efficiency is a lot higher**:

![Source: https://www.optionmatters.ca/top-3-strategies-to-generate-income-with-options/](<../../.gitbook/assets/image (25).png>)

Secondly, we need to select strike prices that are far enough from today’s spot price to reduce the risk of exercise. Our current methodology for strike selection and backtests show that we only get exercised less than 5% of the time from Jan 2020 to today, even throughout the entire run up of ETH from $80 to $2000.&#x20;

{% hint style="success" %}
We've done two rounds of backtesting: for [simple option-writing strategies](https://medium.com/neuron-fund/backtesting-option-writing-strategies-the-neuron-way-48eb69d8fb73) and [complex ones](https://medium.com/neuron-fund/backtesting-mk-2-2d5ffa5e73fc), including multi-legged.
{% endhint %}
