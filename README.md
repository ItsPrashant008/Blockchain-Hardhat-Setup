# Install Packages with Latest Version

# Dev-Dependencies

npm i --save-dev @nomicfoundation/hardhat-chai-matchers @nomicfoundation/hardhat-network-helpers @nomicfoundation/hardhat-toolbox @nomiclabs/hardhat-ethers @nomiclabs/hardhat-etherscan @nomiclabs/hardhat-solhint @nomiclabs/hardhat-waffle @openzeppelin/contracts-upgradeable @openzeppelin/hardhat-upgrades @typechain/ethers-v5 @typechain/hardhat @types/chai @types/mocha @types/node @typescript-eslint/eslint-plugin @typescript-eslint/parser chai chai-bignumber chai-bn dotenv eslint eslint-config-prettier eslint-config-standard eslint-plugin-import eslint-plugin-node eslint-plugin-prettier eslint-plugin-promise ethereum-waffle ethers hardhat hardhat-contract-sizer hardhat-gas-reporter prettier prettier-plugin-solidity solhint solidity-coverage ts-node typechain typescript

# Dependency

npm i @openzeppelin/contracts

# Using this packages you get Coverage / Gas Report

---

# Ethereum Network

#################################### Testnet Network ####################################

    Metamask Network Parameters
    Network Name: Goerli test network
    New RPC URL: https://goerli.infura.io/v3/
    Chain ID: 5
    Currency Symbol: GoerliETH
    Block Explorer URL: https://goerli.etherscan.io

Deploy: npx hardhat run --network goerli scripts/deploy.ts
Verify: npx hardhat verify --network goerli <token.address>

---

Polygon Network
#################################### Testnet Network ####################################

    Metamask Network Parameters
    Network Name: Mumbai Testnet
    New RPC URL: https://polygon-mumbai.g.alchemy.com/v2/<apikey>
    Chain ID: 80001
    Currency Symbol: MATIC
    Block Explorer URL: https://mumbai.polygonscan.com/

Deploy: npx hardhat run --network polygon_mumbai scripts/deploy.ts
Verify: npx hardhat verify --network polygon_mumbai <token.address>

#################################### Mainnet Network ####################################

    Network Name: Polygon Mainnet
    New RPC URL: https://polygon-rpc.com/
    Chain ID: 137
    Currency Symbol: MATIC
    Block Explorer URL: https://polygonscan.com/

Deploy: npx hardhat run --network matic scripts/deploy.ts
Verify: npx hardhat verify --network matic <token.address>

---

```

```
