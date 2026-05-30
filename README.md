# FILE-CREATE - JACK Tool Suite

A powerful Facebook UID analysis, generation, and extraction tool with real-time device monitoring, rainbow UI, and concurrent checking capabilities.

## ⚠️ Disclaimer
**This tool is for educational and research purposes only. Use responsibly and in compliance with Facebook's Terms of Service. The author is not responsible for any misuse or violations.**

## 🌟 Features

### Core Functionality
- **UID Checking** - Fast concurrent Facebook UID verification (20 threads)
- **UID Generation** - Generate UIDs based on different Facebook eras (2007-2026)
- **URL to UID** - Extract UIDs from Facebook profile URLs
- **Profile Detection** - Identifies REAL, DISABLED, CHECKPOINT, and HIDDEN profiles

### Device Information Display
- Real-time clock with colored output
- Public IP address (via api.ipify.org)
- Network type detection (Wi-Fi/Mobile Data)
- Geolocation from IP (via ip-api.com)
- VPN/Proxy detection with ISP identification
- Internet speed test (download/upload via speedtest-cli)
- RAM usage (total/used/free)
- Storage information (total/free)
- Device name and Android version detection

### Visual Features
- **Ultra Color Palette** - 12 vibrant colors with rainbow effects
- **Blinking text effects** for attention-grabbing elements
- **Spinner animations** with ETA during UID checking
- **Progress bars** for UID generation
- **Loading animations** with checkmark confirmations
- **Colorful ASCII banner** with owner information

### Data Management
- Auto-saves results to both current directory and `/sdcard/jack_results/`
- Generates separate files for:
  - `real_uids.txt` - Valid profiles with names
  - `cp_uids.txt` - Checkpoint restricted profiles
  - `fake_uids.txt` - Disabled/fake/non-existent profiles
  - `extracted_uids.txt` - UIDs from URL conversion
- Telegram auto-forward for real UIDs
- Interruption handling with partial data saving

### About & Contact Section
- Complete system information display
- Direct links to Telegram channels and personal contacts
- Browser integration to open Telegram links automatically
- Support and contribution information

## 📋 Requirements

- **Android** with Termux (primary target)
- **Python 3.8+**
- Required packages (auto-installed if missing):
  - `requests`
  - `speedtest-cli` (optional, for speed test)
  - `iproute2`

## 🔧 Installation

### Termux (Android)
```bash
pkg update && pkg upgrade
pkg install python git
git clone https://github.com/poran0-9/FILE-CREATE.git
cd FILE-CREATE
python FILE-CREATE.py
