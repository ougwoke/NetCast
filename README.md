**NETCAST (OSS FREE VERSION)**

NetCast is a lightweight, high-performance command-line interface (CLI) mail forensics and domain threat auditing utility designed for security analysts and network administrators. It automates local infrastructure diagnostics, validates essential email authentication postures, and conducts passive WHOIS footprinting entirely from the terminal.

![System Interface](images/image1.png)

🚀 **Key Features**

• Advanced DNS Auditing: Resolves and displays structural namespace mapping including A, AAAA, and NS records.

• Email Security Posture Validation: Parses live text data or direct file inputs to analyze infrastructural alignment against SPF and DMARC policies.

• Passive Open-Source Intelligence (OSINT): Queries domain age vectors, registration lifecycles, and registrar origins via raw WHOIS data scraping.

• Console-Native Risk Scoring: Computes instant threat visibility calculations dynamically formatted directly to the terminal screen.

    
📋 **System Prerequisites**

NetCast is engineered to operate cross-platform across modern Linux distributions (tested on Kali Linux), and Windows environments running Python 3.8+.

🔧 **Installation & Configuration**

    1. Clone the Source Repository:
       ```bash
          git clone [https://github.com/ougwoke/NetCast.git](https://github.com/ougwoke/NetCast.git)
          cd NetCast
       
       How to do it:
       
       * Open your terminal (like the Kali Linux terminal you are using).
       * Copy the URL link of NetCast
       * Type git clone followed by that link and press Enter.

2. **Deploy Local Dependencies:**

Install the required foundational Python packages utilizing pip:

       * pip install -r requirements.txt (On Linux & Windows)
       * pip3 install -r requirements.txt (On macOS)  

Note: for Kali Linux / Ubuntu Users:
If you encounter an externally-managed-environment error, you can safely bypass it by forcing the installation to your user profile:

       * pip install -r requirements.txt --break-system-packages

Alternatively create a virtual environmentand run:

       * python3 -m venv venv && source venv/bin/activate
       * pip install -r requirements.txt
       * python3 netcast
  
   If you are passing an email file path use:

       * python3 netcast_core suspicious_email.eml (On linux & macOS)
       * python netcast_core C:\path\to\suspicious_email.eml


💻 **Operational Usage**

Execute the primary forensic file directly from your terminal session:

       * python3 netcast_core (linux & macOS)
       * python netcast_core (Windows) 


3. **Sample Terminal Execution Output**
   
   Scan Domain
   
   Scan Email Texts (Multi-line Input Supported)
   
   Scan Email File (.eml)
   
   Exit
   
   Select option (1-4): 1
   
   Enter domain: targetdomain.com

   Scan Verdict: LEGITIMATE (Score: 0/100)
 - DNS record types found: A, AAAA, NS
 - A records resolved successfully: 142.250.181.142
 - NS records found: ns1.targetdomain.com, ns2.targetdomain.com
 - SPF Record Found: "v=spf1 include:_spf.targetdomain.com ~all"
 - DMARC Policy Found: "v=DMARC1; p=reject;"
 - Registrar: MarkMonitor, Inc.
 - Country of Registration: US
 - Risk Severity: Low




🌟 **PREMIUM VERSION (WHAT MAKS PREMIUM ELITE):**

1. GLOBAL THREAT INTELLIGENCE INTEGRATION: Features a dynamic, isolated API module mapping directly against global reputation aggregates (VirusTotal) for zero-day URL and malicious infrastructure cross-referencing.
2. AUTOMATED JSON TELEMETRY ARCHIVING: Every scan automatically commits structured JSON log payloads down to local disk space for enterprise compliance logging.
3. EXECUTIVE HTML POSTURE DASHBOARD GENERATOR: Includes an independent compilation engine that crawls your log database to render production-ready, beautiful HTML dashboards reflecting your daily, weekly, monthly, and yearly enterprise risk trends.

📦 **WHAT IS INCLUDED IN YOUR COMMERCIAL PACK:**
* netcast_tool (Fully Compiled, Self-Contained High-Performance Executable)
* dashboard_generator (Plain-Text Adaptable HTML Reporting Engine Script)
* .env (Global Context Token Environment Template)
* SETUP_GUIDE.txt (Granular, Step-by-Step Security Deployment Manual)

Stop copy-pasting terminal readouts into Notepad. Deploy NetCast Premium, generate professional corporate dashboard reports, and maximize your client delivery standards today!


📊**PRACTICAL DEMO & EXECUTIVE REPORTING**

1. MODULE PREVIEW: DOMAIN AUDIT (CLI & REPORT ALIGNMENT) 
Run the Tool (NetCast)

![System Interface](images/image1.png)

![System Interface](images/image2.png)

![System Interface](images/image3.png)

![System Interface](images/image4.png)

![System Interface](images/image5.png)

2. MODULE PREVIEW: EMAIL_TEXT AUDIT
   
→ Paste email texts

→ Type done on the next line

→ Hit Enter

![System Interface](images/image6.png)


3. MODULE PREVIEW: EMAIL_FILE AUDIT (DEEP CONTEXT FORENSICS)

![System Interface](images/image7.png)

![System Interface](images/image8.png)


4. COMPLIANCE ENGINE: MASTER POSTURE OVERVIEW PANEL
   
To generate your weekly/monthly/yearly reports:
 Run: python3 dashboard_generator on your Terminal (where your packs are sitting) and you see all your reports drop in your directory.

![System Interface](images/image9.png)

![System Interface](images/image10.png)


MIT LICENSE + LEGAL DISCLAIMER & TERMS OF USE
=============================================


MIT LICENSE 
============

Copyright (c) 2026 Ugwoke Oliver Igwenagum

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


LEGAL DISCLAIMER & TERMS OF USE
================================

NetCast is developed strictly for educational, administrative, defensive security research, and authorized forensic auditing purposes. 

1. AUTHORIZATION REQUIRED: Users must ensure they have explicit, written authorization from the respective infrastructure owners before performing any audits or threat intelligence processing using this utility. Unsanctioned querying or infrastructure mapping against target networks may violate local and international cybercrime laws.

2. WARRANTY & LIABILITY: The developer assumes zero liability and is not responsible for any misuse, disruptions, data leaks, service degradation, or collateral damage caused by the application or execution of this software. 
