# SmartContract Lottery

How it works:

> 1. Users will be able to enter the lottery using ETH whose price will be based on USD - > 50$
> 2. An administrator decides when the lottery ends (Upgrade with DAO and Chainlink Keepers)
> 3. The lottery selects a winner randomly

An Alchemi API key was used to connect to mainnet-fork-dev

Testing:

> 1. 'mainnet-fork'.
> 2. 'development' with Mocks.
> 3. 'testnet'



```console
(brownieProject) user@DESKTOP-9GLMDS2:~/Smart-Contracts/smartcontract-lottery$ brownie test --network mainnet-fork-dev
Brownie v1.19.3 - Python development framework for Ethereum

New compatible solc version available: 0.6.6
Compiling contracts...
  Solc version: 0.6.6
  Optimizer: Enabled  Runs: 200
  EVM Version: Istanbul
Generating build data...
 - smartcontractkit/chainlink-brownie-contracts@1.1.1/AggregatorV3Interface
 - Lottery

============================================= test session starts ==============================================
platform linux -- Python 3.10.6, pytest-6.2.5, py-1.11.0, pluggy-1.0.0
rootdir: /home/user/Smart-Contracts/smartcontract-lottery
plugins: eth-brownie-1.19.3, forked-1.4.0, web3-5.31.3, hypothesis-6.27.3, xdist-1.34.0
collected 1 item

Launching 'ganache --chain.vmErrorsOnRPCResponse true --wallet.totalAccounts 10 --fork.url https://eth-mainnet.g.alchemy.com/v2/y-T67Jfyv1a8_xedzxQO3KuNiy_BsM70 --wallet.mnemonic brownie --server.port 8545 --hardfork istanbul'...

tests/test_lottery.py .                                                                                  [100%]

============================================== 1 passed in 9.08s ===============================================
Terminating local RPC client...
```
