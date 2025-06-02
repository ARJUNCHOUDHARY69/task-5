# Wireshark Packet Capture Analysis

## Overview

This project demonstrates basic network traffic analysis using Wireshark. The objective is to capture and inspect real-time network packets, identify key protocols in use, and summarize findings from a `.pcapng` file.

## Steps Followed

1. **Installed Wireshark**  
   - Downloaded and installed from [https://www.wireshark.org/](https://www.wireshark.org/).

2. **Captured Live Traffic**  
   - Selected the active network interface.
   - Captured packets for about 1 minute while:
     - Browsing websites.
     - Running `ping` commands to external servers.

3. **Stopped Capture**  
   - Saved the capture session as `main.pcapng`.

4. **Filtered by Protocol**  
   - Applied filters like `http`, `dns`, `tcp` in Wireshark’s filter bar.

5. **Identified Protocols**
   - Observed the following protocols:
     - **DNS** – Used for resolving domain names.
     - **TCP** – Manages reliable data transmission.
     - **TLS** – Handles encrypted communication.
     - *(Others may include HTTP, ICMP, ARP depending on traffic.)*

6. **Exported the Capture**  
   - File exported in `.pcapng` format.

## Findings

| Protocol | Description                  | Notes                               |
|----------|------------------------------|--------------------------------------|
| DNS      | Domain Name System           | Seen during site lookups.           |
| TCP      | Transmission Control Protocol| Used for data transfer sessions.    |
| TLS      | Transport Layer Security     | Secures HTTPS sessions.             |

> Captured packet details (source/destination IPs, ports, flags) are available in the `.pcapng` file.

## File

- `main.pcapng` – Packet capture file (Wireshark format)

## Tools Used

- **Wireshark** – for capturing and analyzing packets.

## Notes

To analyze this file yourself:
1. Open Wireshark.
2. Load `main.pcapng`.
3. Use filters like `tcp`, `dns`, `http`, etc., to explore traffic.

---![image](https://github.com/user-attachments/assets/cc20e909-0110-47d0-82b8-491b27598123)

