# Solidity Program: MyToken

This is a Solidity smart contract that implements a basic token named MyToken (META) with functionalities for minting and burning tokens.

## Requirements

1. The contract has public variables to store the details of the token, including its name, abbreviation, and total supply.
2. A mapping is used to track the token balances of different addresses (address => uint).
3. The contract includes a mint function that takes an address and a value as parameters. It increases the total supply by the specified value and adds that value to the balance of the sender's address.
4. The contract also includes a burn function that works  the exact opposite way of the mint function. It takes an address and a value as parameters, deducts the value from the total supply, and reduces the balance of the sender's address accordingly.
5. The burn function includes conditionals to ensure that the balance of the sender is greater than or equal to the amount to be burned.

## Usage

1. tokenName: It is a public variable that represents the name of the token.It is set as "KILLDILL" in this contract.
2. tokenAbbrev: It is a public variable that represents the abbreviation of the token.It is set to "KDL" in this contract.
3. totalSupply: It is a public variable that represents the total supply of the token. Initially it is set to 0, it increases when tokens are minted and decreases when tokens are burned.
4. balances: A mapping that associates addresses with token balances. Each address's balance is stored as a positive integer.
5. mint: A function that mints new tokens. It takes an address (_address) and a value (_value) as parameters. It increases the total supply by the specified value and adds that value to the balance of the specified address.
6. burn: A function that burns existing tokens. It takes an address (_address) and a value (_value) as parameters. If the balance of the specified address is greater than or equal to the value, it deducts the value from the total supply and reduces the balance of the specified address.

Please note that this contract is a basic implementation and may require additional functionality and security measures for use in production environments.

## License

This contract is not licensed.
