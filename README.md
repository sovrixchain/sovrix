# Sovrix (SVX)

**Sovrix (SVX)** is a next-generation, community-driven cryptocurrency designed for speed, security, and true decentralization.  
Built as a fork of Litecoin, Sovrix introduces a **fixed supply of 12.5 million SVX**, with **block reward halving every 6 months**, ensuring long-term scarcity and sustainable value.

---

## 🔹 Features

- **Total Supply:** 12,500,000 SVX (fixed, no inflation)
- **Halving Schedule:** Block rewards halve every 6 months
- **Consensus:** Proof-of-Work (Scrypt-based mining)
- **Fair Launch:** No premine, no ICO, no VC allocations
- **Governance:** Community-powered DAO (Sovrix DAO)
- **Cross-Platform Support:** Windows, Linux, macOS (binaries + build from source)
- **Mobile Mining:** Android GUI app (in development)

---

## 🔹 Roadmap

- ✅ Core Sovrix blockchain (Litecoin fork with new parameters)
- ✅ Wallets & Daemon (CLI + Qt GUI)
- 🔄 GUI Wallet with integrated miner
- 🔄 Android mining app with user-friendly interface
- 🔄 DAO Governance (Snapshot + smart contract integration)
- 🔄 Cross-chain bridge for wrapped SVX (wSVX)

---

## 🔹 Building From Source

### Linux / macOS
```bash
git clone https://github.com/sovrix360/sovrix.git
cd sovrix
./autogen.sh
./configure
make -j$(nproc)
Windows (MSYS2 / MinGW)
Install MSYS2

Install dependencies:

bash
Copy code
pacman -S mingw-w64-x86_64-toolchain autoconf automake libtool make git
Clone & build:

bash
Copy code
git clone https://github.com/sovrix360/sovrix.git
cd sovrix
./autogen.sh
./configure
make -j4
🔹 Usage
Start Sovrix daemon:

bash
Copy code
./src/sovrixd -daemon
Command-line wallet:

bash
Copy code
./src/sovrix-cli getnewaddress
Run the Qt GUI wallet:

bash
Copy code
./src/qt/sovrix-qt
🔹 Mining
Sovrix uses Scrypt for mining.

CPU Mining
bash
Copy code
./src/sovrixd setgenerate true
GPU Mining
Use external Scrypt miners such as cgminer or cpuminer, pointing to your Sovrix node.

Example:

bash
Copy code
cgminer -o http://127.0.0.1:9332 -u rpcuser -p rpcpassword --scrypt
🔹 Governance (Sovrix DAO)
DAO voting via wrapped SVX (wSVX) on Ethereum

Community proposals hosted on Snapshot.org

Treasury managed via Gnosis Safe (multisig) → migrating to on-chain DAO contracts

🔹 Contributing
We welcome contributors!

Fork the repo

Create a feature branch

Submit a Pull Request

Please open an Issue to report bugs, request features, or discuss improvements.

🔹 Community
🌍 Website: [Coming Soon]

🐦 Twitter: @sovrix

💬 Telegram: t.me/sovrixdao

💻 GitHub: github.com/sovrixchain

📜 License
Sovrix is released under the MIT License – free and open-source forever.
