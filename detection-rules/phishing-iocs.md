# Phishing IOC Analysis

## Scenario
This case reviews a suspicious email for phishing indicators and extracts relevant IOCs.

## Indicators Reviewed
- Sender email address
- Sender domain
- URLs in the email
- Attachment hashes
- Spoofed branding
- Urgent language

## Possible IOCs
- malicious domain
- suspicious URL
- file hash
- reply-to mismatch

## MITRE ATT&CK
- T1566 – Phishing

## Response Actions
- Block sender/domain
- Quarantine similar emails
- Reset impacted accounts
- Submit artifacts for further analysis
