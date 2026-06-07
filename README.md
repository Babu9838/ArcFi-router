# ArcFi-router
ArcFi - Smart value router MVP on Arc. A simple web app that routes transaction accross chain. 
 Arc Multi-Chain Web3 App — FULL FEATURE LIST + STRUCTURE
⚡ 1. Core Features (Main App)
🔌 Wallet Connect (MetaMask / EVM wallets)
🔗 Auto Chain Detection
🔁 Chain Switch
Sepolia Testnet
Arbitrum Sepolia
Arc Testnet (future ready)
💰 Real Balance Check
ETH balance
USDC balance
EURC balance
cirBTC (if available)
💸 Send Transaction
ETH transfer
USDC transfer
EURC transfer
cirBTC transfer (if supported)
📊 Transaction Hash Display
📜 Basic Transaction History (optional extension)
🌉 2. Cross-Chain Features
Bridge System (hook ready)
Sepolia → Arc Testnet
Arbitrum → Arc Testnet
CCTP / Circle Bridge integration ready
Cross-chain transfer UI
🔄 3. Swap System
Token Swap UI
Swap logic hook
Ready for:
Uniswap Router
1inch API
Multi-token support:
USDC
EURC
cirBTC (future)
🔐 4. Social / Identity Features
Wallet Signature Login (SIWE)
Social Connect (Web3 login)
Signed message authentication
Session-based login state
🔗 5. Network / RPC Layer
Arc Testnet RPC
Sepolia RPC
Arbitrum Sepolia RPC
WebSocket support (optional)
Chain ID handling
💳 6. Token Layer
USDC contract integration
EURC contract integration
cirBTC placeholder support
ERC20 balance reader
ERC20 transfer logic (approve + transfer)
🧠 7. SDK / Protocol Layer (Future Ready)
Arc Unified Balance SDK
Arc Bridge SDK
Fee estimation API
Cross-chain settlement logic
🖥️ 8. UI / Dashboard Features
Wallet status panel
Chain display panel
Balance dashboard
Send form UI
Swap panel UI
Bridge panel UI
Transaction hash viewer
📁 9. Recommended Project Structure

arc-web3-dapp/
│
├── public/
│   └── index.html
│
├── src/
│   ├── config/
│   │   ├── chains.js
│   │   ├── tokens.js
│   │   ├── rpc.js
│   │
│   ├── wallet/
│   │   ├── connect.js
│   │   ├── switchChain.js
│   │   ├── signIn.js
│   │
│   ├── balance/
│   │   ├── ethBalance.js
│   │   ├── tokenBalance.js
│   │
│   ├── transfer/
│   │   ├── sendEth.js
│   │   ├── sendToken.js
│   │
│   ├── bridge/
│   │   ├── bridge.js
│   │
│   ├── swap/
│   │   ├── swap.js
│   │
│   ├── transactions/
│   │   ├── txHash.js
│   │   ├── history.js
│   │
│   ├── ui/
│   │   ├── dashboard.js
│   │   ├── render.js
│   │
│   ├── app.js
│
├── assets/
│   ├── style.css
│
├── README.md
🔥 10. Architecture Flow
UI (Dashboard) ↓
app.js (main controller) ↓
wallet / balance / transfer / swap / bridge modules ↓
ethers.js / SDK calls ↓
RPC endpoints ↓
Blockchains (Sepolia / Arbitrum / Arc)
