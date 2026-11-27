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

The results identified two active ports.

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

### Enumeration

I used `curl` to perform enumeration on the target with the following commands:

````bash
curl -s https://medirozahospital.com | grep -Eo 'href="[^"]+"' | sort -u
````

````bash
curl https://medirozahospital.com/sitemap.xml 
````

````bash
curl https://medirozahospital.com/robots.txt
````

---

<img width="1917" height="1077" alt="curl enumeration" src="https://github.com/user-attachments/assets/ffd976b9-8726-481d-8088-41f6de57f230" />

---

<img width="1917" height="1077" alt="curl enumeration 2" src="https://github.com/user-attachments/assets/b1b1a826-e046-448f-bb33-b58bbf099e08" />

---

<img width="1917" height="1077" alt="curl enumeration 3" src="https://github.com/user-attachments/assets/a8df4f0d-162a-4210-8a8c-a00fdda949c0" />

---

<img width="1891" height="1077" alt="robots" src="https://github.com/user-attachments/assets/49dc0500-31d7-4731-9338-3ec6fc21c0eb" />

---

<img width="1917" height="1076" alt="robots 2" src="https://github.com/user-attachments/assets/c7ef06e3-6035-412d-b7aa-11fbb16b73f8" />



The outputs of the commands used for enumeration were saved in a txt file that is available at **`/output_files/enumeration.txt`**.

I remarked information disclosure via **`robots.txt`**: paths that were not visible through normal navigation on the website had showed up. 

They were 3 key paths:

````text
https://medirozahospital.com/patient/
https://medirozahospital.com/staff/
https://medirozahospital.com/old/
````

Those are exposed entry points.

I entered them one by one in the browser.

---

#### /patient/

<img width="1917" height="1071" alt="index of patient" src="https://github.com/user-attachments/assets/cb75fd92-5136-4385-8827-c9f36fe88711" />

---

#### /staff/

<img width="1917" height="1077" alt="index of staff" src="https://github.com/user-attachments/assets/e1812fdf-c5e1-43ab-8037-c3d8983c7458" />

---

#### /old/

<img width="1917" height="1077" alt="index of old" src="https://github.com/user-attachments/assets/6c14df03-4309-4a35-a116-06613e44d971" />

---

The presence of a folder **/patient/reports** indicated that there would patient reports files in the **Patient Portal**.

I tried to gain the access with common usernames and passwords. I analyzed the behaviour of the authentication mechanisms.

---

#### wrong username error message

<img width="1917" height="1077" alt="incorrect password" src="https://github.com/user-attachments/assets/343ed3c5-7a8d-44cb-8ee8-3ea6450029d3" />

---

A trial with the default username `admin` got **Incorrect password**.

---

<img width="1917" height="1077" alt="admin username" src="https://github.com/user-attachments/assets/2df8a40b-f266-4233-9718-e4101eb20762" />

---

#### correct username error message

<img width="1917" height="1077" alt="incorrect password" src="https://github.com/user-attachments/assets/2191b942-b5a2-48dd-93d3-13dd2d0ae302" />

---

That behaviour lets guess which one of the credentials is wrong and helps a correct username even if the entered password is wrong.

Having a valid username could make the attack easier.

As many common passwords were failing, I opted for SQL injection.

---

<img width="1917" height="1077" alt="login details" src="https://github.com/user-attachments/assets/f77c2b97-a1b4-411e-958f-772f595c9cd0" />

---

I gained the access by commenting the password requirement with the SQL injection.

---

<img width="1917" height="1078" alt="Screenshot 2026-11-26 021658" src="https://github.com/user-attachments/assets/5a18cabc-0b91-41f9-ad75-f356a20db998" />

---

I downloaded the 3 reports by clicking on the `download` buttons.

---

<img width="1917" height="1077" alt="downloaded file" src="https://github.com/user-attachments/assets/dc91dc5d-cdd1-462f-a99c-e9f0ad264ce3" />

---

The downloaded encrypted reports PDF files are : **`patient_report_1.pdf`**, **`patient_report_2.pdf`** and **`patient_report_3.pdf`**. They are available in the folder **`/download/`**.

---

## 3.2 Milestone 2 - Cracking the encrypted files

---

### Calculating hash values

I analyzed the  encryption of the locked reports PDF files.

I used Networkwalks Hash Calculator and uploaded the files turn by turn. A crackable hash had been extracted in pdf2john or hashcat compatible format.

The hash values of each file were saved and are available in the **`/output_files/`** : **`patient_report_1.hash.txt`**, **`patient_report_2.hash.txt`** and **`patient_report_3.hash.txt`**.

---

<img width="1917" height="1077" alt="hash pdf1" src="https://github.com/user-attachments/assets/6dd2164d-aff7-48ec-91ba-9c22587a3256" />

---

<img width="1917" height="1077" alt="hash pdf 2" src="https://github.com/user-attachments/assets/49a46758-58c6-4818-9433-82a23edcc1a4" />

---

<img width="1917" height="1077" alt="hash pdf 3" src="https://github.com/user-attachments/assets/6d698f22-a6eb-4915-9286-638b79747750" />

---

### Cracking the passwords

I used Networkwalks Password Cracker over the 3 hash values.

---

<img width="1917" height="1077" alt="password 12345" src="https://github.com/user-attachments/assets/cbefd176-ab78-4e5e-8099-5fbf10e6504a" />

---

<img width="1917" height="1077" alt="password" src="https://github.com/user-attachments/assets/e38b85bb-0a6a-4816-ac2b-ffb2a7f5232c" />

---

<img width="1917" height="1072" alt="access denied" src="https://github.com/user-attachments/assets/902f0f15-2df3-456a-8631-1553603e6d39" />

---

The password cracking was not successful for the **`patient_report_3.hash.txt`** using the native wordlist of 100 words integrated to the Networkwalks tool.

I uploaded the Kali Linux wordlist of 14,344,379 words into the Networkwalks tool. I run the cracking again and that was successful.

---

<img width="1917" height="1077" alt="last cracked password" src="https://github.com/user-attachments/assets/771ac9c5-5a10-4fb0-96e1-c574398eb32f" />

---

### Contents recovering

I launched each of the encrypted reports PDF files. I entered the cracked passwords and validated. 

---

<img width="1917" height="1077" alt="patient result" src="https://github.com/user-attachments/assets/91699f95-acc6-4f4a-87fb-aff05f3750a6" />

---

<img width="1906" height="1077" alt="patient result 2" src="https://github.com/user-attachments/assets/b66591a3-7078-4e92-bbdd-7a259cfa6f60" />

---

<img width="1917" height="1077" alt="patient result 3" src="https://github.com/user-attachments/assets/7dbef350-198a-4818-9b69-4263837e22b9" />

---

All the PDF files opened and their contents were recovered successfully.

---

## 3.3 Milestone 3 - Critical data exposure on the client server

---

I conducted a thorough analysis of everything retrieved so far. 

I tried to exploit /staff/ and /old/ found paths via enumeration.

### Exploiting /staff/ enumerated path

I entered common credentials in the fields of /staff/login.php. I also entered SQL injection requests.

No valuable result was found via the /staff/ revealed path.

---

<img width="1917" height="1077" alt="index of staff" src="https://github.com/user-attachments/assets/866206f2-aa2c-47b4-a267-dfe7e9f57679" />

---

<img width="1917" height="1077" alt="staff login" src="https://github.com/user-attachments/assets/1403d145-3121-498a-93db-075dfb94c531" />

---

### Exploiting /old/ enumerated path

I clicked and opened the file **`mediroza_db_backup_2019.sql`**.

<img width="1917" height="1077" alt="index of old" src="https://github.com/user-attachments/assets/9aafa2e7-966f-4f7f-a2f1-f78e47a8eae4" />

---

The opened page showed the company's database backup data.

---

<img width="1917" height="1077" alt="database 1" src="https://github.com/user-attachments/assets/38cead2e-863d-4cd8-b7fb-6deacc45ce72" />

---

<img width="1917" height="1072" alt="daabase 2" src="https://github.com/user-attachments/assets/fa5faa99-4584-464f-a68b-fb302e9152c5" />

---

The exposed details were critical and sensitive data. They were business financial data and staff sensitive personal data. 

Specifically, the database details (name: **`mediroza_hr`**), confidential staff and shareholder records were clearly exposed.

I extracted  the salaries of all hospital employees and the shareholder details of the hospital.

I made a readable summary of the confidential data uncovered.

---

### Database and technical details

|Element|Details|
|----|----|
|Backup date: |2019-08-27 02:14:03|
|Backup name:|mediroza_db_backup_2019.sql|
|Backup type:|internal database backup|
|Contents:| confidential staff and shareholder records |
|Host: | localhost |
|Database name: | mediroza_hr|
|Company:| Mediroza General Hospital |
|Generated by: | Mediroza CMS 1.4.2 backup module|


---

---

### Salaries

ID (`id`)|Full Name (`full_name`)|Job Title (`job_title`)|Department (`department`)|Salary in ZAR (`monthly_salary_zar`)|Date Joined (`date_joined`)|
----|-------|-----------|--------|-----------|------------|
1|Dr. Rajesh Naidoo|Chief Pathologist|Diagnostics Lab|138000|2009-03-16|
2|Sarah Botha|Chief Financial Officer|Finance|152000|2011-07-01|
3|Dr. Johan van der Merwe|Medical Director|Management|160000|2007-01-22|
4|Dr. Anita Naicker|Consultant Cardiologist|Cardiology|132000|2012-09-10|
5|Dr. Ahmed Kara|Consultant Physician|Internal Medicine|128000|2013-02-18|
6|Dr. Yusuf Cassim|Senior Registrar|Emergency & Trauma|74000|2018-05-04|
7|Michael Roberts|HR Director|Human Resources|96000|2010-11-15|
8|Susan Pretorius|HR Officer|Human Resources|32000|2016-08-23|
9|Jameel Malik|IT Systems Administrator|IT|58000|2015-04-12|
10|Thabo Molefe|Network Engineer|IT|46000|2017-10-02|
11|Nomvula Khumalo|Registered Nurse|Emergency & Trauma|34000|2016-01-19|
12|Lerato Mokoena|Registered Nurse|Pediatrics|33000|2017-06-07|
13|Bongani Ndlovu|Registered Nurse|Cardiology|35000|2015-12-01|
14|Zanele Mahlangu|Nursing Sister|Theatre|42000|2013-03-25|
15|Kagiso Sithole|Pharmacist|Pharmacy|61000|2014-09-08|
16|Naledi Zulu|Pharmacy Assistant|Pharmacy|26000|2019-02-14|
17|Themba Nkosi|Radiographer|Radiology|44000|2016-07-30|
18|Palesa Radebe|Radiographer|Radiology|43000|2017-04-11|
19|Deepak Pillay|Lab Technologist|Diagnostics Lab|41000|2015-05-20|
20|Kavitha Govender|Lab Technician|Diagnostics Lab|35000|2018-08-06|
21|Dr. Suresh Moodley|Consultant Radiologist|Radiology|130000|2012-02-28|
22|Dr. Fatima Patel|Pediatrician|Pediatrics|118000|2013-10-17|
23|Nisha Singh|Physiotherapist|Rehabilitation|48000|2016-11-09|
24|Dr. Vikram Chetty|Anaesthetist|Theatre|135000|2011-06-13|
25|David Smith|Facilities Manager|Operations|52000|2014-01-27|
26|Karen O'Connor|Billing Administrator|Finance|29000|2018-03-19|
27|James Wilson|Security Supervisor|Operations|27000|2019-09-02|
28|Linda Fourie|Receptionist|Front Office|19000|2020-02-10|
29|Peter van Wyk|Procurement Officer|Supply Chain|38000|2015-08-24|
30|Andile Mbeki|Ward Clerk|Administration|21000|2019-11-05|

---

### Shareholders

|ID (`id`)|Shareholder Name (`shareholder_name`)|Share Percent (`share_percent`)|Shares Held (`shares_held`)|Share Class (`share_class`)|
-----|-------------------|------------------|---------|---------|
1|Dr. Rajesh Naidoo|18.0|180000|Ordinary|
2|Cedar Health Holdings (Pty) Ltd|15.0|150000|Ordinary|
3|Dr. Johan van der Merwe|12.0|120000|Ordinary|
4|Reddy Family Trust|11.0|110000|Ordinary|
5|Thabo Molefe|10.0|100000|Ordinary|
6|Sarah Botha|9.0|90000|Ordinary|
7|Dr. Ahmed Kara|8.0|80000|Preferential|
8|Naledi Zulu|7.0|70000|Ordinary|
9|Michael Roberts|6.0|60000|Ordinary|
10|Dr. Vikram Chetty|4.0|40000|Preferential|


---

# 4. 💎 Risk Rating

Based on the information collected during the penetration testing activities, I identified the following potential risks.

[**OWASP resources**](#-tools--resources) were used for risk classification and rating.

---

## Risk evaluation criteria

**Likelihood and Impact Levels:** 🟢 Low 🟡 Medium 🟠 High

**Risk severity levels:** 🔵 Note 🟢 Low 🟡 Medium 🟠 High 🔴 Critical


<table cellspacing="0" cellpadding="5" border="1" align="center">
<tr>
<th colspan="5" align="center">Overall Risk Severity</th>
</tr>
<tr>
<th rowspan="4" width="15%" align="center">Impact</th>
<td width="15%" align="center">HIGH</td>
<td width="15%" bgcolor="orange" align="center">Medium</td>
<td width="15%" bgcolor="red" align="center">High</td>
<td width="15%" bgcolor="pink" align="center">Critical</td>
</tr>
<tr>
<td align="center">MEDIUM</td>
<td bgcolor="yellow" align="center">Low</td>
<td bgcolor="orange" align="center">Medium</td>
<td bgcolor="red" align="center">High</td>
</tr>
<tr>
<td align="center">LOW</td>
<td bgcolor="lightgreen" align="center">Note</td>
<td bgcolor="yellow" align="center">Low</td>
<td bgcolor="orange" align="center">Medium</td>
</tr>
<tr>
<td align="center">&nbsp;</td>
<td align="center">LOW</td>
<td align="center">MEDIUM</td>
<td align="center">HIGH</td>
</tr>
<tr>
<td align="center">&nbsp;</td>
<th colspan="4" align="center">Likelihood</th>
</tr>
</table>
<br/>

---

## Risk Severity Classification

|Rating|	Description|	Management Attention|
|------------|----|-----|
|🔴 Critical	|Immediate risk of unauthorized access, large-scale data exposure, or significant business impact.	|Immediate remediation required (0-48 Hours)
|🟠 High	|Serious weakness that could lead to compromise of sensitive assets.	|Remediate as a priority (1-2 Weeks)
|🟡 Medium|Exploitable weakness with limited scope or requiring additional conditions.|Planned remediation (3-5 Weeks)
|🟢 Low	|Security weakness with limited impact or exploitability.	|Monitor and address during normal maintenance (Ongoing)
|🔵 Note |Very low impact security notification|Document and monitor 

---

## Risk rating

|ID|Finding|	OWASP Category|Likelihood|	Impact	|Risk Rating|
|---|---|----------|-----------|------|-------|
|1	|Weak Passwords Protecting Encrypted Reports	|A07 Identification and Authentication Failures	|🟠 High|🟠 High|	🔴 Critical
|2|Publicly Accessible Legacy Database Backup	|A01 Broken Access Control / A02 Security Misconfiguration|🟠 High|🟠 High	|🔴 Critical
|3	|SQL Injection in Patient Portal Authentication|A05 Injection	|🟠 High|🟠 High|	🔴 Critical
|4	|Unauthorized Access to Confidential Patient Reports|A01 Broken Access Control|🟠 High|🟠 High	|🔴 Critical
|5|	No Account Lockout or Rate Limiting|	A07 Identification and Authentication Failures|🟠 High|	🟠 High|	🟠 High
|6	|Username Enumeration Through Authentication Messages|A07 Identification and Authentication Failures|🟠 High	|🟡 Medium|🟠 High
|7|	Directory Listing Enabled on Patient Portal	|A02 Security Misconfiguration|🟠 High|🟡 Medium	|🟠 High
|8	|Sensitive Directory Disclosure via robots.txt	|A02 Security Misconfiguration|🟡 Medium|🟡 Medium|🟡 Medium

---

# 5. 💎 Recommendations and Remediation

Based on the observations from these activities, I recommend the following security corrections and improvements.

---

## 5.1. Prioritized recommandations and remediations

The following recommendations are prioritized according to the assessed risk level and aligned with OWASP Top 10 (2025) principles. Critical findings should be addressed immediately, followed by High and Medium risk findings.

|ID|	Finding|	Risk	|Recommendations|Remediation|Actions|
|-----|------|-------|----------|---------|------|
|1	|Weak Passwords Protecting Encrypted Reports	|🔴 Critical	|Strengthen protection of sensitive documents and stored records.	|Enforce strong password requirements. Block passwords found in known breach datasets and common password dictionaries. Add multi-factor authentication for the patient portal and administrative access. Consider centralized document access controls rather than separate document passwords. Require minimum length and complexity standards. Assess breach notification obligations to the data protection authority and affected individuals.|0-48 Heures
|2	|Publicly Accessible Legacy Database Backup	|🔴 Critical	|Eliminate public exposure of sensitive business and personal data.	|Immediately remove backup files from web-accessible locations. Store backups outside the web root. Restrict access using file system permissions. Review exposure logs and assess potential data compromise. Implement backup management and retention policies.|0-48 Heures
|3	|SQL Injection in Patient Portal Authentication	|🔴 Critical	|Eliminate injection vulnerabilities from all application components.	|Replace dynamic SQL statements with parameterized queries and prepared statements. Validate and sanitize user input server-side. Perform secure code review and vulnerability testing across all database interactions.|0-48 Heures
|4	|Unauthorized Access to Confidential Patient Reports	|🔴 Critical	|Ensure sensitive medical information is accessible only to authorized users.	|Review and redesign authorization controls. Enforce server-side access validation for every request. Implement role-based access control (RBAC) and verify authorization before granting access to reports.|0-48 Heures
|5	|No Account Lockout or Rate Limiting	|🟠 High	|Reduce the effectiveness of credential guessing and password attacks.|	Implement rate limiting, account lockout policies, progressive delays, and monitoring for repeated authentication failures. Consider CAPTCHA protection after multiple failed attempts.|1-2 Weeks
|6	|Username Enumeration Through Authentication Messages	|🟠 High	|Prevent attackers from identifying valid accounts.	|Replace detailed authentication errors with generic responses such as "Invalid username or password." Ensure identical responses are returned regardless of whether a username exists.|1-2 Weeks
|7|Directory Listing Enabled on Patient Portal	|🟠 High	|Prevent disclosure of application structure and internal resources.	|Disable directory indexing on the web server. Configure Apache/Nginx/IIS to deny directory browsing. Implement least-privilege access controls on application directories.|1-2 Weeks
|8	|Sensitive Directory Disclosure via robots.txt	|🟡 Medium	|Minimize information disclosure through publicly accessible configuration files.|	Remove references to sensitive, legacy, administrative, or restricted directories from robots.txt. Ensure sensitive resources are protected through access controls rather than obscurity. Review all publicly exposed metadata files.|3-5 Weeks

---

## 5.2. Other recommandations

1.  **Review publicly exposed technology information**  
    Organizations should regularly review what information about their web technologies.

2.  **Keep software updated**  
    CMS platforms, plugins and other web technologies should be regularly updated and reviewed against current security advisories.

3.  **Review HTTP headers**  
    HTTP response headers should be reviewed regularly to determine whether unnecessary technical information is being exposed.

4.  **Review DNS records regularly**  
    DNS records should be checked periodically to ensure that only required information and services are publicly exposed.

5.  **Properly configure and monitor the WAF**  
    Keep the WAF (LiteSpeed) enabled and tuned.

6.  **Perform regular internal network discovery**  
    Organizations should periodically scan their own networks to identify active devices.

7.  **Investigate unknown devices**  
    Any unexpected device discovered during network scanning should be investigated and verified.

8.  **Maintain network documentation**  
    Network topology and device information should be documented and updated regularly.

9.  **Perform security testing with authorization**  
    Reconnaissance and scanning should only be performed against systems and networks where appropriate authorization has been provided.

10. **Align the hospital ISM with international standards and regulations**
    ISO/IEC 27001 and applicable healthcare and privacy regulations.

---

# 6. Conclusion

The security assessment of the Mediroza Hospital web platform identified a combination of weaknesses that collectively resulted in unauthorized access to sensitive organizational and patient information. The assessment revealed deficiencies in security configuration, access control, authentication mechanisms, input validation, and document protection controls. Most notably, critical weaknesses allowed unauthorized access to confidential patient reports and exposed sensitive business information, creating substantial risks to data confidentiality, regulatory compliance, and organizational reputation.

The findings indicate that security controls currently in place are insufficient for an environment processing sensitive healthcare and corporate information. Several vulnerabilities could be exploited by an attacker with moderate technical skills and publicly available tools, demonstrating that the application's security posture does not adequately reflect the sensitivity of the assets being protected.

Remediation efforts should prioritize the elimination of critical vulnerabilities, particularly those affecting access control, authentication, and sensitive data exposure. High-risk findings should be addressed immediately thereafter to reduce the likelihood of future compromise and strengthen the organization's overall resilience against cyber threats.

Definitively, the overall security posture of the assessed website is Critical due to the presence of multiple high-impact vulnerabilities that can be chained together to achieve unauthorized access to sensitive information. Prompt remediation, strengthened security governance, and the adoption of secure development and operational practices are strongly recommended to reduce organizational risk and improve long-term security maturity.



---

## 🏹 For more

This penetration testing project was limited to the steps mentioned above. However, a full audit would include an analysis of open ports and their potential exploitation. Running services should also be evaluated. Furthermore, various cybersecurity tools—such as OpenVAS or ZAP—could be employed to conduct a more in-depth analysis of the web platform. In this context, more listed vulnerabilities (CVE) and their CVSS scores would be detected.


---

-End-

---

# 🔗 Tools & Resources

- **Networkwalks Hash Calculator:** [https://networkwalks.com/hash-calculator/](https://networkwalks.com/hash-calculator/)
- **Networkwalks Password Cracker:** [https://networkwalks.com/password-cracker/](https://networkwalks.com/password-cracker/)
- **PTES:** [https://github.com/penetration-testing-execution-standard](https://github.com/penetration-testing-execution-standard)
- **OWASP Risk Rating Methodology:** [https://community.owasp.org/OWASP_Risk_Rating_Methodology](https://community.owasp.org/OWASP_Risk_Rating_Methodology)
- **OWASP Top 10:2025:** [https://top10.owasp.org/2025/](https://top10.owasp.org/2025/)


---

# 👤 Author

**Dickson Kenneth Chigozie**\
Cybersecurity intern B084

LinkedIn: www.linkedin.com/in/kenneth-dickson-3868631b3
---

## 📌 Project Information

**Program Name:** Cybersecurity at Networkwalks | **Week:** 04 | **Project:** Real-world Penetration Testing - Mediroza Hospital | **Repository:** GitHub

