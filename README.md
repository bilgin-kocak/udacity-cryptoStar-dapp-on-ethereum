# ND1309 C2 Ethereum Smart Contracts, Tokens and Dapps - Project Starter 
**PROJECT: Decentralized Star Notary Service Project** - For this project, you will create a DApp by adding functionality with your smart contract and deploy it on the public testnet.

Udacity Blockchain Developer project to develop a digital app and deploy to Ethereum network.

With this project I have learnt how to interact with the Ethereum Blockchain, create and deploy a smart contract
and develop a Web App

## Requirements
* Truffle
* OpenZeppelin 
* Node
* [Infura Account](https://infura.io/)
* MetaMask Browser Add-on

Asset|Details
---|---
Truffle Version|5.3.8
OpenZeppelin|2.1.2
ERC-721 Token Name|Bilgin StarToken
ERC-721 Token Symbol|BST
Token Address @ Rinkeby|[0x2eb697bb0b6c6002a54a1dad0091f1262048f083](https://rinkeby.etherscan.io/address/0x2eb697bb0b6c6002a54a1dad0091f1262048f083)

## Installation
1) Download App
    ```
    git clone https://github.com/stevenhankin/udacity-cryptoStar-dapp-on-ethereum.git
    cd udacity-cryptoStar-dapp-on-ethereum
    ```
2) Put your Infura Project Secret into ".secret" file
    ```
    echo "Metamask Wallet Seed" > .secret
    ```
3) Install required packages
    ```
    npm install && cd app && npm install
    ```
4) In truffle-config.js, set **infuraKey** to be your Infura Project ID
5) From Crypto-Star-Dapp root, deploy StarNotary contract to network
    ```
    truffle compile
    truffle migrate --network rinkeby
    ```
6) Start App Server
    ```
    cd app
    npm run dev
    ```
7) Application should now be available on http://localhost:3000

# Testing
Start ```truffle develop``` then run the following:
```
migrate --reset
test


### Dependencies
For this project, you will need to have:
1. **Node and NPM** installed - NPM is distributed with [Node.js](https://www.npmjs.com/get-npm)
```bash
# Check Node version
node -v
# Check NPM version
npm -v
```


2. **Truffle v5.X.X** - A development framework for Ethereum. 
```bash
# Unsinstall any previous version
npm uninstall -g truffle
# Install
npm install -g truffle
# Specify a particular version
npm install -g truffle@5.0.2
# Verify the version
truffle version
```


2. **Metamask: 5.3.1** - If you need to update Metamask just delete your Metamask extension and install it again.


3. [Ganache](https://www.trufflesuite.com/ganache) - Make sure that your Ganache and Truffle configuration file have the same port.


4. **Other mandatory packages**:
```bash
cd app
# install packages
npm install --save  openzeppelin-solidity@2.3
npm install --save  truffle-hdwallet-provider@1.0.17
npm install webpack-dev-server -g
npm install web3
```


### Run the application
1. Clean the frontend 
```bash
cd app
# Remove the node_modules  
# remove packages
rm -rf node_modules
# clean cache
npm cache clean
rm package-lock.json
# initialize npm (you can accept defaults)
npm init
# install all modules listed as dependencies in package.json
npm install
```


2. Start Truffle by running
```bash
# For starting the development console
truffle develop
# truffle console

# For compiling the contract, inside the development console, run:
compile

# For migrating the contract to the locally running Ethereum network, inside the development console
migrate --reset

# For running unit tests the contract, inside the development console, run:
test
```

3. Frontend - Once you are ready to start your frontend, run the following from the app folder:
```bash
cd app
npm run dev
```

---

### Important
When you will add a new Rinkeyby Test Network in your Metamask client, you will have to provide:

| Network Name | New RPC URL | Chain ID |
|---|---|---|
|Private Network 1|`http://127.0.0.1:9545/`|1337 |

The chain ID above can be fetched by:
```bash
cd app
node index.js
```

