# Lottery in Ethereum

This repository contains a sample project that user can use to place bet for lottery. It's base on other project named
[Hardhat Hackathon Boilerplate](https://github.com/nomiclabs/hardhat-hackathon-boilerplate) (thanks a lot). It is also a hardhat framework project. And its frontend is an React App.

## Quick start

The first things you need to do are cloning this repository and installing its
dependencies:

```sh
git clone https://github.com/FeiyangTan/Lottery.git
cd Lottery
npm install
```

Once installed, let's run Hardhat's testing network. Of course you can config to run rinkeby or other test network by edit the hardhat.config.js file:

```sh
npx hardhat node
```

Then, on a new terminal, go to the repository's root folder and run this to
deploy your contract:

```sh
npx hardhat run scripts/deploy_upgradeable.js --network localhost
```

Finally, we can run the frontend with:

```sh
cd frontend
npm install
npm start
```

> Note: If you modify the contract, and compile sucessfully, you should sync the artifacts into frontend/src/contracts directory, and update the right address for the deployed contract. So the app can invoke the contract correctly.

Open [http://localhost:3000/](http://localhost:3000/) to see your Dapp. You will
need to have [Metamask](https://metamask.io) installed and listening to
`localhost 8545`.

## What’s Included?

Your environment will have everything you need to build a Dapp powered by Hardhat and React.

- [Hardhat](https://hardhat.org/): An Ethereum development task runner and testing network.
- [Mocha](https://mochajs.org/): A JavaScript test runner.
- [Chai](https://www.chaijs.com/): A JavaScript assertion library.
- [ethers.js](https://docs.ethers.io/ethers.js/html/): A JavaScript library for interacting with Ethereum.
- [Waffle](https://github.com/EthWorks/Waffle/): To have Ethereum-specific Chai assertions/mathers.
- [A sample frontend/Dapp](./frontend): A Dapp which uses [Create React App](https://github.com/facebook/create-react-app).

## Troubleshooting

- `Invalid nonce` errors: if you are seeing this error on the `npx hardhat node`
  console, try resetting your Metamask account. This will reset the account's
  transaction history and also the nonce. Open Metamask, click on your account
  followed by `Settings > Advanced > Reset Account`.

## Feedback, help and news

We'd love to have your feedback on this tutorial. Feel free to reach us through
this repository or [My Contact Info]().

**Happy _buidling_!**
