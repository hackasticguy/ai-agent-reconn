# 🛡️ AI Security Reconnaissance Agent

> **An AI-powered Security Reconnaissance Automation Workflow built with n8n, OpenAI, and multiple OSINT intelligence sources.**

Automatically collect reconnaissance data, correlate intelligence using AI, calculate a security risk score, generate professional reports, upload them to Google Drive, and notify your team on Discord—all from a single automated workflow.

![License](https://img.shields.io/badge/License-MIT-green)
![n8n](https://img.shields.io/badge/Built%20With-n8n-orange)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4.1--Mini-blue)
![Status](https://img.shields.io/badge/Status-Production%20Ready-success)

---

## 📌 Project Overview

Reconnaissance is one of the most important phases of a security assessment, but collecting intelligence from multiple OSINT platforms manually is repetitive and time-consuming.

This project automates that entire process.

The workflow gathers intelligence from multiple trusted sources, combines the results, uses AI to analyze security posture, calculates an overall risk score, and produces professional reports in multiple formats.

The generated reports are automatically uploaded to Google Drive, while a summary is delivered to Discord for quick review.

This project demonstrates how modern AI can be integrated into cybersecurity automation workflows to improve efficiency and reduce repetitive manual tasks.

---

# ✨ Features

- 🤖 AI-powered reconnaissance analysis
- 🌍 Multi-source OSINT intelligence collection
- 🌐 WHOIS lookup
- 📡 DNS Enumeration
  - A Records
  - MX Records
  - TXT Records
  - NS Records
- 🛡️ VirusTotal intelligence
- 🔍 Shodan integration
- 🌎 Censys search
- 🚨 AlienVault OTX lookup
- 🔗 URLScan analysis
- 📊 AI-generated Risk Score
- 📝 Executive Summary
- 💡 AI-generated Recommendations
- 📄 HTML Report
- 📑 PDF Report
- 📘 Markdown Report
- 📦 JSON Report
- ☁️ Google Drive Upload
- 💬 Discord Notification
- ⚡ Fully automated workflow using n8n

---

# 🏗️ Architecture

```text
                 Target Domain
                       │
                       ▼
            Normalize & Validate
                       │
                       ▼
        ┌──────────────────────────────┐
        │      Reconnaissance APIs     │
        ├──────────────────────────────┤
        │ WHOIS                        │
        │ Google DNS                   │
        │ VirusTotal                   │
        │ Shodan                       │
        │ Censys                       │
        │ AlienVault OTX               │
        │ URLScan                      │
        └──────────────────────────────┘
                       │
                       ▼
           Aggregate Reconnaissance Data
                       │
                       ▼
              OpenAI AI Correlation
                       │
                       ▼
          Professional Security Report
                       │
          ┌────────────┴────────────┐
          ▼                         ▼
   Google Drive Upload      Discord Notification
```

---

# 🛠️ Technology Stack

| Category | Technology |
|----------|------------|
| Workflow Automation | n8n |
| AI Analysis | OpenAI GPT-4.1 Mini |
| Programming | JavaScript |
| WHOIS | API Ninjas |
| DNS | Google Public DNS |
| Threat Intelligence | VirusTotal |
| Internet Intelligence | Shodan |
| Search Engine | Censys |
| Threat Intelligence | AlienVault OTX |
| URL Intelligence | URLScan |
| PDF Generation | PDFShift |
| Cloud Storage | Google Drive |
| Notifications | Discord |

---

# 📂 Repository Structure

```text
ai-agent-reconn/

├── workflow/
│   ├── security-recon-agent.json
│   └── README.md
│
├── docs/
│   └── architecture.png
│
├── Screenshots/
│   ├── workflow.png
│   ├── execution.png
│   ├── html-report.png
│   ├── pdf-report.png
│   └── discord-notification.png
│
├── report/
│   ├── sample-report.html
│   ├── sample-report.md
│   ├── sample_report.json
│   └── sample_report.pdf
│
├── README.md
├── LICENSE
└── CHANGELOG.md
```

---

# ⚙️ Workflow

The automation performs the following operations:

1. Validate target
2. WHOIS lookup
3. DNS enumeration
4. VirusTotal analysis
5. Shodan lookup
6. Censys search
7. AlienVault OTX lookup
8. URLScan search
9. Aggregate findings
10. AI correlation
11. Risk scoring
12. Professional report generation
13. Google Drive upload
14. Discord notification

---

# 📊 Generated Reports

Each execution automatically generates:

- HTML Report
- PDF Report
- Markdown Report
- JSON Report

Every report includes:

- Executive Summary
- Risk Score
- AI Analysis
- DNS Information
- WHOIS Details
- Threat Intelligence
- Security Findings
- Recommendations

---

# 📸 Screenshots

> Add screenshots inside the **Screenshots** folder.

Suggested screenshots:

- Workflow
- Successful Execution
- Discord Notification
- HTML Report
- PDF Report

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/your-username/ai-agent-reconn.git
```

Import the workflow into n8n.

Configure your API credentials.

Update the target domain.

Execute the workflow.

---

# 🔑 Required Credentials

Configure the following services inside n8n:

- OpenAI
- API Ninjas
- VirusTotal
- Shodan
- Censys
- AlienVault OTX
- URLScan
- Google Drive
- Discord
- PDFShift

> No credentials or API keys are included in this repository.

---

# 🎯 Learning Outcomes

This project helped me gain hands-on experience with:

- Security Automation
- AI-assisted Security Analysis
- Workflow Orchestration
- OSINT Collection
- API Integration
- Threat Intelligence
- Report Automation
- Cloud Integrations
- n8n Development

---

# 🚀 Future Roadmap

Planned improvements include:

- Web dashboard
- Authentication
- Scheduled scans
- Email report delivery
- IOC enrichment
- CVE intelligence
- SIEM integration
- Docker deployment
- Scan history database
- Multi-user support

---

# ⚠️ Educational Disclaimer

This project has been developed for **educational purposes, cybersecurity learning, portfolio demonstration, security research, and authorized security assessments only**.

The workflow performs **passive OSINT-based reconnaissance** by collecting publicly available information from trusted third-party services. It does **not** perform exploitation, privilege escalation, brute-force attacks, denial-of-service attacks, malware deployment, or any destructive activity.

Always obtain proper authorization before scanning domains, IP addresses, or infrastructure that you do not own or manage.

The author assumes no responsibility for misuse or unauthorized use of this project.

---

# 📄 License

Licensed under the **MIT License**.

See the LICENSE file for more information.

---

# 👨‍💻 Author

## Anubhav

**Bachelor of Computer Applications (Hons.)**

Cybersecurity • SOC • Penetration Testing • Security Automation • AI Agents • n8n

⭐ If you found this project useful, consider giving it a star.
