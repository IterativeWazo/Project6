# Coffee supply chain 

This repository contains an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

## Contract address
  ```
   "networks": {
    "3": {
      "events": {},
      "links": {},
      "address": "0x4d1e5fe4f2555276576d67faba43981d1871a13c",
      "transactionHash": "0x451c87de29eec37729bbdf349006f3cc0371f73a889d949197c367ac5b8677ac"
    },
  ```

### Prerequisites

Please make sure the following software installs:
  ```
  Truffle v4.1.14 (core: 4.1.14)
  Solidity v0.4.24 (solc-js)
  node v10.13.0
  Ganache CLI v6.7.0 (ganache-core: 2.8.0)
  MetaMask extension in your browser
  ```

### Installing
Clone this repository:

```
git clone https://github.com/IterativeWazo/Project6.git
```

Change directory to ```project-6``` folder and install all requisite npm packages (as listed in ```package.json```):

```
cd project-6
npm install
```
After this step, the following dependencies/libraries will be installed:

```
"devDependencies": {
    "lite-server": "2.4.0",
    "truffle-hdwallet-provider": "^1.0.17"
  }
```



Launch Ganache:

```
ganache-cli -m "spirit supply whale amount human item harsh scare congress discover talent hamster"
```

In a separate terminal window, Compile smart contracts:

```
truffle compile
```


This will create the smart contract artifacts in folder ```build\contracts```.

Migrate smart contracts to the locally running blockchain, ganache-cli with ropsten test network:

```
truffle migrate --network ropsten
```

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

In a separate terminal window, launch the DApp:

```
npm run dev
```


