# HelloWorldSolidity
Hello World Smart Contract in Solidity


Broadcasting Simple Transaction to local TestRPC blockchain
How to setup the development environment, connect the testRPC local blockchain to node console. Once set up, code a basic Ethereum transaction from scratch using "web3" and broadcast it to testRPC.
*Inside console1:
//Create dependencies in package.json using Sublime text editor
$ sublime package.son
*Inside package.json type in:
{
    "dependencies" : {
        "web3": "0.19.0",
        "solc": "0.4.11"
    }
}
//where web3 => https://github.com/ethereum/web3.js/ and solc => https://solidity.readthedocs.io/en/latest/using-the-compiler.html
*Inside console1
//install the packages
$ npm install
*Inside separately opened console2
$ testrpc
*Inside console1
$ node
> var Web3 = require("web3")
> var web3 = new Web3(new Web3.providers.HttpProvider("http://localhost:8545"))
//make sure you have access to testrpc accounts, gives a list of 10 accounts, start index at 0
> web3.eth.accounts
> var acct1 = web3.eth.accounts[0]
