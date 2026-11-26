<div align="center">

# 🔐 Cybersecurity Lab - PENETRATION TESTING REPORT

**Real-world Penetration Testing Project**

</div>

<p align="center">

<p align="center">
  <img src="https://img.shields.io/badge/Skill-Cybersecurity-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Ver-Virtualbox%20v7.2-0070C0?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Kali%20Linux-v2026.3-E87500?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Skill-Linux-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Local%20Network-10.0.0.0%2F24-238F89?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Penetration%20Testing-C00000?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Skill-Virtualization-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Ethical%20Hacking-E87500?style=flat-square&labelColor=000000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Kali%20Linux-404040?style=flat-square&labelColor=C00000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Skill-Reconnaissance%20&%20Footprinting-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Skill-Scanning%20&%20Network%20Discovery-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Skill-Password%20Hacking-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Skill-Dictionary%20Attacks-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Skill-Hash%20Cracking-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Networkwalks%20Tool-Hash%20Calculator-238F89?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Networkwalks%20Tool-Password%20Hacker-238F89?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/GitHub-404040?style=flat-square&labelColor=0070C0&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/NetworkWalks-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Chigozie%20Kenneth%20Chigozie-%20CCEP-C00000?style=flat-square" />>
</p>

---

## 📌 Project Overview

This project is a real-world Penetration Testing Project structured in four milestonese (M1, M2, M3 and M4).

👉 M1 - Initial Access : Attack of the website and retrieval of 3 confidential patient PDF lab reports.

    D E L I V E R A B L E: Proof of access and the 3 retrieved PDF files.

👉 M2 - Data Extraction : Cracking the encryption on all 3 retrieved files.

    D E L I V E R A B L E: Recovered contents of all 3 files with proof of successful access.

👉 M3 - Attack (cracking) : Finding staff salaries and shareholder details of the hospital.

    D E L I V E R A B L E: Full documented evidence of the exposure and a readable summary of the confidential data uncovered.

👉 M4 - Pentest Report : Writing a professional penetration testing report for the client.

    D E L I V E R A B L E: A complete professional penetration testing report.

The project has a timeline of 5 days.

The client has provided written authorisation to conduct security testing on their web infrastructure.

---

##  ⚖️ Liability Disclaimer

This project is conducted in a controlled environment for educational purposes only. The target has been authorised for security testing by Networkwalks. These techniques must never be applied to any system without explicit written permission from the owner.

Do not use anything from here to break the law. The instructor, the authors and Networkwalks are not responsible for what you do with this knowledge. Every action you take is your own responsibility. Misuse can lead to criminal charges, heavy fines, loss of your job and a permanent record. In most countries unauthorised access is a crime even when nothing is damaged.

---

# 📘Penetration Testing Report

---

# 1. 🎯 Executive Summary

In the context of the Mediroza Hospital’s website `https://medirozahospital.com` security audit, we conducted a  security assessment to evaluate its security posture on November 23rd, 2026. The vulnerabilities assessment revealed security flaws that could expose sensitive information to unauthorized persons. We identified identified several significant weaknesses affecting the protection of sensitive business and patient information. 

The assessment demonstrated that confidential organizational data and protected patient health records are currently exposed. Multiple weaknesses across authentication controls and document protection mechanisms collectively increase the likelihood of unauthorized disclosure of sensitive information. The web platform's security posture is critically weak: independent vulnerabilities were each exploited in practice, and together they give full access to sensitive personal, medical and financial data. This puts the company’s business at risk, as well as its compliance with standards and regulations regarding personal and health data.

We recommend the immediate implementation of the following measures: 

Priority 1: Urgently (in 0–48 hours) ask developpers team to fix and enhance authentication mechanisms, remove public access to the database backup and treat all credentials in the backup as compromised. Rotate database, application, API and admin passwords and keys.

Priority 2: In a short term (1-2 weeks), strenghten the encryption of patient reports, delete the backup from the web root and store it in encrypted storage with restricted access or even offline, block the path at the web server level, review access logs for the backup, login endpoints and any anomalous queries to determine whether data was accessed by anyone other than authorized persons and audit team, activate the incident response and legal process, assess breach notification obligations to the data protection authority and affected individuals.

Priority 3: In a medium term (3-5 weeks), ensure authentication is hardened with CAPTCHA, multi-factor authentication, log and alert on repeated failures, implement system and data monitoring.

Priority 4: Ongoing schedule a full penetration test and re-test after remediation to validate fixes, run periodic vulnerability scans and annual security audits, maintain an incident response plan and conduct awareness training for staff.

Ultimately, the current website security does not meet the standards expected within an Information Security Management System (ISMS), especially in the health industry. Urgent corrective actions are essential to protect the company’s assets and significantly reduce data breach risks, in accordance with ISO 27001 regulatory standards.

---

# 2. 💎 Scope and Methodology

## 2.1 Project details

| Field | Detail |
|---|---|
|**Project Type** | Penetration Testing & Vulnerability Assessment|
|**Client Name**| Mediroza General Hospital|
|**Target**| `https://medirozahospital.com`|
|**Scope** |Full black-box penetration test. Identify vulnerabilities, exploit them to demonstrate real impact, and document all findings in a professional report.|
|**Rules**| Testing limited to the target domain only. No social engineering. No denial of service. No testing outside agreed scope.|
|**Authorization**| The client has provided written authorisation to conduct security testing on their web infrastructure.|
|**Timeline**| 5 days. Work independently.|

---

## 2.2 Report details

| Field | Detail |
|---|---|
| **Date** | 26 November 2026 |
| **Version** | 1.0.0 |
| **Author (Cybersecurity Professional)** | **Dickson Kenneth Chigozie** |
| **Classification** | CONFIDENTIAL|
| **Reference standards** | Compliant with ISO 27001:2022 and PASSI reference standard (ANSSI)|
| **Client company** |Mediroza General Hospital|

---

## 2.3 Methodology

We demonstrated the impact of vulnerabilities in a concrete way, using a structured penetration testing methodology (PTES – Penetration Testing Execution Standard).

````text
Reconnaissance
      ↓
Enumeration
      ↓
Vulnerability Identification
      ↓
Manual Validation
      ↓
Controlled Exploitation
      ↓
Impact Assessment
      ↓
Evidence Collection
      ↓
Risk Rating
      ↓
Remediation
````

---

## 2.4 Tools Used

The table below lists each tool used in this report and its purpose.

| Tool | Purpose |
|---|---|
| Kali Linux  | Operating system used to perform the penetration testing activities|
| whois                | Find domain registration details (owner, dates, name servers).   |
| whatweb              | Fingerprint web technologies (server, CMS, plugins, IP).         |
| nslookup             | Resolve the domain name to its IP address using DNS.             |
| curl              | Read the HTTP response headers of the website & website.xml, robots.txt. |
| wafw00f              | Detect whether a Web Application Firewall protects the site.     |
| dnsrecon             | Enumerate all DNS records (NS, MX, SPF, TXT, SRV).               |
| nmap     | Scan the local subnet to find live hosts, IPs and MAC addresses. |
| Networkwalks Hash Calculator | Get the hash values of files  |
| Networkwalks Password Cracker | Crack password of files  |

---

# 3.  💎 Findings and Proof of Exploitation

---

## 3.1 Milestone 1 - Attack and patients reports getting

---

---

## 3.1 Milestone 1 - Attack and patients reports getting

---

### 🫆 Footprinting & Reconnaissance

I performed reconnaissance against the `https://medirozahospital.com` website using Kali Linux tools: **Whois, WhatWeb, Nslookup, Curl, Wafw00f and DNSRecon**. Each tool was used to collect a different type of information about the target.

First, I used **WHOIS** to obtain publicly available registration information. The results provided no valuable information. 

---

<img width="1917" height="1077" alt="whois" src="https://github.com/user-attachments/assets/8824dfe3-d47c-434a-aac6-2337dcab6d41" />

---

I then used **WhatWeb** to identify technologies used by the website. The results identified **HTML5**, **LiteSpeed** and the IP address **199.188.201.16**. No versions of software exposed here.

---

<img width="1917" height="1077" alt="whatweb" src="https://github.com/user-attachments/assets/5eb041c3-4847-472c-a637-8ebd364eeedd" />

---

Using **Nslookup**, I resolved the website name to its IP address. The provided result identified **199.188.201.16**.

---

<img width="1917" height="1077" alt="nslookup" src="https://github.com/user-attachments/assets/fa2eddd2-9e76-4d36-a1ca-8e7f2a9566f3" />

---

I used **Curl** with the `-I` option to inspect the HTTP response headers. This provided **LiteSpeed** as server. No REST API endpoint exposed.

---

<img width="1917" height="1077" alt="curl i" src="https://github.com/user-attachments/assets/25c5fd8e-8f08-42bd-a2c5-01dde2b489dc" />

---

Next, I used **Wafw00f** to determine whether a Web Application Firewall was protecting the website. The result identified **LiteSpeed (LiteSpeed Technologies)**.

---

<img width="1917" height="1076" alt="wafw00f" src="https://github.com/user-attachments/assets/851f8d58-98b8-436e-aa28-7b88d60f94dd" />

---

Finally, I used **DNSRecon** to enumerate DNS records. The results provided information relating to name servers and TXT records.

---

<img width="1917" height="1077" alt="dnsrecon" src="https://github.com/user-attachments/assets/78d494a2-97e2-45cc-ab8b-d4a78cb75d2a" />

---

The outputs of all the above commands were saved in a txt file available at **`/output_files/footprinting.txt`**.

---

### 🔍 Ports Scanning with Nmap

I used **nmap** from my Kali Linux terminal to perform ports scanning on the target. The website's IP address is **`199.188.201.16`**). 

I scanned with the command : 

````bash
nmap -sV -sC 199.188.201.16
````

The results identified twelve active ports.

---

<img width="1917" height="1077" alt="nmap" src="https://github.com/user-attachments/assets/4c787261-6265-48c4-ae93-c92876e63729" />

---

The output of this first scan is saved in a txt file available at **`/output_files/scan_short.txt`**.

---

I also full scanned with the command : 

````bash
nmap -A -p- -T4 199.188.201.16 -oN scan_full.txt 
````

The results identified twelve active ports.

---

<img width="1917" height="1077" alt="nmap full scan" src="https://github.com/user-attachments/assets/fafe0b53-11e6-4205-ab40-bf5a6634a3ec" />

---

<img width="1917" height="1077" alt="nmap full scan 2" src="https://github.com/user-attachments/assets/6eda1a7e-d77c-4085-8709-74add0167274" />

---

The output of this second scan is saved in a txt file available at **`/outputs_files/scan_full.txt`**.

---
