# SimpleToken

This is a simple ERC20 token smart contract implemented using Solidity. The contract uses OpenZeppelin's ERC20 implementation.

## Reading

At the top of the contract, we have the SPDX license identifier for specifying the license under which the code is released.

## Code

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.9;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract SimpleToken is ERC20 {
    constructor() ERC20("YashToken", "YD") {
        _mint(msg.sender, 100 * 10 ** decimals());
    }
}
```

## Requirements

- Remix IDE (https://remix.ethereum.org/)

## Setup and Deployment in Remix

1. Open [Remix IDE](https://remix.ethereum.org/).

2. Create a new file named `SimpleToken.sol` and paste the above code into the file.

3. Navigate to the "Solidity Compiler" tab and select the appropriate compiler version (`0.8.9`). Click on "Compile SimpleToken.sol".

4. Once compiled, navigate to the "Deploy & Run Transactions" tab.

5. Select the environment (e.g., JavaScript VM, Injected Web3 for MetaMask, etc.).

6. Ensure the contract to deploy is selected (`SimpleToken`).

7. Click on "Deploy".

## Owner

Yash Dhiman
