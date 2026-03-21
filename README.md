# Amnezia VPN Deployment Suite

This tool automates the deployment of a secure Amnezia VPN server based on `amnezia-wg-easy`.

## 🚀 Quick Start

To run the interactive wizard from any machine with Python 3:

```bash
curl -sSL https://raw.githubusercontent.com/sky-night-net/enl-cdn/main/amnezia-cli.py | python3
```

*Note: The script will automatically install required dependencies (`paramiko`, `bcrypt`).*

## 🛠 Manual Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/sky-night-net/enl-cdn.git
   cd enl-cdn
   ```

2. Run the tool:
   ```bash
   python3 amnezia-cli.py
   ```

## 📖 Features

- **Interactive Wizard**: Step-by-step setup asking for server IP, password, etc.
- **Auto Mode**: Deploy with a single command passing arguments.
- **Cleanup**: Remove existing installations cleanly.
- **High Security**: Pre-configured with "hard" obfuscation for stealth.
- **Firewall**: Automatically configures UFW for security.

## ⚙️ Parameters

- `image`: `ghcr.io/w0rng/amnezia-wg-easy`
- `web_port`: `4466`
- `vpn_port`: `993/UDP`
- `obfuscation`: `JC=10`, `JMIN=100`, `JMAX=1000`, `S1=15`, `S2=100`
