# 🔍 Security

## **Smart Contract Audits**

### Pessimistic Security

We've **completed an audit** by [Pessimistic Security](https://pessimistic.io/) in August'2022:

* [Neuron Pools](https://github.com/pessimistic-io/audits/blob/main/Neuron%20Option%20Strategy%20Security%20Analysis%20by%20Pessimistic.pdf)
* [Option Protocol](https://github.com/pessimistic-io/audits/blob/main/Neuron%20Options%20Security%20Analysis%20by%20Pessimistic.pdf)

## **Timelocks & Multisig**

All key admin functions on the `MasterChef` contract, which controls NEURs emission, are controlled by a 24 hour timelock contract.

All key admin functions relating to the Neuron Pools are controlled by a 12 hour timelock contract.

Each of the above timelock contracts must be executed through a **community multisig wallet**.

## 🐜 Bug bounty program

Neuron Fund is planning to run a continuous bug bounty program - we'll be paying up to $25,000 in NEURs or stablecoins to anyone who finds a bug.&#x20;
