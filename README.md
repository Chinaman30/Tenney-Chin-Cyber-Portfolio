# Tenney-Chin-Cyber-Portfolio
Cybersecurity Analyst specializing in defensive security, threat detection, soc operations.
# Cybersecurity Lab Portfolio – Tenney Chin

This repository contains hands-on cybersecurity labs demonstrating practical experience in:

- SIEM investigations
- Log analysis
  ![image alt]()![SIEM Lab Screenshot](./TrackMe-Labs/Screenshot%202026-02-21%20103045.png)
Log Review

Queried Windows Security logs for failed login attempts.

Filtered Event ID 4720 

Identified repeated login failures from a single source.
Checked for:

Brute force indicators 

Abnormal login times

Logins from unfamiliar IP addresses

Compared successful logins (Event ID 4624) following failed attempts.

Queried for suspicious process execution.

Reviewed command-line activity and parent-child process relationships.

Looked for abnormal PowerShell or CMD execution.
Findings

Detected multiple failed authentication attempts within a short time window.

Observed successful login following repeated failures.

Identified suspicious process execution post-authentication.

This behavior is consistent with potential brute-force or credential-stuffing activity.
![image alt]()![Suspicious PowerShell Investigation Screenshot](https://raw.githubusercontent.com/Chinaman30/Tenney-Chin-Cyber-Portfolio/5fbe295c053412ccf648065e10e50f2b120684bb/Screenshot%202026-02-21%20164750.png)



![image alt]()![LetsDefend Case Screenshot](https://raw.githubusercontent.com/Chinaman30/Tenney-Chin-Cyber-Portfolio/9ba8cbda07e8fcef77cb077e4523fd775da1042a/Screenshot%202026-02-21%20164758.png)
