# Phishing Email Investigation

## 📌 Overview
This project investigates a real-world phishing email sample impersonating Bradesco Bank (Brazil). The analysis was performed using industry-standard SOC tools to identify malicious indicators and validate the threat.

## 🛠 Tools Used
- VirusTotal  
- MXToolbox  
- WHOIS (DomainTools)  

## 🔧 Tool Explanation
- **VirusTotal**  
  Used to analyze the sender IP address and detect malicious activity across multiple security vendors.

- **MXToolbox**  
  Used to analyze email headers, identify relay paths, and check SPF, DKIM, and DMARC authentication results.

- **WHOIS Lookup (DomainTools)**  
  Used to gather domain registration details and verify legitimacy of the sender domain.

## 🔍 Key Findings
- Email failed SPF, DKIM, and DMARC authentication checks  
- Originated from a DigitalOcean VPS server (not associated with a bank)  
- Sender domain is not related to the legitimate Bradesco Bank  
- **Final Verdict: CONFIRMED PHISHING**

## 📁 Project Structure
```
phishing-email-investigation/
│
├── README.md
├── Phishing email invest report.pdf
├── evidence/
│   ├── virustotal-ip-analysis.png
│   ├── whois-domain-lookup.png
│   ├── mxtoolbox-auth-failures.png
│   ├── mxtoolbox-relay-path.png
│   └── mxtoolbox-headers.png
└── phishing email1.eml
```
