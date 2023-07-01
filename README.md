Using these packages are used in a project, like in testing, configs, contract, scripts. For those no need to use any additional package for right and test smart contract. After these packages you check code coverage, contract size, contract and methods gas fee/ price in usd etc.

<b> Take a Clone or Setup</b>

# Install Packages with Latest Version ( Using this packages you get Coverage / Gas Report )
--

# Setps

    npm init -y

# Dev-Dependencies

    npm i --save-dev @nomiclabs/hardhat-waffle @nomiclabs/hardhat-ethers @nomiclabs/hardhat-etherscan @nomiclabs/hardhat-solhint  @nomicfoundation/hardhat-network-helpers @openzeppelin/hardhat-upgrades  @openzeppelin/contracts-upgradeable @types/chai @types/mocha @types/node chai chai-bignumber chai-bn dotenv eslint eslint-config-prettier eslint-config-standard eslint-plugin-import eslint-plugin-node eslint-plugin-prettier eslint-plugin-promise ethereum-waffle ethers hardhat hardhat-contract-sizer hardhat-gas-reporter prettier prettier-plugin-solidity solhint solidity-coverage ts-node typescript typechain @typechain/ethers-v5 @typescript-eslint/eslint-plugin @typescript-eslint/parser

# Dependency

    npm i @openzeppelin/contracts

# Dev-Dependencies

    npm i --save-dev @nomicfoundation/hardhat-toolbox @typechain/hardhat --force

--

# Setps

    npx hardhat

<!-- Choose script, I choose Typescript -->
<!-- Add .git ignore -->
<!-- No need to install hardhat-toolbox -->

    npx hardhat compile

    npx hardhat test

# Then, Add Test, Contract, Hardhat Config and Env files and Run testcases

    npx hardhat clean

    npx hardhat compile

    npx hardhat test

<!-- After Successfully run test case you can use this setup as per you code/contract -->

---

# Ethereum Network

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
