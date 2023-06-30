# MyToken
This Solidity contract provides a basic implementation of a token contract with two functions i.e. mint and burn. This allows the users to create and destroy tokens, while maintaining the total supply and individual balances of the individuals.

## Requirements
This contract is designed to complete the requirements mentioned below-

1. Token Details: This contract uses some variables with public access specifiers to store the information about the token. These variables are- token_name, token_abbreviation and total_supply.

2. Balances addressing: In this contract we are using a mapping named as 'balances' to map address to their token balance.

3. Mint Function: This function has two parameters- an address and a value. This function increases the total token supply the the value given in parameter and then update the balance of the sender's address accordingly.

4. Burn Function: This function also uses two parameters same as the mint function but it work opposite to the mint function. This function is used to burn or destroy the total supply by  the given value and update the balance of the individual accordingly.

5. Condition check: With this condition we are allowing the 'burn' function to burn the token if the sender's balance is greater than or equals to the amount of tokens to be burned. 
   
## Usage
   1. Deploy the MyToken contract on  Ethereum Virtual Machine (EVM) having the compatible version(0.8.18).

   2. We can use the two functions for interacting with the contract:
      
       -`mint(address _add, uint _val):` here the '_add' parameter is denoting the recipient's address and the '_val' parameter represents the token amount to be mint. This function increases or mint new tokens with given value by increasing the total supply and the balance at the particular address.

       -`burn(address _add, uint _val):` here the '_add' parameter is denoting the sender's address and the '_val' parameter represents the token amount to be burn. The function burn the tokens from the total supply and also deduct the balance of the sender's address. Also it uses a condition to do so, if the sender's balance is below the need, an error message is returned.

   3. We can access the public variables:

    token_name: Retrieves the name of the token.
    token_abbreviation: Retrieves the abbreviation of the token.
    total_supply: Retrieves the total supply of the token.

## License
This project is licensed under the MIT License. You can find this in the code as "SPDX-License-Identifier: MIT" with a comment(//) ahead  in the first line of code.
