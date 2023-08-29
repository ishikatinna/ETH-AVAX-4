# ETH-AVAX-4 (Degen Token) Building on Avalanche

It represents a custom ERC-20 token contract called "DegenToken" with the symbol "DGN." It is based on the OpenZeppelin ERC20 implementation and introduces additional features such as token minting by the contract owner, token transfers, burn, and redeeming by users.
## Description
The smart contract extends the `ERC20` contract from the `OpenZeppelin` library, creating a new token with the name "Degen Token" and the symbol "DGN." The contract's owner has special privileges to mint new tokens to specified addresses. Users can transfer tokens to others, redeem and burn tokens from their own address, permanently reducing their token balance. The contract allows users to check their token balances as well. The code is licensed under the MIT License.     
`mint`        
The mint function allows the contract owner to create new tokens and add them to a specified address. It takes two parameters: "account" (the address to receive the new tokens) and "amount" (the number of tokens to create). This function can only be executed by the contract owner due to the "onlyOwner" modifier.     

`transfer`     
The contract overrides the ERC20's "transfer" function. It allows users to transfer tokens to another address. The function ensures that the transaction is successful by returning "true" if the transfer is completed.     

`redeem`        
The redeem function allows users to destroy tokens from their own address. This effectively reduces their token balance. The burning process is permanent, and the tokens cannot be recovered once burned.        

`checkBalance`    
The checkBalance function allows users to query their token balance by providing their address. It returns the number of tokens held by the given address.       

## Geting Started
### Prerequisites
1. Ethereum wallet to sign transactions for deploying the smart contract such as Metamask. Add `Avalanche fuji` network in Metamask.
2. A web-based integrated development environment for Ethereum smart contracts (REMIX IDE). 
3. Ethereum Development Environment setup to interact with the Ethereum blockchain and deploy smart contract.
### Executing program
*Step 1:* Go to [Remix IDE](https://remix.ethereum.org/) and create a new file called DegegenToken.sol.     

*Step 2:* Update the DegenToken.sol file with the code snippet i.e. Import the OpenZeppelin ERC20 contract and initialize the token, inheriting from the ERC20.sol contract.

*Step 3:* Compile your contract and prepare it for deployment.

*Step 4:* Go to Deploy and run transactions and select environment Injected Provider - MetaMask.     

 *Step 5:* For verify your smart contract deployment and other information on Snowtrace. Copy the contract address from remix and paste the contract address in search bar.     

 *Step 6:* Click on search icon to retrieve information about the deployed ERC20 token contract.   

 *Step 7:* Now, you are able to see your transactions and all information related to this contract.
 ## Authors
 Ishika Tinna
## License
This project is licensed under the MIT License.
