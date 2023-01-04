## How to create your own token on Binance

MyToken.sol will have the following code and we will use the OpenZeppelin library, a smart contract template library, to write our smart contract and as you can see, we wrote only 5-6 lines to make our token!

We will use Remix IDE to write and deploy our smart contract.

```
// SPDX-License-Identifier: GPL-3.0
pragma solidity >=0.7.0 <0.9.0;
import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
contract MyToken is ERC20 {
constructor () ERC20("Dragon Coin", "Dragon") {
_mint(msg.sender, 1000000 * 10 ** decimals());
}
}
```
You can change Dragon Coin and Dragon with the name of your token and symbol.


