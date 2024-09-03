# divneetburnmint Smart Contract

This repository contains the divneetburnmint smart contract written in Solidity. The contract is designed to handle the minting and burning of tokens, with functionalities to manage token balances and total supply.

## Contract Overview

- *Token Name*: divneettoken
- *Token Abbreviation*: DVT
- *Initial Total Supply*: 1,313 DVT

## Features

- *Minting Tokens*: Increase the balance of a specified address by minting new tokens.
- *Burning Tokens*: Reduce the balance of a specified address by burning tokens, thereby decreasing the total supply.

## State Variables

- *tokenName*: The name of the token, set to divneettoken.
- *tokenAbbr*: The abbreviation of the token, set to DVT.
- *totalSupply*: The total supply of tokens, initially set to 1,313.

## Mappings

- *balances*: A mapping that tracks the token balance of each address.

## Functions

### mint(address addr, uint amount) external

This function allows the minting of new tokens. It increases the balance of the specified address (addr) by the amount (amount) and also updates the total supply accordingly.

*Parameters:*
- addr: The address to which the tokens will be minted.
- amount: The number of tokens to be minted.

### burn(address addr, uint amount) external

This function allows the burning of tokens. It decreases the balance of the specified address (addr) by the amount (amount) and updates the total supply if the balance and total supply conditions are met.

*Parameters:*
- addr: The address from which the tokens will be burned.
- amount: The number of tokens to be burned.

*Conditions:*
- The balance of the specified address must be greater than or equal to the amount to be burned.
- The total supply must be greater than the amount to be burned.

## Example Usage

### Minting Tokens
mint(0xYourAddressHere, 100);
This command will mint 100 DVT tokens to the specified address and increase the total supply by 100.

### Burning Tokens

burn(0xYourAddressHere, 50);
This command will burn 50 DVT tokens from the specified address, reducing the total supply by 50.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

### Contributing
Contributions are welcome! Please open an issue or submit a pull request if you have any improvements or new features to add.

### Contact
For any questions or inquiries, feel free to reach out via Email.

Thank you for using the divneetburnmint smart contract. We hope it meets your needs!
