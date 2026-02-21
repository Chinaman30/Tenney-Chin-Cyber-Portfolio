# TrackMe Lab 1 – Investigation Report

## Objective
Analyze system logs to detect suspicious activity and identify indicators of compromise.

## Scenario
A suspicious login attempt was detected. The goal was to determine:
- Source IP
- Affected user account
- Type of attack
- Timeline of activity

## Tools Used
- Splunk
- Windows Event Viewer
- Command Line

## Investigation Steps
1. Reviewed authentication logs
2. Filtered for failed login attempts
3. Identified repeated attempts from same IP
4. Correlated timestamp activity

## Findings
- Multiple failed login attempts from IP: XXX.XXX.XXX.XXX
- Targeted user account: administrator
- Activity consistent with brute force attempt

## MITRE ATT&CK Mapping
- T1110 – Brute Force

## Remediation Recommendations
- Lock account after X failed attempts
- Implement MFA
- Block malicious IP

---

## What I Learned
This lab strengthened my ability to:
- Analyze log data
- Identify attack patterns
- Document investigations clearly
