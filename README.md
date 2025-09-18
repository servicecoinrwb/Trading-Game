On-Chain Trading Game dApp

A decentralized trading simulation game built on the Base blockchain.
Players connect their crypto wallets and practice leveraged trading with virtual funds in a fully on-chain environment.

🎮 Core Features

Connect Wallet
Seamless integration with browser wallets like MetaMask.

Virtual Balance
Each new player receives 10,000 vUSD (virtual USD) to trade with.

Leveraged Trading
Open long or short positions with user-defined margin and leverage.

On-Chain Settlement
All trades are executed and resolved by a Solidity smart contract, ensuring fairness and transparency.

Manual Trade Management
Players can close their open positions at any time before liquidation or target hit.

🛠️ Technology Stack

Smart Contracts: Solidity

Frontend: HTML, CSS, JavaScript with ethers.js

Blockchain: Base (EVM-compatible)

⚙️ How It Works

The system has two main components:

TradingGame.sol (Smart Contract)

Manages player registration

Tracks virtual balances

Enforces trading rules

Processes trade openings, closures, and outcomes

Uses an Oracle address to inject real-world price data for trade resolution

trading-dapp.html (Frontend)

Web interface for players

Wallet connection and registration

Simple forms for opening and closing trades

Sends transactions directly to the contract

🔮 Oracle Integration

Trades reference real asset prices (e.g., BTC/USD).

An Oracle address pushes price updates to the smart contract.

Stop Loss / Take Profit levels are resolved trustlessly on-chain.

🚀 Getting Started
Prerequisites

Browser wallet (MetaMask or similar)

RPC endpoint for Base (Infura / Alchemy)

Testnet ETH on Base Sepolia for deployment

Deploy the Smart Contract

Compile TradingGame.sol in Remix or Hardhat

Deploy to Base or Base Sepolia

Copy the contract address and ABI

Configure the Frontend

Open trading-dapp.html

Paste contract address + ABI in the <script> section

Save and reload

Launch

For local testing: open trading-dapp.html in your browser

For public hosting: deploy to GitHub Pages, Vercel, or Netlify

📖 Gameplay

Connect your wallet

Click Register to mint 10,000 vUSD

Choose your trade parameters:

Asset (BTC/ETH mock pairs)

Position (long or short)

Margin size

Leverage

Stop Loss / Take Profit

Confirm in your wallet

Monitor or close your position manually

🧱 Roadmap

✅ Core virtual trading contract

✅ Frontend wallet connection

⏳ Oracle integration for live price feeds

⏳ Leaderboard with on-chain scores

⏳ NFT badges for milestones (e.g., first profit, best win streak)

⏳ DAO-style governance for rule changes
