# Generated NFT Contract and Deployment

This project uses hardhat to "randomly" generate an simple SVG with a single-color background and a three word string consisting of three random words chosen from Emily Dickenson's "Hope is a thing with feathers".

This contract generates the NFTs and stores meta-directly on-chain.

To use this contract you will need the following:

1. A metamask account with a Rinkeby wallet: https://metamask.io/
2. Some testnet ETH: https://faucet.rinkeby.io/
3. An AlchemyAPI account and API Key: https://www.alchemy.com/

To customize and deploy do the following:

1. Clone repo to local enviornment
2. In terminal run: npm install
3. In hardhat.config.js replace STAGING_ALCHEMY_KEY with your key
4. In hardhat.config.js replace PRIVATE_KEY with your Rinkeby wallet private key -- DO NOT SHARE THIS OR PUSH TO GITHUB
5. In terminal run: npx hardhat run --network rinkeby scripts/deploy.js
6. Contract is now deployed to testnet and can be viewed via https://rinkeby.etherscan.io/address/CONTRACT_ADDRESS
7. You can test minting an NFT programmatically by running: npx hardhat run --network rinkeby scripts/run.js
