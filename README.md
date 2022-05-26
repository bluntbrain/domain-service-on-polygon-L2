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

The Hardhat Runtime Environment, or HRE for short, is an object containing all the functionality that Hardhat exposes when running a task, test or script. In reality, Hardhat is the HRE.

domains: This variable is special because it's called a "state variable" and it's cool because it is stored permanently in the contract’s storage. Meaning anyone who calls the register function will permanently store data related to their domain right on our contract.

If the require logic fails the transaction is reverted, meaning that blockchain data doesn’t change.

Inheritance = it means we can call other contracts from ours. It's almost like importing functions for us to use!
https://solidity-by-example.org/inheritance/

We are able to mint NFTs using the standard known as ERC721 
https://eips.ethereum.org/EIPS/eip-721

For json -- NFTs use JSON to store details like the name, description, attributes and the media. What we’re doing with json is combining strings with abi.encodePacked to make a JSON object. We’re then encoding it as a Base64 string before setting it as the token URI.