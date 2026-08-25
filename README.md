#  My Cybersecurity Cheat-Sheets & Resources

Welcome to my personal cybersecurity knowledge base. This repository contains essential websites, tools, documentation links, and command-line cheat-sheets that I use for learning and daily practice.

---

## 🗺️ Table of Contents
* [🌐 Useful Learning Platforms](#-useful-learning-platforms)
* [🔍 Threat Intelligence & OSINT](#-threat-intelligence--osint-open-source-intelligence)
* [🛑 Vulnerability Databases & Exploits](#-vulnerability-databases--exploits)
* [🐧 Linux Cheat-Sheet (Useful Commands)](#-linux-cheat-sheet-useful-commands)
* [🪟 Windows Cheat-Sheet (PowerShell)](#-windows-cheat-sheet-powershell)
* [📘 Manuals & Reading Material](#-manuals--reading-material)

---

## 🌐 Useful Learning Platforms

### Practice & Labs
* [TryHackMe](https://tryhackme.com) — Interactive rooms and structured learning paths for all levels.
* [Hack The Box](https://hackthebox.com) — Advanced gamified machines for penetration testing practice.
* [PortSwigger Web Security Academy](https://portswigger.net) — The absolute best free course for web vulnerabilities (OWASP Top 10).

### Reference & Methodologies
* [OWASP Top 10](https://owasp.org) — The standard awareness document for web application security risks.
* [MITRE ATT&CK Matrix](https://mitre.org) — A globally-accessible knowledge base of adversary tactics and techniques based on real-world observations.

---

## 🔍 Threat Intelligence & OSINT (Open Source Intelligence)

### IP, Domain & File Investigation
* [VirusTotal](https://virustotal.com) — Analyze suspicious files, domains, IPs, and URLs to detect malware and breaches.
* [Shodan](https://shodan.io) — The search engine for Internet-connected devices (IoT, servers, industrial control systems).
* [Censys](https://censys.io) — Attack surface management and search engine for global network infrastructure.
* [WHOIS Lookup by DomainTools](https://domaintools.com) — Find domain ownership data, nameservers, and registration details.

### Threat Feeds & URL Sandbox
* [IntelX](https://intelx.io) — Intelligence X search engine for historical archives, open buckets, and data leaks.
* [URLScan.io](https://urlscan.io) — A sandbox for websites; safely analyzes what a URL does without visiting it directly.
* [AlienVault OTX](https://alienvault.com) — Open Threat Exchange; crowd-sourced threat intelligence feed.

---

## 🛑 Vulnerability Databases & Exploits

### Finding Exploits
* [CVE Details](https://cvedetails.com) — Comprehensive and easy-to-use database of historical security vulnerabilities.
* [Exploit-DB](https://exploit-db.com) — An ultimate archive of public exploits and shellcode for penetration testing.

### Practical Utilities
* [CyberChef](https://github.io) — "The Cyber Swiss Army Knife". Web tool for decoding, encoding, hashing, and analyzing data.
* [PayloadsAllTheThings](https://github.com) — A massive repository of payloads and bypasses for Web Application Pentesting.

---

## 🐧 Linux Cheat-Sheet (Useful Commands)

### Network Reconnaissance
Scan a target IP address for open ports, OS detection, and service versions using `nmap`:
```bash
nmap -sV -sC -Pn <target_ip>
```

### Privilege Escalation (Finding SUID Files)
Find all files with the SUID bit set (potential vector for getting Root access):
```bash
find / -perm -u=s -type f 2>/dev/null
```

### Privilege Escalation Reference
* [GTFOBins](https://github.io) — Curated list of Unix binaries that can be used to bypass local security restrictions.

---

## 🪟 Windows Cheat-Sheet (PowerShell)

### View Active Network Connections
Show all active TCP connections and the processes using them:
```powershell
Get-NetTCPConnection | Select-LocalAddress,LocalPort,RemoteAddress,RemotePort,State | Format-Table
```

### Privilege Escalation Reference
* [LOLBAS Project](https://github.io) — Curated list of Windows binaries, scripts, and libraries used for Living Off The Land techniques.

---

## 📘 Manuals & Reading Material
* Book: *«How Linux Works»* by Brian Ward.
* Book: *«The Pentester BluePrint»* by Phillip Wylie.
* Reference: [Nmap Official Command-Line Brief Reference](https://nmap.org).
* Documentation: [Wireshark Display Filters Official Guide](https://wireshark.org).
