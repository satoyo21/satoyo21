// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
import "@openzeppelin/contracts/access/Ownable.sol";

contract Zonic is ERC20, Ownable {
    uint256 private constant _initialSupply = 21000000 * (10 ** 18);

    constructor() ERC20("Zonic", "Zc") {
        _mint(msg.sender, _initialSupply);
    }
}
