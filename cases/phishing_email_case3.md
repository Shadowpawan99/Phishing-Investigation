# 🚨 Case Study: Phishing Email - Suspicious Task Scheduler  
**📅 Date:** March 21, 2021  
**🎯 Target:** `mark@letsdefend.io`  
**📩 Subject:** `COVID19 Vaccine`    
**📌 Device Action:** Blocked  

---

## 🔍 Investigation Steps  
### 1️⃣ **Email Header Analysis**  
- **SMTP Server:** `189.162.189.159`  
- **Sender:** `aaronluo@cmail.carleton.ca` (Possible spoofing)  

### 2️⃣ **Suspicious Email Content**  
- **Topic:** COVID-19 vaccine (common phishing lure).  
- **Possible Phishing Indicators:**
- Urgent language.
- No official branding or contact details.
- Encourages user to click a link or open an attachment.

### 3️⃣ **Indicators of Compromise (IoCs)**  
| **Indicator** | **Description** |
|--------------|----------------|
| `189.162.189.159` | Malicious SMTP Server |
| `cmail.carleton.ca` | Possible Spoofed Domain |
| `Task Scheduler Activity` | Potential Execution of Malicious Script |

### 🛡️ **Mitigation Steps**  
✅ Block SMTP server 189.162.189.159  
✅ Check if other users received similar emails  
✅ Educate employees about COVID-19 vaccine phishing scams  
✅ Ensure Task Scheduler execution logs are monitored 

---

📌 **Back to Main Page**: [🔙 Home](../README.md)  
