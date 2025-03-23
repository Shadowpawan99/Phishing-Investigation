# 🚨 Case Study: Phishing URL Detected 
**📅 Date:**  March 22, 2021  
**🎯 Target:** `ellie@letsdefend.io`  
**📩 Subject:** `Invoice`  
**🔗 Suspicious URL:** `http://mogagrocol.ru/wp-content/plugins/akismet/fv/index.php?email=ellie@letsdefend.io`  
**📌 Device Action:** Allowed  

---

## 🔍 Investigation Steps  
### 1️⃣ **Email Header & Network Analysis**  
- **Source IP**: 172.16.17.49 (Ellie's Computer - EmilyComp)  
- **Destination IP**: 91.189.114.8 (Phishing Server - mogagrocol.ru)
- **User-Agent**: Mozilla/5.0 (Windows NT 6.1; Win64; x64) Chrome/79.0.3945.88  

### 2️⃣ **Phishing URL Analysis**  
- **Domain Reputation**: 🚨 Blacklisted (Confirmed Phishing Site)
- **VirusTotal Result**: Check URL
- **URLScan.io Analysis**: Redirects to fake login page (Credential Harvesting) 

### 3️⃣ **Indicators of Compromise (IoCs)**  
| **Indicator** | **Description** |
|--------------|----------------|
| `mogagrocol.ru` | Phishing Domain |
| `91.189.114.8` | Malicious Server Hosting Phishing Page |
| `172.16.17.49` | Infected User’s System (EmilyComp) |

### 🛡️ **Mitigation Steps**  
✅ Blacklist the domain mogagrocol.ru at DNS level
✅ Block 91.189.114.8 on firewall and security tools
✅ Investigate if Ellie entered credentials on the phishing site
✅ Enforce Multi-Factor Authentication (MFA) on her account
✅ Educate employees about phishing awareness  

---

📌 **Back to Main Page**: [🔙 Home](../README.md)  
