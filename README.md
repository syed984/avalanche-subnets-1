# Vault and ERC20 

## Summary

Welcome to the repository containing the Solidity contracts for the Vault and ERC20 Token. This collection includes two robust contracts: `Vault` and `ERC20`. The `Vault` contract facilitates decentralized management of ERC20 tokens in a secure vault setting, while the `ERC20` contract implements the ERC20 standard with additional features for minting and burning tokens.

## Vault Contract

### Overview

The `Vault` contract functions as a secure decentralized vault, allowing users to deposit and withdraw ERC20 tokens. It handles total supply and individual user balances efficiently, enabling seamless interaction with assets.

### Key Features

- **Deposit Functionality**: Users can deposit ERC20 tokens into the vault, receiving shares proportional to their contribution.

- **Withdrawal Functionality**: Users can withdraw tokens by burning their shares, receiving a proportionate amount.

### Internal Mechanics

- **Minting Function (`_mint`)**: Privately mints shares, updating total supply and user balances accordingly.

- **Burning Function (`_burn`)**: Privately burns shares, adjusting total supply and user balances.

### Events

- **Transfer Event**: Triggered when tokens are transferred within the vault.

### Usage Guidelines

1. Deploy the `Vault` contract by specifying the ERC20 token address in the constructor.

2. Users can interact with the contract by depositing and withdrawing tokens seamlessly.

## ERC20 Contract

### Overview

The `ERC20` contract is a comprehensive implementation of the ERC20 standard, enhancing basic functionalities with additional minting and burning capabilities. Users can transfer tokens, grant approval for spending, and execute transfers on behalf of others.

### Key Features

- **Transfer Functionality**: Allows users to transfer tokens to other addresses.

- **Approval Mechanism**: Permits users to grant approval for spending tokens on their behalf.

- **Minting and Burning Functions**: Provides flexibility in creating and destroying tokens, respectively.

### Events

- **Transfer Event**: Emitted when tokens are transferred.

- **Approval Event**: Emitted when approval is granted for spending tokens.

### Usage Guidelines

1. Deploy the `ERC20` contract to create a new ERC20 token.

2. Utilize standard ERC20 functions, including transferring, approval for spending, and minting/burning tokens.

## Author 

Syed owaiz

owaiz9866@gmail.com

## License

Both contracts are licensed under the MIT License.
