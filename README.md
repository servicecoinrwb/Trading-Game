On-Chain Trading Game dApp
A decentralized trading simulation game built on the Base blockchain. This dApp allows users to connect their crypto wallets and practice trading with virtual funds in an on-chain environment.

!

Core Features
Connect Wallet: Integrates with browser wallets like MetaMask.

Virtual Balance: Players can register to receive 10,000 virtual USD to trade with.

Leveraged Trading: Open long or short positions with user-defined margin and leverage.

On-Chain Settlement: All trades are opened and resolved via a Solidity smart contract, acting as a trustless referee.

Manual Trade Management: Players can request to close their active positions at any time.

Technology Stack
Smart Contract: Solidity

Frontend: HTML, CSS, JavaScript (using the ethers.js library)

Blockchain: Base (or any EVM-compatible chain)

How It Works
The project consists of two main components:

TradingGame.sol (The Smart Contract): This is the backend logic that lives on the blockchain. It manages player registration, virtual balances, and the rules for opening and resolving trades. It acts as the single source of truth for the game.

trading-dapp.html (The Frontend): This is the user interface. It allows players to interact with the smart contract by connecting their wallets and sending transactions to register, open trades, and close trades.

Trade resolution is handled by a designated Oracle address, which is responsible for pushing real-world price data to the smart contract to determine if a trade's Stop Loss or Take Profit has been hit.

Getting Started
To run this project locally or deploy it yourself, follow these steps:

Prerequisites:

A browser with a crypto wallet extension (e.g., MetaMask).

An RPC endpoint for the Base network (e.g., from Infura or Alchemy).

Testnet ETH on Base Sepolia for deployment fees.

Deploy the Smart Contract:

Compile TradingGame.sol using a development environment like Remix or Hardhat.

Deploy the compiled contract to the Base network.

Copy the deployed contract's address and its ABI.

Configure the Frontend:

Open trading-dapp.html.

Paste the contract address and ABI into the placeholder variables in the <script> section.

Launch:

For local testing, simply open the trading-dapp.html file in your browser.

For public access, host the HTML file (e.g., using GitHub Pages).

Play:

Connect your wallet.

Click "Register" to get your virtual funds.

Enter your trade parameters and open a position!
