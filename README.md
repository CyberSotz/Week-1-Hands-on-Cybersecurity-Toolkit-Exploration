# Week-1-Hands-on-Cybersecurity-Toolkit-Exploration

# 🛡️ Cybersecurity Tools & Concepts – Weekly Learning Reflection

## 👋 Introduction

This repository presents a structured reflection on essential cybersecurity tools and frameworks, curated during weekly training at **KaiRiz Cyber Technologies** by **Muhammad Naveed Ul Hassan**.  
The learning is hands-on and aligns with real-world cybersecurity practices covering reconnaissance, scanning, protocol inspection, and red teaming.

---

## 🔧 Tools & Frameworks Covered

### 🛰️ Nmap – Advanced Network Mapping
- **Purpose**: Host discovery, port scanning, service enumeration, OS detection.
- **Key Features**:
  - TCP/UDP scanning
  - NSE scripting (vulnerability detection)
  - Version detection & OS fingerprinting
  - Customizable scan speed and timeout
- **Example Command**:
  ```bash
  nmap -sS -sV -O --top-ports 100 -Pn 192.168.1.1
  ```

---

### 🔬 Wireshark – Protocol Analysis & Deep Packet Inspection
- **Purpose**: Capture and analyze network traffic in real time.
- **Use Cases**:
  - TCP/UDP session inspection
  - TLS handshake & certificate analysis
  - DNS resolution and filtering
- **Filters Used**:
  ```
  http, tls.handshake, ip.addr == 192.168.1.1
  ```

---

### 🔍 Google Dorking (OSINT)
- **Description**: Leveraging advanced search operators to discover exposed data or misconfigured systems online.
- **Examples**:
  - `intitle:"index of" site:.gov`
  - `filetype:sql inurl:admin`
  - `site:example.com intext:password`

---

### 🧠 MITRE ATT&CK Framework
- **What It Is**: A matrix of Tactics, Techniques, and Procedures (TTPs) used by threat actors.
- **Red Team Usage**: Simulate attack behaviors (e.g., APT28, TeamTNT)
- **Blue Team Usage**: Detect adversary patterns in logs and alerts
- **Example Techniques**:
  - `T1059.001` – PowerShell
  - `T1087` – Account Discovery

---

## ⚙️ Additional Kali Linux Tools

### 🔐 Hydra – Password Brute Force Tool
- Supports SSH, FTP, HTTP, SMB, RDP, Telnet, and more.
- **Command Example**:
  ```bash
  hydra -l admin -P rockyou.txt ssh://192.168.1.5
  ```

### 🌐 Nikto – Web Server Scanner
- Scans for outdated software, misconfigurations, default credentials.
- Checks for 6700+ known vulnerabilities.
- **Example**:
  ```bash
  nikto -h http://192.168.1.100
  ```

### 🕷️ Burp Suite – Web Application Security Testing
- **Key Modules**:
  - Proxy: Intercept and inspect traffic
  - Repeater: Manual request modification
  - Intruder: Automated payload fuzzing
  - Scanner: Vulnerability detection
- **Example Workflow**:
  Intercept login request → Modify payload → Replay → Analyze response

---

## ✅ Key Accomplishments

- 🛠️ Practiced enumeration with **Nmap**
- 🔍 Analyzed live network packets using **Wireshark**
- 🧠 Simulated adversary behaviors via **MITRE ATT&CK**
- 🧪 Performed brute force and scanning using **Hydra**, **Nikto**, and **Burp Suite**
- 🛰️ Strengthened both red teaming and blue teaming thinking

---

## 📎 Resources

- [Nmap Documentation](https://nmap.org/book/man.html)
- [Wireshark Filters Guide](https://wiki.wireshark.org/DisplayFilters)
- [MITRE ATT&CK Matrix](https://attack.mitre.org/)
- [Kali Linux Toolset](https://tools.kali.org/)
- [Google Hacking DB](https://www.exploit-db.com/google-hacking-database)

---

## 🧑‍💻 Author

**Muhammad Naveed Ul Hassan**  
📧 muhammadnaveedulhassan@proton.me  
🎓 Red Teamer Trainee  
🏢 KaiRiz Cyber Technologies

---

 “Cybersecurity is not just a skill—it's a mindset. Understanding the attacker makes you a better defender.”
