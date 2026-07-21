# Documentation

This directory contains the technical documentation for the **AI Security Recon Agent**.

## Contents

| File | Description |
|------|-------------|
| `ai-analysis-prompt.md` | The complete AI prompt used by the n8n AI Agent to analyze reconnaissance data and generate structured security assessments. |
| `architecture.md` *(Future)* | Project architecture, workflow design, and data flow documentation. |

## Purpose

The documentation in this folder explains how the AI Security Recon Agent works, including its analysis logic, prompt design, and workflow architecture.

## AI Analysis

The AI prompt is designed to:

- Analyze reconnaissance data from multiple OSINT sources
- Generate evidence-based security findings
- Calculate a risk score (0–10)
- Assign an overall risk level
- Produce actionable remediation recommendations
- Return structured JSON for automated report generation

## Technologies

- n8n
- OpenAI
- OSINT APIs
- JSON
- Markdown

---

**Note:**  
This documentation is intended for educational purposes and to help developers understand the AI analysis workflow used in this project.
