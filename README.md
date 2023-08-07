# Build-an-nft-collection-with-a-whitelist-using-hardhat-and-solidit

This project demonstrates how build an nft collection with a whitelist using hardhat and solidity. 

Is part of https://learnweb3.io/degrees/ethereum-developer-degree/ course.

https://learnweb3.io/degrees/ethereum-developer-degree/sophomore/build-an-nft-collection-with-a-whitelist-using-hardhat-and-solidity/


# Run (testnet)

First you need to deploy Whitelist.sol

```shell
npx hardhat run scripts/deploy.js --network mumbai
```

Now you have to use the Contract Address generated in deploy-ntf.js script

```javascript
const contractAddress = "0xEB3dD8Ca9DE738948695Ec12448FFe3cDEA16CfB";
```

and deploy CrypotDevs.sol contract

```shell
npx hardhat run scripts/deploy-nft.js --network mumbai
```

# Play

You can play with the smartcontracts deployed by me:

-   https://mumbai.polygonscan.com/address/0xeb3dd8ca9de738948695ec12448ffe3cdea16cfb (Whitelist)
-   https://mumbai.polygonscan.com/address/0x133d06D87D8B429d530EaDb0684956F6A332569c (NFT)

First, you can add some address to Whitelist Contract (using etherscan funcionality) and after minting the NFT (with the same address and sending 0MATIC). 

Second, you can try mint a new NFT directly with a new address (not included in the whitelist) sending 0MATIC ¿What happened? :-) 

# ToDo

Write tests


