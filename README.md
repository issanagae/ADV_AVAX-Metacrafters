# ADV_AVAX-Metacrafters

### Overview

This contract implements the ERC-20 standard for a fungible token on the Ethereum blockchain. It includes basic functionalities for transferring tokens, approving spending, and handling minting and burning operations.

### Token Details

- **Name:** Solidity by Example
- **Symbol:** SOLBYEX
- **Decimals:** 18

### Functions

- **Transfer**
  ```solidity
  function transfer(address recipient, uint amount) external returns (bool)
  ```
  Transfers `amount` tokens from the caller's address to `recipient`.

- **Approve**
  ```solidity
  function approve(address spender, uint amount) external returns (bool)
  ```
  Approves the spender to spend `amount` tokens on behalf of the caller.

- **TransferFrom**
  ```solidity
  function transferFrom(address sender, address recipient, uint amount) external returns (bool)
  ```
  Transfers `amount` tokens from `sender` to `recipient` using the allowance mechanism.

- **Mint**
  ```solidity
  function mint(uint amount) external
  ```
  Mints new tokens and assigns them to the caller.

- **Burn**
  ```solidity
  function burn(uint amount) external
  ```
  Burns `amount` tokens, reducing the total supply.

### Events

- **Transfer Event**
  ```solidity
  event Transfer(address indexed from, address indexed to, uint value);
  ```
  Emitted when tokens are transferred from one address to another.

- **Approval Event**
  ```solidity
  event Approval(address indexed owner, address indexed spender, uint value);
  ```
  Emitted when the approval of a spender to spend tokens on behalf of the owner occurs.

### License

This contract is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

**SPDX-License-Identifier: MIT**

---

## Vault (Vault.sol)

### Overview

The Vault contract is designed to manage deposits and withdrawals of the ERC-20 token. It calculates shares for deposit and the corresponding amount for withdrawal based on the total supply and token balances.

### Functions

- **Deposit**
  ```solidity
  function deposit(uint amount) external
  ```
  Deposits a specified amount of tokens into the vault, minting shares for the depositor.

- **Withdraw**
  ```solidity
  function withdraw(uint shares) external
  ```
  Withdraws a specified number of shares from the vault, returning the corresponding amount of tokens to the shareholder.

### License

This contract is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

**SPDX-License-Identifier: MIT**
