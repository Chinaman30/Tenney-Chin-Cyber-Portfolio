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
Step 1: Initial Network Investigation

I began the investigation by analyzing the infected host’s IP address to identify any outbound communications.

Reviewed network logs to determine which external IP addresses the system communicated with.

Identified suspicious outbound traffic potentially related to command-and-control (C2) infrastructure.

Checked for lateral movement or additional compromised internal hosts.
Step 2: Email Analysis

Next, I investigated the origin and distribution of the malicious email.

Reviewed email logs to determine the sender and recipient.

Verified whether the malicious payload was sent to additional users.

Confirmed that only the user Tony received the malicious attachment.

Ruled out widespread phishing distribution within the organization.

This helped scope the incident and confirm it was isolated to a single endpoint.



![image alt]()![LetsDefend Case Screenshot](https://raw.githubusercontent.com/Chinaman30/Tenney-Chin-Cyber-Portfolio/9ba8cbda07e8fcef77cb077e4523fd775da1042a/Screenshot%202026-02-21%20164758.png)
Step 3: File Hash Analysis

After identifying the suspicious file, I extracted the file hash and performed integrity verification.

Retrieved the SHA256 hash of the file.

Submitted the hash to threat intelligence platforms.

Confirmed the file was flagged as malicious.

This validated that the file was malware and not a false positive.
Step 4: Threat Intelligence & C2 Investigation

I then pivoted to deeper malware analysis:

Reviewed file metadata and behavior.

Identified potential additional payloads dropped by the malware.

Investigated associated Command-and-Control (C2) servers.

Checked for known indicators of compromise (IOCs).

Correlated findings with threat intelligence sources.

This helped determine the attacker’s infrastructure and possible impact.

![image alt]()![LetsDefend Case Screenshot](https://raw.githubusercontent.com/Chinaman30/Tenney-Chin-Cyber-Portfolio/3013b06e7d28fcbc10f80199ce85b1113de71020/Screenshot%202026-02-21%20171117.png)
Step 5: Containment

Once the investigation confirmed malicious activity:

The infected host was contained.

Further communication with external C2 servers was blocked.

Additional monitoring was enabled to detect related activity.
