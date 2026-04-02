# 🧠 OIntell

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux%20%2F%20Windows-informational?style=flat-square&logo=linux&logoColor=white&color=0a0c10"/>
  <img src="https://img.shields.io/badge/Category-OSINT%20%2F%20Intelligence-cyan?style=flat-square"/>
  <img src="https://img.shields.io/badge/Dependencies-None%20(Standalone)-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-Proprietary-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-v1.0-cyan?style=flat-square"/>
</p>

> **OIntell** is a comprehensive passive OSINT intelligence engine. It gathers information on IPs, domains, emails, usernames, phone numbers, and hashes using only public sources — no API keys required for core functionality.

---

## 📌 Overview

OIntell combines multiple OSINT modules into one clean terminal interface. It supports IP geolocation & threat intel, full domain reconnaissance (WHOIS, DNS, subdomains, cert transparency), email validation & breach hints, username hunting across major platforms, phone number analysis, and hash identification/computation. All modules are passive where possible and include colored output with detailed reporting.

---

## 🖥️ Modules

| # | Module                | Description |
|---|-----------------------|-------------|
| **[1]** | **IP Intelligence**       | Geolocation, ASN, rDNS, Tor/VPN/Proxy detection, threat indicators |
| **[2]** | **Domain Recon**          | WHOIS/RDAP, DNS records (A, MX, NS, TXT), subdomains, cert transparency, HTTP headers |
| **[3]** | **Email Lookup**          | Syntax validation, MX check, disposable email detection, provider identification |
| **[4]** | **Username Hunt**         | Check username existence across 20+ major platforms (GitHub, Twitter, Instagram, etc.) |
| **[5]** | **Phone Lookup**          | Country/code detection, E.164 formatting, carrier type inference |
| **[6]** | **Hash Analyser**         | Identify hash type by length/pattern, known hash matching, compute multiple hashes |
| **[7]** | **Bulk Lookup**           | Process multiple targets from a file with type prefixes (ip:, domain:, email:, etc.) |

---

## 📊 Key Features

- **Passive OSINT Only**: Uses public APIs and system resolvers (no aggressive scanning)
- **Multi-Source Intelligence**: ip-api.com, RDAP, crt.sh, DNS, HTTP headers
- **Live Spinner Feedback**: Clear progress indicators during lookups
- **Colored Output**: Easy-to-read results with severity highlighting
- **Session Export**: Save all lookups in one JSON report
- **CLI + Interactive**: Supports both menu mode and direct command-line arguments

---

## ⚙️ Requirements

- **Linux or Windows**
- **No Python installation needed** — runs as a standalone executable
- **Internet connection** required for most modules
- **Optional**: Some DNS lookups use system tools (`dig`/`nslookup`)

---

## 🚀 Usage

```bash
./OIntell


Command-line examples:
Bash./OIntell --ip 8.8.8.8
./OIntell --domain example.com
./OIntell --email user@example.com


📦 Part of OwlSec Toolkit
This tool is part of the OwlSec suite — a collection of 300+ security and privacy tools.
🔗 owlsec.org

©️ License
Proprietary — © Khaled S. Haddad
Tools are distributed as pre-built executables. Source code is proprietary.

AUTHORISED SECURITY TESTING USE ONLY
