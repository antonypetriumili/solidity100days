# Solidity Functions

![Alt function](https://media1.tenor.com/images/649cb11ec4e7a08801e107ccbbb94648/tenor.gif?itemid=27526500)

# What are Solidity Functions 
A function is basically a group of code that can be reused anywhere in the program, which generally saves the excessive use of memory and decreases the runtime of the program. Creating a function reduces the need of writing the same code over and over again. With the help of functions, a program can be divided into many small pieces of code for better understanding and managing.

# Solidity Function Syntax

`Use the following syntax to create your Solidity ` function, as seen in the example below:

* Define the function with the function keyword
* Create a name for the function, which is unique and does not coincide with any of the reserved keywords
* List any parameters containing the name and data type of the parameter or include no extra parameters
* Create a statement block surrounded by curly brackets

`function function-name(parameter-list) scope returns() {  // statements} `

![Alt function](https://media1.tenor.com/images/5e44681dc08aaf26ac3f15b5098986d0/tenor.gif?itemid=27526510)

The image below shows the three main components of a Solidity function:

* Function name
* Function type
* Return types

# What are the different types of Solidity functions?
* # View Functions
In Solidity, view functions are read-only and cannot alter the state variables defined in a smart contract. The syntax for a view function is as follows:
` function <function-name>() <access-modifier> view returns() {  // function body } `
* # Pure Functions

A pure function declares that no state variable will be changed or read. Typically pure functions serve some common utility or calculation. The syntax for a pure function is as follows:
` function <function-name>() <access-modifier> pure returns() {  // function body } `

* # Special Functions

Solidity has a couple of special functions that you can use when developing a smart contract. Getter and receive functions are important payable functions for smart contracts in Solidity.


- Geeter Function
State variables defined as public have a getter function that is automatically created by the compiler. The function has the same name as the variable and has external visibility.
- Receive Ether Function
A contract can have at most one receive function. A receive function cannot have arguments, is unable to return, and must have external visibility and payable state mutability.

A receive function is executed on a call to the contract that sends Ether and does not specify any function. This function is declared as follows:



`receive() external payable {...}`

* # Fallback Function

In Solidity, a fallback function is an external function without a name, arguments, or return values. Fallback functions are executed when a function identifier doesn't match any of the available functions in a smart contract, or if there was no data supplied along with the function call.

# What is function overloading?

Function overloading occurs when you have multiple definitions for the same function name within the same scope. The definition of the function must differ from each other by the types and/or the number of arguments in the argument list. You cannot overload function declarations that differ only by return type.

# What does function visibility mean?
Specifying function visibility allows us to control which entities can call functions within the smart contract. There are three types of callers: 

* The main contract 
* A contract derived (i.e. inheriting) from the main contract 
* A third party

Function visibility helps you control which of the above callers can execute the function. There are four types of function visibility: 

* Public 
* External
* Internal
* Private

The accessibility of the functions decreases from External to Private: public functions are the most accessible and private functions are the least.

# External vs. Public 
External and public are the two function visibilities that can be called from outside of the contract they are defined within. External means that the function can exclusively be called by other contracts or Externally Owned Accounts (EOA). Public means that the function can be called externally or from within the contract itself.

# Internal vs. Private
As opposed to external and public, internal and private both disallow external parties from accessing the function. For a private function, only functions within the same contract can call it. For an internal function, functions within the same contract or functions within derived contracts can call it.

# CHECK OUT HOW IT IS USED
[Functions](https://github.com/BernardOnuh/100DaysOfSolidity/tree/main/2.SolidityFunctions)

