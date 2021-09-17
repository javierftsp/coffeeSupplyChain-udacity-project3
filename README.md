# Supply chain & data auditing

This repository containts an Ethereum DApp that demonstrates a Supply Chain flow between a Seller and Buyer. The user story is similar to any commonly used supply chain process. A Seller can add items to the inventory system stored in the blockchain. A Buyer can purchase such items from the inventory system. Additionally a Seller can mark an item as Shipped, and similarly a Buyer can mark an item as Received.

## download and install

In order to test this application locally you need to download the source code and run the following commnads:
First clone this repository:

```
git clone https://github.com/javierftsp/coffeeSupplyChain-udacity-project3
```

Change directory to ```project-6``` folder and install all requisite npm packages (as listed in ```package.json```):

```
cd project-6
npm install
```

Launch Ganache:

```
ganache-cli -m "spirit supply whale amount human item harsh scare congress discover talent hamster"
```

Your terminal should look something like this:

![truffle test](images/ganache-cli.png)

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

Your terminal should look something like this:

![truffle test](images/truffle_compile.png)

This will create the smart contract artifacts in folder ```build\contracts```.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Your terminal should look something like this:

![truffle test](images/truffle_migrate.png)

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

![truffle test](images/truffle_test.png)

## Testing the DApp:

In a separate terminal window, launch the DApp:

```
npm run dev
```


## Front End
![product overview](images/screenshot_product_overview.png)

![farm detail](images/screenshot_farm_details.png)

![product detail](images/screenshot_product_details.png)

![transaction history](images/screenshot_transaction_history.png)


## Versions
* Truffle v5.4.8
* Solidity ^0.4.24
* Node v14.17.6
* Web3.js v1.5.2

## Rinkeby Contract Address
* transaction hash:    0x216dff6b01c1f984b56f9b366d000f9c49af17b92309e18654d4799413c223a3
* contract address:    0x66CfC8aec06C5617D634ed10D08a1651894Dacd9
