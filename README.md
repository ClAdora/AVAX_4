# DegenToken

DegenToken is an Ethereum ERC20 token contract that allows users to mint, burn, buy food items from a menu, transfer tokens, and keep track of owned food items.

## Features

- Mint and burn tokens by the owner.
- Add food items to the menu with prices and available servings.
- Buy food items using tokens, which burns the tokens and reduces available servings.
- Transfer tokens between addresses.
- Keep track of owned food items for each user.

### Interacting with the Contract

- `mint(uint256 amount)`: Allows the owner to mint new tokens.
- `burn(uint256 amount)`: Allows any address to burn their own tokens.
- `addMenu(string memory foodName, uint256 price, uint256 servings)`: Allows the owner to add food items to the menu.
- `orderFood(string memory foodName)`: Allows any address to buy a food item from the menu, burning tokens and reducing available servings.
- `transferTokens(address to, uint256 amount)`: Allows any address to transfer tokens to another address.
- `userOwnedFood(address owner, string memory foodName)`: Returns the quantity of a specific food item owned by an address.
