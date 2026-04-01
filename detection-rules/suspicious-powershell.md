# Suspicious PowerShell Activity

## Scenario
This case investigates suspicious PowerShell execution that may indicate malicious command execution or attacker activity.

## Detection Clues
- Use of `powershell.exe`
- Encoded command execution
- Unusual parent process
- Suspicious command-line arguments

## Indicators
- `-enc`
- hidden window execution
- abnormal script behavior

## MITRE ATT&CK
- T1059.001 – PowerShell

## Response Actions
- Isolate affected host
- Review PowerShell logs
- Check for persistence mechanisms
- Inspect parent-child process relationship
