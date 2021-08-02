# Security

## **Smart Contract Audits**

### Techrate **Audit**

An audit of the full suite of Neuron Capital smart contracts by Techrate had started on July 23, 2021.

To date, the following scope of Neuron's function-critical smart contracts were reviewed:

1. [https://github.com/avele/Neuron-Contracts/blob/master/contracts/NeuronToken.sol](https://github.com/avele/Neuron-Contracts/blob/master/contracts/NeuronToken.sol)
2. [https://github.com/avele/Neuron-Contracts/blob/master/contracts/MasterChef.sol](https://github.com/avele/Neuron-Contracts/blob/master/contracts/MasterChef.sol)
3. [https://github.com/avele/Neuron-Contracts/blob/master/contracts/Controller.sol](https://github.com/avele/Neuron-Contracts/blob/master/contracts/Controller.sol)
4. [https://github.com/avele/Neuron-Contracts/blob/master/contracts/strategies/StrategyBase.sol](https://github.com/avele/Neuron-Contracts/blob/master/contracts/strategies/StrategyBase.sol)
5. [https://github.com/avele/Neuron-Contracts/blob/master/contracts/Gauge.sol](https://github.com/avele/Neuron-Contracts/blob/master/contracts/Gauge.sol)
6. [https://github.com/avele/Neuron-Contracts/blob/master/contracts/Axon.sol](https://github.com/avele/Neuron-Contracts/blob/master/contracts/Axon.sol)
7. [https://github.com/avele/Neuron-Contracts/blob/master/contracts/GaugesDistributor.sol](https://github.com/avele/Neuron-Contracts/blob/master/contracts/GaugesDistributor.sol)

No critical or major issues were found in the aforementioned contracts. Minor issues have been fixed. The full report can be viewed [**here**](https://github.com/neuron-fund/audits/blob/master/Techrate%20audit.pdf).

An audit of the remaining contracts is underway and is expected to complete shortly.

## **Timelocks & Multisig**

All key admin functions on the [MasterChef](https://etherscan.io/address/0xbD17B1ce622d73bD438b9E658acA5996dc394b0d) contract, which controls NEURs emission, are controlled by a [**24 hour timelock contract**](https://etherscan.io/address/0x0040E05CE9A5fc9C0aBF89889f7b60c2fC278416).

All key admin functions relating to the Neuron Pools are controlled by a [**12 hour timelock contract**](https://etherscan.io/address/0xD92c7fAa0Ca0e6AE4918f3a83d9832d9CAEAA0d3).

Each of the above timelock contracts must be executed through a 2/5 community [**multisig wallet**](https://etherscan.io/address/0x9d074E37d408542FD38be78848e8814AFB38db17). The current multisig keyholders are as follows:

![https://gblobscdn.gitbook.com/assets%2F-MI-yJcvm6yA8baawmo4%2F-MSwxPIwdGNBirxB9nIL%2F-MSwz9covoAP3wOruCpI%2Fimage.png?alt=media&amp;token=a8491e72-7dd1-4341-a8b5-afb010960e0c](https://gblobscdn.gitbook.com/assets%2F-MI-yJcvm6yA8baawmo4%2F-MSwxPIwdGNBirxB9nIL%2F-MSwz9covoAP3wOruCpI%2Fimage.png?alt=media&token=a8491e72-7dd1-4341-a8b5-afb010960e0c)

### 🐜 Bug bounty program

Neuron Capital is running a continuous bug bounty program - we're paying _bountyAmount_ in NEURs or stablecoins to anyone who contacts us with a bug. We're taking security dead-serious - if you find one, click the image below to contact us:

![](../.gitbook/assets/image%20%283%29.png)

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6b686f5b-c8b6-4729-a369-5413fd0ab475/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6b686f5b-c8b6-4729-a369-5413fd0ab475/Untitled.png)

