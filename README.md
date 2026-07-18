# SecSCan

> **AI-Powered Automated Web Application Security Assessment Framework**

SecSCan is an intelligent web application security assessment framework developed as a senior graduation project. It automates the penetration testing workflow by combining traditional security tools with AI-assisted analysis to perform comprehensive reconnaissance, crawling, technology fingerprinting, and vulnerability assessment.

The framework is designed to reduce manual effort during security assessments while providing accurate, organized, and actionable results through an intuitive web interface.

---

## Features

- Automated Web Application Reconnaissance
- Subdomain Enumeration
- Active Host Verification
- Technology Fingerprinting
- Frontend Framework Detection
- Web Application Firewall (WAF) Detection
- WHOIS Information Gathering
- Recursive Web Crawling
- URL & Endpoint Discovery
- Form Discovery
- JavaScript Asset Discovery
- AI-Assisted Vulnerability Analysis
- Security Report Generation
- Interactive Web Dashboard

---

# 📸 Screenshots

## Home Page
> **<<img width="886" height="442" alt="image" src="https://github.com/user-attachments/assets/a7f27962-00fc-44e6-b5e0-7030361df9f8" />
" />**

## Dashboard

> **<img width="1600" height="1100" alt="WhatsApp Image 2026-07-01 at 12 54 38 AM" src="https://github.com/user-attachments/assets/4acd18c6-1b49-4413-b389-fc270f4fd9ba" />**


---

## Reconnaissance Results

> **<img width="1280" height="975" alt="subdomain" src="https://github.com/user-attachments/assets/115665fe-9b4d-4476-b918-7a3f2990a37d" />
<img width="1280" height="1192" alt="tech" src="https://github.com/user-attachments/assets/901debfb-8958-4ca6-8a80-70e3ca9d7545" />
<img width="722" height="699" alt="image" src="https://github.com/user-attachments/assets/e84514ee-afc2-40fc-9fa0-f1e28177d8e5" />
<img width="1258" height="1280" alt="waf" src="https://github.com/user-attachments/assets/c9bef663-11e0-431e-bbd4-3d0fc6d4f692" />
<img width="1271" height="1280" alt="port" src="https://github.com/user-attachments/assets/acbacf8c-1e37-4807-abdf-c8c65fa9affe" />**



---

## Crawling Results

> **Place a screenshot showing discovered URLs, Forms, and Buttons**

```markdown
![Crawler Results](images/crawler-results.png)
```

---

## Vulnerability Assessment

> **Place a screenshot showing the vulnerability scanning results**

```markdown
![Vulnerability Assessment](images/vulnerability-results.png)
```

---

## Generated Report

> **Place a screenshot of the final generated report**

```markdown
![Report](images/report.png)
```

---

# 🏗️ System Architecture

```
                +----------------+
                |   User Input   |
                +--------+-------+
                         |
                         ▼
             +-----------------------+
             | Reconnaissance Stage  |
             +-----------+-----------+
                         |
      +------------------+------------------+
      |                  |                  |
      ▼                  ▼                  ▼
Subdomains       Technology Scan       WHOIS
Enumeration      & Fingerprinting
      |                  |                  |
      +------------------+------------------+
                         |
                         ▼
              Reachable Targets
                         |
                         ▼
                Crawling Engine
                         |
                         ▼
      URLs • Forms • Buttons • Parameters
                         |
                         ▼
         Vulnerability Assessment Engine
                         |
                         ▼
              AI Analysis & Classification
                         |
                         ▼
               Security Assessment Report
```

---

# ⚙️ Workflow

```
Target Domain
      │
      ▼
Subdomain Enumeration
      │
      ▼
Active Host Verification
      │
      ▼
Technology Detection
      │
      ▼
Frontend Detection
      │
      ▼
WAF Detection
      │
      ▼
WHOIS Collection
      │
      ▼
Recursive Crawling
      │
      ▼
URL & Form Discovery
      │
      ▼
Vulnerability Assessment
      │
      ▼
AI-Based Analysis
      │
      ▼
Security Report
```

---

# 📂 Project Structure

```
SecSCan/
│
├── Backend/
│   ├── Recon/
│   │   ├── ReconSubDomain.py
│   │   ├── ReconFingerprint.py
│   │   ├── ReconFrontend.py
│   │   ├── ReconWHOIS.py
│   │   ├── ReconWAF.py
│   │   └── main.py
│   │
│   ├── Crawler/
│   ├── Scanner/
│   ├── AI/
│   └── Reports/
│
├── Frontend/
│
├── Database/
│
├── images/
│
├── requirements.txt
│
└── README.md
```

---

# 🔍 Reconnaissance Modules

### Subdomain Enumeration

Discovers subdomains using Certificate Transparency Logs and validates reachable hosts before forwarding them to subsequent modules.

---

### Technology Fingerprinting

Identifies:

- Web Server
- Backend Language
- Framework
- CMS
- JavaScript Libraries
- Technology Versions

---

### Frontend Detection

Detects frontend technologies including:

- React
- Angular
- Vue.js
- Svelte
- jQuery

---

### WAF Detection

Identifies deployed Web Application Firewalls to provide better understanding of the target infrastructure before security testing.

---

### WHOIS Enumeration

Collects:

- Registrar
- Registration Date
- Expiration Date
- Name Servers

---

# 🕸️ Crawling Engine

The crawler recursively explores the target application while remaining within the target domain.

It automatically discovers:

- URLs
- Forms
- Buttons
- Parameters
- JavaScript Assets
- Input Fields
- Interactive Components

The discovered resources are then passed to the vulnerability assessment stage.

---

# 🛡️ Vulnerability Assessment

The framework evaluates discovered endpoints against common web application vulnerabilities including:

- Cross-Site Scripting (XSS)
- SQL Injection (SQLi)
- Command Injection
- Local File Inclusion (LFI)
- Broken Authentication
- Security Misconfiguration
- Sensitive Information Disclosure
- Insecure Direct Object References (IDOR)
- Cross-Site Request Forgery (CSRF)

---

# 🤖 AI Integration

SecSCan enhances traditional security testing by leveraging AI to:

- Analyze scanner outputs
- Reduce false positives
- Explain detected vulnerabilities
- Recommend remediation steps
- Generate readable security reports

---

# 💻 Technologies Used

## Backend

- Python
- Flask
- Requests
- BeautifulSoup
- Selenium
- Playwright
- AsyncIO

## Frontend

- Next.js
- React
- TypeScript
- Tailwind CSS

## Database

- MySQL
- Prisma ORM

## Security Tools

- Nmap
- WhatWeb
- Wappalyzer
- crt.sh
- Burp Suite

## AI

- OpenAI API

---

# ⚡ Installation

Clone the repository

```bash
git clone https://github.com/your-username/SecSCan.git
```

Move into the project directory

```bash
cd SecSCan
```

Install dependencies

```bash
pip install -r requirements.txt
```

Configure environment variables

```env
OPENAI_API_KEY=YOUR_API_KEY
DATABASE_URL=YOUR_DATABASE_URL
```

Run the application

```bash
python main.py
```

---

# 🎯 Future Improvements

- Authenticated Crawling
- Multi-threaded Scanning
- CVE Enrichment
- Docker Support
- PDF Report Export
- Scan Scheduling
- REST API
- Dashboard Analytics

---

# ⚠️ Disclaimer

This project was developed for educational purposes and authorized security assessments only.

Always obtain explicit permission before performing security testing against any target.

---

# 👨‍💻 Author

**Omar El Gohary**

Computer Engineering Graduate • Penetration Tester • Cybersecurity Researcher

- LinkedIn: *(Add your LinkedIn URL)*
- GitHub: *(Add your GitHub URL)*

---

# 📄 License

This project is licensed under the MIT License.
