# PlatinumToken (MNT) README

## Overview

PlatinumToken (MNT) is a simple ERC-20 token smart contract built on the Ethereum blockchain. It is designed to be used as a standard fungible token with additional functionality for minting and burning tokens. The contract also inherits from the Ownable contract, ensuring that only the owner can perform certain privileged operations.

## Features

 **Token Name and Symbol:** The token is named "PlatinumToken" with the symbol "MNT."

 **Minting Tokens:** Only the owner of the contract can mint new tokens. This feature allows for the controlled creation of new tokens, typically used for initial token distribution or as part of a rewards mechanism.

 **Burning Tokens:** Token holders can burn their own tokens, reducing the total supply. This feature is useful for token holders who wish to permanently remove some of their tokens from circulation.

 **Transfer Tokens:** Standard ERC-20 functionality is provided for transferring tokens between addresses. Users can transfer tokens to others, subject to the availability of sufficient balance.


## Smart Contract Details

### Functions

 **Constructor:**
   - Initializes the token with the name "PlatinumToken" and the symbol "MNT."
   - Sets the deployer address as the owner of the contract.

 **Mint Tokens:**
   - Function: `mintTokens(address recipient, uint256 amount) external onlyOwner`
   - Allows the owner to mint a specified amount of tokens and send them to a designated recipient.

 **Burn Tokens:**
   - Function: `burnTokens(uint256 amount) external`
   - Enables token holders to burn a specified amount of their own tokens, reducing the total supply.

 **Transfer Tokens:**
   - Function: `transferTokens(address to, uint256 amount) public returns (bool)`
   - Standard ERC-20 transfer function, allowing token holders to send tokens to other addresses.

### Modifiers

 **onlyOwner:**
   - Ensures that only the owner of the contract can execute specific functions, such as minting tokens.


## License

This smart contract is released under the MIT License. See the SPDX-License-Identifier tag in the contract source code for details.
