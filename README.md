# Token_contract
A simple token system where tokens can be minted and burned

This Solidity contract, titled "MyToken," creates a basic token system. It stores details like the token's name, abbreviation, and total supply. Users can mint new tokens, increasing the total supply and their balance. They can also burn tokens, ensuring sufficient balance before reducing both the total supply and their own balance. However, it lacks functionalities like transfer between addresses and advanced access control, making it suitable for educational purposes but not a fully fledged real world token.

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


Deploy MyToken: Compile and deploy the contract to a blockchain network. This creates the token and assigns a contract address.

Mint Tokens: Call the mint function with a recipient address and amount. This increases the total supply and credits the recipient.

View Balances: Check the balances mapping for any address to see their token holdings.

Burn Tokens: Call the burn function with an address and amount. This reduces the total supply and the address's balance (if sufficient).

Limitations: This is a basic example. It lacks transfer functionality and advanced access control.

Real World Use: This serves as a learning tool, but real-world tokens would have more features and security measures.
