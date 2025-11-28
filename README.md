# Bash-Script-Port-Scanning-Tool

## 🔎 Bash Port Scanner

This script is a lightweight Bash-based tool designed to scan TCP ports on a target IP address across a specified range. By attempting to establish a TCP connection to each port, it determines whether the port is open or closed. Ideal for quick diagnostics, it's a handy utility for network administrators and cybersecurity professionals.

## ⚙️ Features
- Scan a custom range of ports
- Shows OPEN and CLOSED ports
- Fast and lightweight
- Pure Bash (no external tools like nmap)
- Input validation included

## 🧪 How It Works
You provide two inputs:  
1. A target IP address  
```./port_scanner.sh <target> <start_port> <end_port>```
2. A port range in the format `start-end` (e.g., `1-1000`)

The script parses the range, then loops through each port, attempting a TCP connection. If the connection succeeds, the port is marked as open; otherwise, it's reported as closed.

## 📌 Example Usage
```bash
./port_scanner.sh scanme.nmap.org 20 100
