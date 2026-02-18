# AmirTunnel-Pro
High-performance, Reverse TCP Tunnel with dynamic Xray port synchronization. Designed for maximum speed and intranet-to-internet bridging.

Markdown
# 🚀 AmirTunnel-Pro (MPS PRO)

High-performance, Reverse TCP Tunnel with dynamic Xray port synchronization. Specifically designed to bypass upload speed restrictions and provide a seamless connection between Iran and External servers.

## ⚡ Quick Start (Auto-Install & Run in Background)

Use this single command to download the script and run it inside a **Screen** session. This ensures the tunnel keeps running even after you close the terminal.

```bash
wget --no-check-certificate -O AmirTunnelPro.py http://raw.githubusercontent.com/amircpuir/AmirTunnel-Pro/main/AmirTunnelPro.py && screen -S amirtunnel python3 AmirTunnelPro.py
🛠 How to Use
1. Setup on Iran Server (Bridge)
Run the command above and select Option 2 (Iran Server).

Enter your Tunnel Bridge Port (e.g., 443).

Enter your Port Sync Port (e.g., 444).

Choose y for Auto-Sync or n for Manual Entry.

2. Setup on Europe Server (Exit)
Run the command above and select Option 1 (Europe Server).

Enter your Iran Server IP.

Use the same ports you configured on the Iran server.

📺 Managing your Session (Screen Commands)
Since the script runs inside a "Screen" session named amirtunnel:

To Detach: Press Ctrl + A then D (This leaves the tunnel running in the background).

To Re-attach: Run screen -r amirtunnel to see the logs and the menu again.

To Kill: Run screen -XS amirtunnel quit.

🚀 Key Features
Persistence: Runs in a screen session to prevent disconnection issues.

Dynamic Sync: Automatically detects and opens Xray inbounds.

SSL Bypass: Uses --no-check-certificate for reliable downloads on restricted networks.

Zero Latency: Optimized for Iranian network infrastructures.

🔧 Troubleshooting
If you see Address already in use, it means a previous session is still holding the ports. Kill all python processes using:

Bash
pkill -f python3
