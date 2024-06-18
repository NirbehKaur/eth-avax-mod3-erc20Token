Project: Create and Mint Token

Description:
For this project, you will write a smart contract to create your own ERC20 token and deploy it using HardHat or Remix. Once deployed, you should be able to interact with it for your walk-through video. From your chosen tool, the contract owner should be able to mint tokens to a provided address and any user should be able to burn and transfer tokens.

# BitLand Token (BITL)

## Overview

BitLand Token (BITL) is an ERC20 token deployed on the Ethereum blockchain. It utilizes the OpenZeppelin library for ERC20 implementation and includes additional functionalities for minting and burning tokens.

## Features

- **Name**: BitLand Token
- **Symbol**: BITL
- **Decimals**: 18
- **Total Supply**: Customizable at deployment

## Contracts

### BitLandToken.sol

`BitLandToken.sol` is the main contract that defines the BitLand Token. It extends ERC20 and includes additional functionalities such as token minting and burning.

#### Functions

- `constructor(uint256 initialBalance)`: Initializes the token with an initial supply and assigns the entire supply to the deployer's address.
  
- `mint(address to, uint256 amount)`: Allows the owner to mint new tokens and assign them to a specified address.
  
- `burn(uint256 amount)`: Allows any token holder to burn a specific amount of their own tokens.
  
- `transfer(address recipient, uint256 amount)`: Overrides the transfer function from ERC20 to include additional validations.

### Dependencies

This project relies on OpenZeppelin's contracts for ERC20 and Ownable functionalities:
- ERC20: [OpenZeppelin ERC20.sol](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/v4.9.5/contracts/token/ERC20/ERC20.sol)
- Ownable: [OpenZeppelin Ownable.sol](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/v4.9.5/contracts/access/Ownable.sol)

## Getting Started

To deploy your own instance of BitLand Token, follow these steps:

1. Open remix ide and make a new .sol file.
2. Set the compiler version to 0.8.17+.... and compile the code.
3. Change environment to Remix VM(London) and put initial supply as 1000000000000000000000000 tokens and deploy it.
4. Run the functions mint, transfer, balanceOf, burn etc and play around with the functions.

## Usage

### Deploying the Token

Deploy the `BitLandToken` contract, specifying the initial supply in the constructor.

### Interacting with the Token

Use any Ethereum wallet or interface (such as MetaMask or Remix) to:
- View your balance of BITL tokens.
- Transfer tokens to other addresses.
- Mint new tokens if you are the owner.
- Burn your own tokens.


