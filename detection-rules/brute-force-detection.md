# Brute Force Login Detection

## Scenario
This investigation simulates a brute-force attack against a Windows system using repeated failed logon attempts.

## Detection Clues
- Multiple failed login attempts
- Same username targeted repeatedly
- Repeated login failures within a short time
- Event ID 4625 observed in Windows Security logs

## Indicators
- Event ID: 4625
- Repeated source IP or host
- High frequency of failed login attempts

## Analyst Notes
Repeated failed logon events may indicate brute-force activity or password spraying. This should be investigated by reviewing affected accounts, timestamps, source systems, and any successful logons that followed.

## Response Actions
- Review affected user accounts
- Check if any successful logins occurred after repeated failures
- Block suspicious source IP if identified
- Enforce MFA
- Reset compromised credentials if necessary

## MITRE ATT&CK
- T1110 – Brute Force
