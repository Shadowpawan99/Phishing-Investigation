# 🚨 Case Study: Phishing Email with Malicious Attachment  
**📅 Date:** January 31, 2021  
**🎯 Target:** `richard@letsdefend.io`  
**📩 Subject:** `Invoice`  
**📎 Attachment:** `c9ad9506bcccfaa987ff9fc11b91698d`  
**📌 Device Action:** Allowed  

---

## 🔍 Investigation Steps  
### 1️⃣ **Email Header Analysis**  
- **SMTP Server:** `49.234.43.39`  
- **Sender:** `accounting@cmail.carleton.ca` (Possible spoofing)  

### 2️⃣ **Attachment Analysis**  
- **File Hash:** `c9ad9506bcccfaa987ff9fc11b91698d`  
- **VirusTotal Result:** [Check Hash](https://www.virustotal.com/)  
- **Sandbox Analysis:** Detected as `Trojan.Downloader`  

### 3️⃣ **Indicators of Compromise (IoCs)**  
| **Indicator** | **Description** |
|--------------|----------------|
| `49.234.43.39` | Malicious SMTP Server |
| `mogagrocol.ru` | Phishing Domain |
| `c9ad9506bcccfaa987ff9fc11b91698d` | Malware Attachment |

### 🛡️ **Mitigation Steps**  
✅ Block SMTP server `49.234.43.39`  
✅ Quarantine all emails with similar patterns  
✅ Alert employees about similar phishing attempts  
✅ Enforce MFA on all email accounts  

---

📌 **Back to Main Page**: [🔙 Home](../README.md)  
