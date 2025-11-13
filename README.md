# IronForge - Web Wallet

> 🌐 Browser-based cryptocurrency wallet built with Rust and WebAssembly

---

## 🌐 Iron Blockchain Wallet Ecosystem

| # | Project | Description | Repository |
|---|---------|-------------|------------|
| 1️⃣ | **IronCore** | 🎯 钱包后端 - Backend API Server | [→ Visit](https://github.com/wejfiowej124234/IronCore) |
| 2️⃣ | **IronForge** | 🌐 前端钱包 - Web Wallet | 👉 **[You are here]** |
| 3️⃣ | **IronLink-DApp** | 📱 移动端 - Mobile DApp Wallet | [→ Visit](https://github.com/wejfiowej124234/IronLink-DApp) |
| 4️⃣ | **IronGuard-AI** | 🤖 AI安全 - AI Security Layer | [→ Visit](https://github.com/wejfiowej124234/ironguard-ai) |
| 5️⃣ | **IronVault-XR** | 🥽 智能眼镜 - AR/VR Wallet | [→ Visit](https://github.com/wejfiowej124234/IronVault-XR) |
| 6️⃣ | **Attack-Defense** | ⚔️ 攻防知识库 - Security Knowledge Base | [→ Visit](https://github.com/wejfiowej124234/Attack-Defense) |

---

## 🏆 核心特性

<div align="center">

| 🦀 Rust 全栈 | 🔓 非托管架构 | 🏢 企业级 API |
|:----------:|:------------:|:------------:|
| **100% Rust** 前后端 | 私钥永不上传 | IronCore 46+ 端点 |
| WASM 接近原生性能 | 用户完全掌控 | 99.9% SLA 保证 |
| 内存安全编译时保证 | 硬件隔离存储 | 审计日志 + 监控 |

</div>

---

## Overview

IronForge is a **100% Rust-powered, non-custodial** Web wallet that runs in browsers via WebAssembly. Built on enterprise-grade IronCore API, it delivers native performance with maximum security.

### Why IronForge?

- 🦀 **Full-Stack Rust**: Frontend (WASM) + Backend (IronCore), 95%+ code reuse
- 🔓 **Non-Custodial**: You control your private keys, always. We never touch them.
- 🏢 **Enterprise Backend**: 99.9% SLA, monitoring, audit logs, multi-chain support

## Features

- **Browser-Based**: Runs in Chrome, Firefox, Safari, and other modern browsers
- **Non-Custodial**: Private keys stored locally in browser storage
- **Multi-Chain**: Support for Ethereum, BSC, Polygon, and testnets
- **Transaction Management**: Send, receive, and track transactions
- **Wallet Import/Export**: Compatible with BIP39 mnemonic phrases
- **No Installation**: Access directly via web browser
- **WASM Performance**: Native-like performance in the browser

## Technology Stack

- **Frontend**: Rust + Dioxus Web
- **Runtime**: WebAssembly (WASM)
- **Storage**: IndexedDB with AES-256-GCM encryption
- **Backend**: Connects to [IronCore](https://github.com/wejfiowej124234/IronCore)

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
git clone https://github.com/wejfiowej124234/IronForge.git
cd IronForge
trunk serve --open
```

## Security Considerations

- Private keys stored in browser's IndexedDB
- Encrypted with AES-256-GCM
- Keys never transmitted to servers
- Users responsible for backing up mnemonics
- Recommend using hardware wallets for large amounts
- Integration with [IronGuard-AI](https://github.com/wejfiowej124234/ironguard-ai) for threat detection

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

Connects to IronCore backend API:
- API Repository: [IronCore](https://github.com/wejfiowej124234/IronCore)
- 46+ API endpoints
- 900+ test cases
- 95%+ test coverage

## Development Status

Currently in early development. Not recommended for production use with real funds.

## License

MIT License - see [LICENSE](LICENSE) for details

## Contributing

Contributions welcome via pull requests. Please follow Rust coding standards and include tests.

## Contact

- Issues: https://github.com/wejfiowej124234/IronForge/issues
- Repository: https://github.com/wejfiowej124234/IronForge

## Disclaimer

This is experimental software. Users are responsible for securing their private keys and mnemonic phrases. The developers assume no liability for any losses. Use at your own risk.

---

**Built with ❤️ using Rust + WebAssembly**
