# Brute Force Incident Report

## Incident Title
Suspected Brute Force Login Activity on Windows Endpoint

## Summary
Multiple failed login attempts were observed against a Windows endpoint over a short period. The activity is consistent with brute-force or password spraying behavior.

## Evidence
- Windows Security Event ID 4625
- Repeated failed login attempts
- High frequency of authentication failures

## Impact
Potential unauthorized access attempt against user accounts.

## Investigation Steps
1. Reviewed failed login events in Event Viewer
2. Identified repeated login failures tied to the same account
3. Checked for any successful login after repeated failures
4. Assessed whether the source appeared internal or external

## Findings
The log pattern strongly suggests credential attack activity.

## MITRE ATT&CK Mapping
- T1110 – Brute Force

## Containment Recommendations
- Enable account lockout policy
- Enforce multi-factor authentication
- Reset affected passwords
- Monitor for follow-up login attempts

## Lessons Learned
Repeated Event ID 4625 entries can be an early indicator of brute-force or password spraying attacks and should be monitored closely.
