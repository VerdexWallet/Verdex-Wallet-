Verdex Wallet

The first privacy-focused, multi-chain wallet built entirely on a mobile device.

> Status: Active Development (Alpha)
> Built on: Android (Acode / Spck Editor)
> License: MIT

💡 About
Verdex is a self-custodial cryptocurrency wallet designed to bridge the gap between CEX and DEX tracking without sacrificing user privacy.

Most wallets today are bloated with analytics, third-party trackers, and corporate backdoors. Verdex was built to be the opposite: Lean, Private, and Transparent.

The Origin Story:
This entire project—from the AES encryption logic to the canvas charting engine—was written on a smartphone by a solo developer. No laptop. No VC funding. Just code.

🛠 Tech Stack
- Core: Vanilla JavaScript (ES6+), HTML5, CSS3
- Blockchain: Ethers.js (v5.7.2)
- Cryptography: WebCrypto API (Native Browser Security)
- Charting: Custom HTML5 Canvas Engine (Zero dependencies)

🔒 Security Deep Dive
Verdex does not rely on proprietary backends. Your security is handled entirely client-side using industry-standard cryptography.

1. Military-Grade Encryption
- Key Derivation: Your 6-digit PIN is salted and hashed using PBKDF2 (SHA-256) with 250,000 iterations to prevent brute-force attacks.
- Storage: Private keys and mnemonics are encrypted using AES-GCM (256-bit) before being stored in your device's local storage.
- Zero Knowledge: The app never transmits your keys or seed phrases. They strictly stay on your device.

2. The "Master Loader" Engine
To solve the issue of broken free APIs, Verdex uses a custom aggregation engine:
- Validation: Cross-references token contracts against a "Golden Dictionary" (Uniswap/CoinGecko lists) to flag fake tokens.
- Redundancy: Automatically fails over between Binance, Mobula, and Ethplorer APIs to ensure prices always load.

✨ Key Features
- True Watch-Only Mode: Track any whale wallet or cold storage address without ever inputting a private key.
- Privacy First: No IP tracking, no analytics scripts, no account registration required.
- Smart Import: Supports BIP39 mnemonic phrases (12/24 words) with auto-complete suggestions for safety.
- Visual Trust: Custom-built charting engine that renders price history directly in the app without external widgets.

🚀 Roadmap
- [x] Core Wallet: Creation, Import, and Local Storage
- [x] Transaction Logic: Send/Receive ETH & ERC20 Tokens
- [x] Security: PIN Lock & AES Encryption Implementation
- [ ] In Progress: CoinGecko Pro API Integration (Needs funding)
- [ ] In Progress: Multi-Chain Support (BSC, Base, Solana)
- [ ] Future: Built-in Swap Aggregator

🤝 Support the Build
I am building this with zero funding, fighting against unstable free-tier APIs.
If you want to support open-source, privacy-first tools, please consider donating on Giveth. Your support directly funds the API costs required to keep the data feeds live.

[https://giveth.io/project/verdex-wallet]

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
