# Custom ICMP-Based IP Blocklist

## 🚀 Overview
This repository provides a list of IP addresses captured and banned by **banip** on my local infrastructure. 

### 🔍 How these IPs are caught
Unlike many other lists that simply mirror existing databases, this list focuses on active attackers:
1. **No Prior Listing:** At the moment of capture, these IPs were **not** found in the standard `banip` feed providers.
2. **ICMP Protocol Violation:** These addresses were automatically caught by the system log flag `PROTO=ICMP`.
3. **Behavior:** They were flagged for suspicious ping sweeps, ICMP flooding, or reconnaissance probes.

## 📊 Format
The list is provided in a standard text format with timestamps:
`IP_ADDRESS # added on YYYY-MM-DD HH:MM:SS`

## ⚖️ Disclaimer
This list is generated automatically based on detected network attacks. 
- **Use at your own risk.** - The author is not responsible for any network connectivity issues caused by blocking these IPs.
- If you believe your IP was blocked by mistake (False Positive), please open an **Issue** in this repository for manual review.
