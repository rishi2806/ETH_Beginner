# ETH-Beginner
## MyToken
This is a simple ERC-20 token contract implemented in Solidity. The contract allows for the creation and destruction of tokens, as well as storing information about the token.

## Requirements
1. The contract has three public variables that store the details about the token:

      tokenName: A string represents the name of the token.

      abbrv: A string represents the abbreviation of the token.

      totalSupply: An unsigned integer that represents the total supply of the tokens.

2. The contract has a mapping of addresses to the balances:

      balances: This is a mapping that associates addresses with their corresponding token balances.

3. The contract has a mint function that increases the total supply and the balance of the "sender" address by a given value:

    Parameters:

        _add: The address to which the tokens will be minted.

        _val: The amount of tokens to be minted.

    Results:

        Increase the totalSupply by _val.

        Increase the balance of the _add by _val.

4. The contract has a burn function that decreases the total supply and the balance of the "sender" address by a given value:

    Parameters:

        _address: The address from which the tokens will be burned.

        _value: The amount of tokens to be burned.

    Results:

        Check if the balance of the _add is greater than or equal to _val.

        If true, decrease the totalSupply by _val.

        Decrease the balance of the _add by _val.
## Usage
1. Deploy the MyToken contract to the supported Ethereum network.

2. Once deployed, you can interact with the contract by calling the functions below:

    mint: This function is used to create new tokens and assigns them to a specified address.

    Parameters:

       _add: The address to which the tokens will be minted.
  
       _val: The amount of tokens to be minted.

    burn: This function is used to destroys or decrement the existing tokens by reducing the total supply and the balance of a specified address.

    Parameters:
   
        _add: This parameter is used to fetch the address from which the tokens will be burned.

        _val: This paramater is used for the amount of tokens to be burned.
## License
    This contract is licensed under the MIT License- "SPDX-License-Identifier: MIT".
