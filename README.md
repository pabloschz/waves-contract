# WavesPortal contract

Basic Smart Contract definition and deploy command.

Basic usage:
- Store a Wave Struct globally with some methods for retrieve and create a new wave to the contract creator address-
- Randomly (50% chance) reward to the waver with an amount `0.0001 ether`
- Avoid spam allowing only 15 minutes between each wave.

Command for test the smart contract functionallity before push in a hardhat network local:
```shell
npx hardhat run scripts/run.js
```

Before deploy the smart contract you need:
- Get some rinkeby ETH for fund the smart contract during the deploy
- Create a `.env` with the following values:
    - ALCHEMY_KEY: Alchemy app url.
    - PRIVATE_KEY: Metamask private key.

Command for deploy the contract to the rinkeby netowork:
```shell
npx hardhat run scripts/deploy.js --network rinkeby
```