# RedBelly </br>

## **Token Contract Documentation** </br>

**Contract Address:** `0xfea6cf4cd4072d4f9238327ce4ea5ce59d7460e0` </br>

**Token Name :** `Dogecoin`  </br>

**Token Symbol :**  `DOGE` </br>

[Open Remix](https://remix.ethereum.org/) and click on the `New File`

Name your file, in our case we've named it `Dogecoin.sol`


Now add code. 

pragma solidity 0.8.17;

 // SPDX-License-Identifier: MIT

 contract Bustaaal { string public name = "Dogecoin"; string public symbol = "DOGE"; uint8 public decimals = 18; uint256 public totalSupply = 100000000;

 mapping (address => uint256) public balances; address public owner;

 constructor() { owner = msg.sender; balances[owner] = totalSupply; }

 function transfer(address recipient, uint256 amount) public { require(balances[msg.sender] >= amount, "Insufficient balance."); balances[msg.sender] -= amount; balances[recipient] += amount; } }


On the left sidebar, you will click on Solidity compiler and Compile Redbelly.sol

```text
Solidity Compiler >>> Compile Contract
```

Now click to the `Deploy & Run Transactions` on the left in the sidebar and open Metamask to check if is our account connected.

 successfully deployed.


