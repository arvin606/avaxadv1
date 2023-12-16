# Vault Smart Contract Readme

This repository contains a simple Ethereum smart contract written in Solidity that represents a basic vault for handling deposits and withdrawals of an ERC-20 token. The vault contract follows the MIT License ([SPDX-License-Identifier: MIT](https://opensource.org/licenses/MIT)).

## Smart Contract Overview

The smart contract consists of two main components: the ERC-20 token interface (`IERC20`) and the `Vault` contract.

### ERC-20 Token Interface (IERC20)

The `IERC20` interface defines standard functions and events for interacting with ERC-20 tokens. It includes methods for checking the total supply, balance of an account, transferring tokens, checking allowances, approving spenders, and transferring tokens on behalf of an owner.

### Vault Contract

The `Vault` contract is designed to handle deposits and withdrawals of an ERC-20 token. It includes the following features:

- **Constructor**: Initializes the contract with the address of the ERC-20 token.

- **Deposit Function**: Allows users to deposit ERC-20 tokens into the vault. The number of shares received is calculated based on the total supply and the amount deposited.

- **Withdraw Function**: Allows users to withdraw ERC-20 tokens from the vault. The amount withdrawn is calculated based on the number of shares burned.

- **Internal Mint and Burn Functions**: Handle the creation and destruction of shares during deposit and withdrawal operations.

