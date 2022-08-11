# Transfer ERC20

Network: Goerli, Rinkeby

Contract: 0x8a9f58dea0cf3d92dd8963f5a0a4c7aa9fa76642

Website: https://leon-do.github.io/transfer-erc20-html/


```solidity
// SPDX-License-Identifier: MIT

pragma solidity ^0.8.0;

import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol";

contract PublicMint20 is ERC20 {
    constructor() ERC20("Test20", "TEST20") {
    }

    function publicMint() public {
        _mint(msg.sender, 99 * (10**18));
    }
}
```
