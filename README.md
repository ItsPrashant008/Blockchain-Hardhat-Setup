If you are setting up by cloning, please remove the "@nomicfoundation/hardhat-toolbox" and "@typechain/hardhat" packages from the package.json because they might not install correctly due to different package versions. After removing them, make sure to add "--force install" at the end to forcefully install all the packages.

# Install Package

    npm install --save

    npm i --save-dev @nomicfoundation/hardhat-toolbox @typechain/hardhat --force

---

These packages will help you in both small and large projects. They will assist you in testing, generating code coverage, determining contract size, and calculating contract gas fees/prices in USD.

<h1> If you want to set up the app from scratch, follow these steps: </h1>

# Install Packages with Latest Version

<b> Create Package.json file </b>

    npm init -y

<b> Dependencies </b>

    npm i --save-dev @nomiclabs/hardhat-waffle @nomiclabs/hardhat-ethers @nomiclabs/hardhat-etherscan @nomiclabs/hardhat-solhint @nomicfoundation/hardhat-network-helpers @types/chai @types/mocha @types/node chai chai-bignumber chai-bn dotenv eslint eslint-config-prettier eslint-config-standard eslint-plugin-import eslint-plugin-node eslint-plugin-prettier eslint-plugin-promise ethereum-waffle ethers hardhat hardhat-contract-sizer hardhat-gas-reporter prettier prettier-plugin-solidity solhint solidity-coverage ts-node typescript typechain @typechain/ethers-v5 @typescript-eslint/eslint-plugin @typescript-eslint/parser

    npm i @openzeppelin/contracts @openzeppelin/hardhat-upgrades@1.28.0 @openzeppelin/contracts-upgradeable

    npm i --save-dev @nomicfoundation/hardhat-toolbox @typechain/hardhat --force

---

# For Hardhat Setps

    npx hardhat

<b> Choose script, I choose Typescript </b>
<b> Add .git ignore </b>
<b> No need to install hardhat-toolbox, we already install </b>

<h2> you can remove the existing contracts, testing files, and scripts from the project and replace them with your own contracts, tests, and scripts. </h2>

<b> Make sure to update your Hardhat configuration and create a .env file, You can refer to the example .env file provided and make the necessary updates to your own .env file and the Hardhat configuration file based on your network specifications.</b>

<p> ETHERSCAN_API_KEY </p>: <span> You will get the ETHERSCAN API KEY from etherscan.io, for which you need to log in to etherscan.io. After logging in, go to the "https://etherscan.io/myapikey" website and create your API key there. </span>
<p> ALCHEMY_GOERLI_API_KEY </p>: <span> You can get the ALCHEMY GOERLI API KEY either from Alchemy or create it from Infura. You have the option to create an API key from Alchemy based on your network preferences by visiting https://dashboard.alchemy.com/. Moreover, you can also use Alchemy's "faucet" feature to get test Ether for your Goerli network or other network. </span>
<p> PRIVATE_KEY </p>: <span> You can obtain your private key from your public address in MetaMask. </span>

# Then, Test your Smart contract

    npx hardhat clean

    npx hardhat compile

    npx hardhat test

    npx hardhat coverage

<b> After Successfully run test case you can use this setup as per you code/contract <b>

---

<h1> Ethereum Network <h1>
<h2> Add Network Network in MetaMask <h2>

# -------- Testnet Network --------

    Metamask Network Parameters
    Network Name: Goerli test network
    New RPC URL: https://goerli.infura.io/v3/
    Chain ID: 5
    Currency Symbol: GoerliETH
    Block Explorer URL: https://goerli.etherscan.io

# Deploy:

    npx hardhat run --network goerli scripts/deploy.ts

# Verify:

     npx hardhat verify --network goerli <token.address>

---

Polygon Network

# -------- Testnet Network --------

    Metamask Network Parameters

    Network Name: Mumbai Testnet
    New RPC URL: https://polygon-mumbai.g.alchemy.com/v2/<apikey>
    Chain ID: 80001
    Currency Symbol: MATIC
    Block Explorer URL: https://mumbai.polygonscan.com/

Deploy: npx hardhat run --network polygon_mumbai scripts/deploy.ts
Verify: npx hardhat verify --network polygon_mumbai <token.address>

# -------- Mainnet Network --------

    Network Name: Polygon Mainnet
    New RPC URL: https://polygon-rpc.com/
    Chain ID: 137
    Currency Symbol: MATIC
    Block Explorer URL: https://polygonscan.com/

Deploy: npx hardhat run --network matic scripts/deploy.ts
Verify: npx hardhat verify --network matic <token.address>
