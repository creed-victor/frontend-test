# Web3.js Frontend Dev Assignment
Assignment is to create simple Ethereum Dapp using `typescript` and `react.js` which allows users to check their Weenus Token balance and send some of it to another wallet.

### 1. Preparations
- Install and setup [MetaMask](https://metamask.io/download.html) extension to your browser.
- Switch your MetaMask network from Ethereum Mainnet to `Ropsten Test Network`.
- Retrieve some of rETH to your MetaMask address from [this faucet](https://faucet.dimensions.network).
- Add/Start tracking `Weenus Token` in your MetaMask wallet. Weenus Token address is [0x101848D5C5bBca18E6b4431eEdF6B95E9ADF82FA](https://ropsten.etherscan.io/address/0x101848D5C5bBca18E6b4431eEdF6B95E9ADF82FA#code)
- Read Help section if you havent worked with blockchain & ethereum before, try to deliver code even if it fails or is not finished.

### 2. Assignment

- Create react.js project, no actual design or styling is required.
- Ask user to connect to MetaMask wallet once app is loaded or by clicking some button (choose one).
- If user is not yet connected to metamask - show "connect to metamask" message and button to connect if you choose to implement it.
- If user is connected to metamask, using web3.js:
  * show connected user's rETH balance.
  * show connected user's Weenus Token balance.
  * add form with two inputs - amount and receiver address, submiting form should initiate token transfer from your metamask wallet to receiver wallet. You can use `0x0000000000000000000000000000000000000000` wallet as receivers.
  * show pending transaction hash when form is submitted.
- *Bonus points for updating user balance without refresh page.*
- *Bonus points for checking and updating transaction status (pending, completed, failed).*
- Provide your source code as github / bitbucket repository.


To work with Weenus Token you will need contract jsonInterface, it's added to this repository as [./WeenusTokenABI.json](./WeenusTokenABI.json)
Weenus Token contract address: `0x101848D5C5bBca18E6b4431eEdF6B95E9ADF82FA`

! Weenus Token balance is shown with 18 decimals (1000000000000000000 returned from contract is equal 1 Weenus Token you would see in your metamask wallet)

## Help

- [Documentation on how to interacting with Smart-Contracts using web3.js](https://web3js.readthedocs.io/en/v1.3.0/web3-eth-contract.html)
- [How to Install and Use Metamask?](https://blog.wetrust.io/how-to-install-and-use-metamask-7210720ca047)
- [How to Connect Web3.js to MetaMask?](https://medium.com/@awantoch/how-to-connect-web3-js-to-metamask-in-2020-fee2b2edf58a)
- [Interacting with a Smart Contract through Web3.js](https://medium.com/@yangnana11/interacting-with-a-smart-contract-through-web3-js-tutorial-56a7ff2ff153)
