# Security Reconnaissance Report

- **Target:** hackthebox.com
- **Scan ID:** 62
- **Scanned At:** 2026-07-21T05:33:51.324Z
- **Risk Score:** 10

## Executive Summary
The domain hackthebox.com is a well-established and reputable domain with proper DNS configurations, valid SSL/TLS certificates, and no malicious detections in threat intelligence sources. However, some minor concerns related to email security and URL reputation were identified that warrant attention to maintain security posture.

## Findings

### 1. Finding — LOW

> Evidence: Domain hackthebox.com is registered with Amazon Registrar, Inc. since 2010-03-18 and is set to expire in 2027-03-18. The domain status is clientTransferProhibited.

### 2. Finding — LOW

> Evidence: DNS records show two A records (109.176.239.69, 109.176.239.70), MX records pointing to Google mail servers, and DNSSEC is enabled with signed delegation.

### 3. Finding — LOW

> Evidence: The SSL certificate for hackthebox.com is valid until 2026-10-08, issued by Google Trust Services, uses strong signature algorithm (ECDSA with secp256r1), and supports server authentication.

### 4. Finding — LOW

> Evidence: VirusTotal and other threat intelligence sources report no malicious or suspicious detections for hackthebox.com. Last analysis shows 0 malicious and 0 suspicious votes.

### 5. Finding — MEDIUM

> Evidence: The domain's SPF record is 'v=spf1 include:_u.hackthebox.com._spf.smart.ondmarc.com ~all' which uses a soft fail (~all) mechanism.

### 6. Finding — MEDIUM

> Evidence: URLScan.io data shows multiple subdomains and URLs related to hackthebox.com with high traffic and legitimate content. However, some URLs (e.g., hacktheboxltd.sjv.io) redirect off-domain and may be used in affiliate or tracking campaigns.

## Remediation Recommendations
- Update SPF record to use a hard fail (-all) instead of soft fail (~all) to improve email spoofing protection.
- Continuously monitor URLs and subdomains for suspicious redirects or phishing attempts.
- Maintain regular renewal and strong configuration of SSL/TLS certificates.
- Ensure DNSSEC is fully deployed and monitored for integrity.
- Keep domain registration details up to date and monitor for unauthorized changes.

## Correlation Notes
The domain's DNS configuration, SSL/TLS certificate, and threat intelligence data collectively indicate a legitimate and secure domain. The email security finding correlates with the SPF record configuration, suggesting a potential vector for spoofing. URL reputation findings highlight the need to monitor external redirects related to the domain to prevent abuse.