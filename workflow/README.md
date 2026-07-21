# AI Reconnaissance Agent Workflow

This directory contains the n8n workflow used by the AI Security Reconnaissance Agent.

## Workflow File

- `security-recon-agent.json`

## What the Workflow Does

The workflow automates the complete reconnaissance and reporting process.

### Workflow Steps

1. Manual Trigger
2. Target Normalization & Validation
3. WHOIS Lookup
4. DNS Enumeration
   - A Records
   - MX Records
   - TXT Records
   - NS Records
5. VirusTotal Domain Analysis
6. Shodan DNS Lookup
7. Censys Host Search
8. AlienVault OTX Intelligence
9. URLScan Search
10. Aggregate Reconnaissance Data
11. AI Risk Correlation (OpenAI GPT-4.1 Mini)
12. Report Generation
    - HTML
    - Markdown
    - JSON
    - PDF
13. Google Drive Upload
14. Discord Notification

## Required Credentials

Before running the workflow, configure your own credentials in n8n.

Required services:

- OpenAI
- API Ninjas (WHOIS)
- VirusTotal
- Shodan
- Censys
- AlienVault OTX
- URLScan
- Google Drive
- Discord Bot
- PDFShift

No API keys or credentials are included in this repository.

## Import Instructions

1. Open n8n.
2. Select **Import Workflow**.
3. Import `security-recon-agent.json`.
4. Configure all required credentials.
5. Update the Manual Test Config node with your target.
6. Execute the workflow.

## Output

The workflow automatically generates:

- HTML Report
- Markdown Report
- JSON Report
- PDF Report

The reports are uploaded to Google Drive and a summary is sent to Discord.

## Disclaimer

This workflow is intended for **authorized security assessments, learning, and research purposes only**.

Always obtain proper authorization before scanning any third-party systems.
