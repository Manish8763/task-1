# Optional Task: Network Services and Ports Report

## 🔍 Objective
To analyze open ports and their services discovered using Nmap, and explain their functions and potential risks.

---

## Discovered Services and Explanations

### Port 135 – MSRPC
- *Service*: Microsoft RPC (Remote Procedure Call)
- *Use*: Communication between Windows applications/services
- *Risk*: Common target for malware and exploits

---

### Port 139 – NetBIOS-SSN
- *Service*: NetBIOS Session Service
- *Use*: File and printer sharing on Windows networks
- *Risk*: Vulnerable if exposed to the internet

---

### Port 445 – Microsoft-DS
- *Service*: SMB over IP (Server Message Block)
- *Use*: Windows file sharing
- *Risk*: Frequent vector for ransomware attacks (e.g., WannaCry)

---

### Port 902 – ISS RealSecure
- *Service*: VMware-related (also used by ISS RealSecure)
- *Use*: Remote access to virtual machines
- *Risk*: May expose VM services if not firewalled

---

### Port 912 – Apex-Mesh
- *Service*: Possibly custom or unknown
- *Use*: Not well-documented — likely part of a private app
- *Risk*: Needs investigation; may indicate custom software

---

### Port 3306 – MySQL
- *Service*: MySQL Database
- *Use*: Open-source relational database service
- *Risk*: Should never be publicly accessible without authentication
---

## Tools Used

- *Nmap*
nmap -sS 192.168.56.1