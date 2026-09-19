# Week 2 - Footprinting, Reconnaissance & Network Scanning

**Networkwalks Academy | Cybersecurity & Ethical Hacking Internship**

## Overview
This repository documents Week 2 of the internship, covering passive footprinting of the domain `networkwalks.com` using multiple Kali Linux tools, OSINT gathering with theHarvester, and local network discovery using Zenmap (Nmap GUI).

## Modules Completed

### W2-PM1: Footprinting with Multiple Kali Tools
Ran six built-in Kali Linux tools against `networkwalks.com`:
- **whois** — domain registration details, registrar, name servers
- **whatweb** — web technology fingerprinting (WordPress 7.1, WP Download Manager 3.3.58)
- **nslookup** — resolved domain to IP (192.232.216.135)
- **curl -I** — HTTP response headers
- **wafw00f** — detected ModSecurity (SpiderLabs) WAF
- **dnsrecon** — enumerated DNS records (SOA, NS, MX, TXT, SRV)

Each tool's output was saved as a `.txt` file and captured as a screenshot.

### W2-PM4: Footprinting with theHarvester
Gathered OSINT (emails, subdomains, hosts) for `microsoft.com`:
- **Task 1:** Search using Baidu source, limit 1000 results
- **Task 2:** Search using all available sources, limit 50 results — found multiple subdomains under `fabric.microsoft.com` and `ait.microsoft.com`

### W2-PM5: Network Scanning with Zenmap
Performed local network discovery on my home LAN:
- Installed Zenmap (Nmap GUI) on Windows
- Identified local IP (192.168.18.9) and subnet (192.168.18.0/24)
- Ran a Ping Scan to discover live hosts
- Found **4 live hosts** with their IP and MAC addresses
- Generated and saved the network topology as a PDF

## Folder Structure
W2-PM1-footprinting/ → whois, whatweb, nslookup, curl, wafw00f, dnsrecon (screenshots + txt outputs)
W2-PM4-theharvester/ → theHarvester Task 1 & 2 (screenshots + txt outputs)
W2-PM5-zenmap/ → Zenmap scan results (screenshot + topology PDF)


## Key Learnings
Passive reconnaissance can reveal a significant amount about a target — hosting provider, software versions, DNS infrastructure, and firewall presence — without ever directly contacting or attacking the system. This information forms the foundation for later stages of a security assessment.

## Disclaimer
All activities in this repository were performed strictly for educational purposes on domains/networks I had authorization to test (own home network, and the instructor-designated practice domain `networkwalks.com`).
