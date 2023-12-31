## CONTRACT IN SOLIDITY
![Contract](https://media1.tenor.com/images/b84dc4ed2481267c0a939652dda2486d/tenor.gif?itemid=27567662)
### What is Contract in Solidity ?
A solidity contract is a block of code that contains functions and state variables. it is stored on a specific address on the Ethereum blockchain.

[ExamplesOfStateVariable](https://github.com/BernardOnuh/100DaysOfSolidity/tree/main/3.Variable)
[ExamplesOfSolidityFunctions](https://github.com/BernardOnuh/100DaysOfSolidity/tree/main/2.SolidityFunctions)

### Creating a contract
Every Solidity code starts with pragma version. The **pragma** version specifies the version of complier that the code should use.

> pragma solidity ^0.8.10;

To create a contract we use the **contract** keyword followed by the contract name. Inside the { brackets},we create the variables and functions 

> contract contractName { //code }

### Lets write our first contract

Our first contract would allow us write the follwing on the blockchain

- Our Name
- Our Age

[contract](https://github.com/BernardOnuh/100DaysOfSolidity/blob/main/8.Contract/contract.sol)