# Domain Service on Polygon L2

This project demonstrates a basic Hardhat use case. 

Try running some of the following tasks:

```shell
npx hardhat accounts
npx hardhat compile
npx hardhat clean
npx hardhat test
npx hardhat node
node scripts/sample-script.js
npx hardhat help
```
```shell
npx hardhat run scripts/run.js
```

```shell
To deploy to Mumbai testnet
npx hardhat run scripts/deploy.js --network mumbai
```

Deployed domains
1. 0x81C9787e0CCC116475330b324a0D08B4f3FfaDE9
2. 0x0a51B2538F59ddCAAAE51F68347c8232D4B44406

Owner of domains: 0xc2223264b4B8f3F98c4DBF0c2f6Be2700Ae86062
Contract balance: 0.1

Opensea link to minted domain: https://testnets.opensea.io/assets/mumbai/0x81c9787e0ccc116475330b324a0d08b4f3ffade9/0

The Hardhat Runtime Environment, or HRE for short, is an object containing all the functionality that Hardhat exposes when running a task, test or script. In reality, Hardhat is the HRE.

domains: This variable is special because it's called a "state variable" and it's cool because it is stored permanently in the contract’s storage. Meaning anyone who calls the register function will permanently store data related to their domain right on our contract.

If the require logic fails the transaction is reverted, meaning that blockchain data doesn’t change.

Inheritance = it means we can call other contracts from ours. It's almost like importing functions for us to use!
https://solidity-by-example.org/inheritance/

We are able to mint NFTs using the standard known as ERC721 
https://eips.ethereum.org/EIPS/eip-721

For json -- NFTs use JSON to store details like the name, description, attributes and the media. What we’re doing with json is combining strings with abi.encodePacked to make a JSON object. We’re then encoding it as a Base64 string before setting it as the token URI.

Alchemy helps us broadcast our contract creation transaction so that it can be picked up by miners as quickly as possible. Once the transaction is mined, it is then broadcasted to the blockchain as a legit transaction. From there, everyone updates their copy of the blockchain.

What is a signer?
https://docs.ethers.io/v5/api/signer/#signers

What is an ABI file?
https://docs.soliditylang.org/en/v0.8.11/abi-spec.html

What is Gas?
https://ethereum.org/en/developers/docs/gas/

How to update the contract in a project
You'd need to do 3 things:

```shell
1. We need to deploy it again.
2. We need to update the contract address on our frontend.
3. We need to update the abi file on our frontend.
```