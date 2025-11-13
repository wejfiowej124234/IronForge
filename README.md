# IronForge

A web-based cryptocurrency wallet built with Rust and WebAssembly.

## Overview

IronForge is a non-custodial wallet that runs directly in web browsers using WebAssembly technology. It provides basic cryptocurrency management functionality without requiring software installation.

## Features

- **Browser-Based**: Runs in Chrome, Firefox, Safari, and other modern browsers
- **Non-Custodial**: Private keys stored locally in browser storage
- **Multi-Chain**: Support for Ethereum, BSC, Polygon, and testnets
- **Transaction Management**: Send, receive, and track transactions
- **Wallet Import/Export**: Compatible with BIP39 mnemonic phrases
- **No Installation**: Access directly via web browser

## Technology Stack

- **Frontend**: Rust + Dioxus Web
- **Runtime**: WebAssembly (WASM)
- **Storage**: IndexedDB with encryption
- **Backend**: Connects to [Rust-Blockchain-Secure-Wallet](https://github.com/DarkCrab-Rust/Rust-Blockchain-Secure-Wallet)

## Supported Networks

- Ethereum Mainnet
- Polygon Mainnet
- BSC Mainnet
- Sepolia Testnet
- BSC Testnet

## Usage

### Online (Coming Soon)
Visit https://ironforge.io to use the application.

### Local Development

```bash
# Install Rust
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

# Install Trunk
cargo install trunk

# Add WASM target
rustup target add wasm32-unknown-unknown

# Clone and run
git clone https://github.com/DarkCrab-Rust/IronForge.git
cd IronForge
trunk serve --open
```

## Security Considerations

- Private keys stored in browser's IndexedDB
- Encrypted with AES-256-GCM
- Keys never transmitted to servers
- Users responsible for backing up mnemonics
- Recommend using hardware wallets for large amounts

## Project Structure

```
IronForge/
├── src/
│   ├── components/     # UI components
│   ├── services/       # Blockchain services
│   ├── crypto/         # Cryptography utilities
│   └── storage/        # Browser storage
├── Cargo.toml
└── Trunk.toml
```

## Backend Integration

Connects to existing Rust backend API:
- API Repository: [Rust-Blockchain-Secure-Wallet](https://github.com/DarkCrab-Rust/Rust-Blockchain-Secure-Wallet)
- 46 API endpoints
- 348 test cases

## Ecosystem

Part of the DarkCrab-Rust wallet ecosystem:

- **Web Wallet**: IronForge (this project)
- **Mobile Wallet**: [IronLink-DApp](https://github.com/DarkCrab-Rust/IronLink-DApp)
- **Backend API**: [Rust-Blockchain-Secure-Wallet](https://github.com/DarkCrab-Rust/Rust-Blockchain-Secure-Wallet)
- **Previous Web UI**: [blockchain-wallet-ui](https://github.com/DarkCrab-Rust/blockchain-wallet-ui) (React version)

## Development Status

Currently in early development. Not recommended for production use with real funds.

## License

MIT License - see [LICENSE](LICENSE) for details

## Contributing

Contributions welcome via pull requests. Please follow Rust coding standards and include tests.

## Contact

- Issues: https://github.com/DarkCrab-Rust/IronForge/issues
- Repository: https://github.com/DarkCrab-Rust/IronForge

## Disclaimer

This is experimental software. Users are responsible for securing their private keys and mnemonic phrases. The developers assume no liability for any losses. Use at your own risk.
