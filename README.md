# Token_contract
A simple token system where tokens can be minted and burned

This Solidity contract, titled "MyToken," creates a basic token system. It stores details like the token's name, abbreviation, and total supply. Users can mint new tokens, increasing the total supply and their balance. They can also burn tokens, ensuring sufficient balance before reducing both the total supply and their own balance. However, it lacks functionalities like transfer between addresses and advanced access control, making it suitable for educational purposes but not a fully fledged real world token.

# DESCRIPTION
This code serves as a blueprint for a simple digital token system on the blockchain. Consider a bag (the contract) containing unique digital items known as "Seth_ken" tokens (identified by "Seth"). The code keeps track of the total number of tokens created (similar to how many items are in the bag). It also keeps track of who has how many "Seth_ken" tokens (similar to who has what items in the bag). Anyone can add more tokens to the bag, but removing them requires that you already have enough. This is a very basic example, and real systems would have more features and safeguards, but it provides an idea of how blockchain tokens can be managed.

# Getting Started

# EXECUTION

TO run this program you can use Remix, an online Solidity IDE. To get started, go to the remix website at " https://t.ly/BIv2z ". Once you're on the remmix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a.sol extension (e.g., HelloWorld.sol). Copy and paste the follwing code into the file:

// SPDX-License-Identifier: GPL-3.0
pragma solidity >=0.8.0 <0.9.0;

contract MyToken{

    string public TokenName = "Seth_ken";
    string public tokenAbbrv = "Seth";
    uint public TotalSupply;

    mapping(address => uint) public balances;

    function mint (address _address, uint _value) public {
        TotalSupply += _value;
        balances[_address] += _value;
    }

     function burn (address _address, uint _value) public {
        if (balances[_address] >= _value){
            TotalSupply -= _value;
        balances[_address] -= _value;


        }
    }

}

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.4"(or another compatible version), and then click on the "Compile HelloWorld.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "HelloWorld" cont786xract from the dropdown menu. and then click on the "Deploy" button.

Once the cotract is deployed, you can interact with it by calling the "sayHello" function. Click on the HelloWorld" contract in the left-hand sidebar, and then click on the "sayHello" function.  Finally, click on the "transact" button to execute the function and retrieve the "HelloWorld!" message.

# AUTHORS
SK SAHIL TARAFDAR
@Seth786x

# LICENSE
This project is licensed under the GPL-3.0 License.
