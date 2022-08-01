# Transfer ERC20

Network: Goerli

Contract: 0x143492ee98B514b07754e36aDA35Bc0E0b756009

Website: https://leon-do.github.io/transfer-erc20-html/


```solidity
// SPDX-License-Identifier: MIT

pragma solidity ^0.8.0;

import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol";

contract PublicMint20 is ERC20 {
    constructor() ERC20("Rink20", "RNK20") {
    }

    function publicMint() public {
        _mint(msg.sender, 99 * (10**18));
    }
}
```
