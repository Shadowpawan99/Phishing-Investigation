🚨 Phishing Investigation Report
📅 Date: March 22, 2021
🎯 Target: ellie@letsdefend.io
📩 Email Subject: N/A (Phishing URL Detection)
🔗 Suspicious URL: http://mogagrocol.ru/wp-content/plugins/akismet/fv/index.php?email=ellie@letsdefend.io
🛑 Device Action: Allowed

1️⃣ Email Header Analysis
This alert was triggered due to a phishing URL detected in a web request. The destination domain (mogagrocol.ru) is suspicious and has been flagged for phishing activities.

Findings:
✅ The domain mogagrocol.ru is not associated with any legitimate service.
✅ The URL path contains "wp-content/plugins/akismet/fv/index.php", which mimics a WordPress plugin directory, a common phishing or malware hosting technique.
✅ The email ellie@letsdefend.io is included in the URL query, indicating possible data harvesting.

2️⃣ URL Analysis & Threat Intelligence
The URL was checked against threat intelligence sources like VirusTotal, URLScan.io, and OpenPhish.

Threat Intelligence Results:
VirusTotal: 🚨 Flagged as Phishing

URLScan.io: 🚨 Redirects to a fake login page

Reputation Score: High Risk (Blacklisted)

3️⃣ Network & Endpoint Investigation
Since the phishing link was accessed, logs were reviewed to see if:

The user clicked the link.

A download or credential input occurred.

A connection to a known malicious IP was made.

Findings:
✅ The request was successful, meaning the phishing page was loaded.
✅ Destination IP (91.189.114.8) is blacklisted.
✅ User-Agent logs indicate the request was made from Chrome 79, which is outdated and potentially vulnerable to exploits.

4️⃣ Indicators of Compromise (IoCs)
Indicator	Type	Status
mogagrocol.ru	Phishing Domain	🚫 Blacklisted
91.189.114.8	Malicious Server IP	🚫 Blocked
172.16.17.49	Infected User’s System	🟡 Under Investigation
5️⃣ Mitigation & Prevention Steps
✅ Block the domain mogagrocol.ru on all security gateways.
✅ Blacklist 91.189.114.8 in firewall and IDS/IPS rules.
✅ Check if Ellie entered credentials on the phishing page.
✅ Enforce MFA on Ellie’s account to prevent credential-based attacks.
✅ Educate employees about phishing and social engineering tactics.

6️⃣ Conclusion
This phishing attempt targeted Ellie using a malicious URL. The domain is known for phishing, and the request was successfully made from the user's system, posing a high security risk. Immediate action is needed to block the threat and secure the affected user’s credentials.

📌 Back to Home: 🔙 README.md

