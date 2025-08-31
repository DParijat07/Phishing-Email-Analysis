📧 Phishing Email Analysis – Case Study  

## 🔹 Executive Summary  
This project analyzes a suspicious phishing email to identify **indicators of compromise (IoCs)** and assess the threat level.  
The investigation revealed:  
- Spoofed sender address  
- Suspicious login link  
- Malicious attachment (invoice.pdf)  
- Urgent and threatening tone  

📌 **Overall Risk Rating: HIGH**  

---

## 🔹 Email Details  

| Attribute       | Value (from sample) |
|-----------------|----------------------|
| **Sender**      | support@paypall-login[.]com |
| **Recipient**   | victim@example.com |
| **Subject**     | Urgent: Verify Your Account Now! |
| **Date/Time**   | 2025-08-24 10:15 UTC |
| **Attachments** | invoice.pdf (potential malware) |
| **Links**       | hxxp://secure-paypall[.]com/login |

---

## 🔹 Phishing Indicators  

| Category   | Observation |
|------------|-------------|
| **Sender Address** | Misspelled domain “paypall” |
| **Headers** | Return-path mismatch |
| **Links** | Fake domain, not PayPal |
| **Attachments** | Suspicious PDF invoice |
| **Language** | Urgent, threatening: “Verify account immediately” |
| **Errors** | Spelling mistakes: “paypall”, “secur account” |

---

## 🔹 Risk Assessment  

| Indicator                | Risk Level |
|---------------------------|------------|
| Spoofed sender address    | 🔴 High |
| Suspicious link redirection | 🔴 High |
| Malicious attachment      | 🔴 High |
| Urgency/Threatening tone  | 🟠 Medium |
| Grammar/Spelling mistakes | 🟡 Low |

📌 **Overall Risk Rating: HIGH**  

---

## 🔹 Recommended Actions  
- ❌ Do not click links or download attachments.  
- 📩 Report email to **security@yourorg.com**.  
- 🚫 Block domain: `paypall-login[.]com`.  
- 🎓 Provide phishing awareness training.  
- 🔎 Upload email sample to SIEM for correlation and tracking.  

---

## 🔹 Interview Q&A (Quick Reference)  

**Q: What is phishing?**  
A: A social engineering attack where attackers impersonate trusted entities to steal credentials, deliver malware, or commit fraud.  

**Q: How do you identify a phishing email?**  
A: Look for spoofed/misspelled sender addresses, urgent language, suspicious links/attachments, poor grammar, mismatched URLs.  

**Q: What is email spoofing?**  
A: Forging the “From” address to make an email appear as if it came from a trusted source.  

**Q: Why are phishing emails dangerous?**  
A: They can steal credentials, deliver ransomware/malware, and enable Business Email Compromise (BEC).  

**Q: How can you verify sender authenticity?**  
A: Check email headers, validate SPF/DKIM/DMARC, hover links, cross-check with official sources.  

**Q: Tools for header analysis?**  
A: MXToolbox, Google Admin Toolbox, built-in email client header view, SIEM/SOAR tools.  

---

## 🔹 Flashcards (Cheat Sheet)  

- **Phishing =** Social engineering attack stealing credentials/money via fake trust.  
- **Red Flags =** Spoofed sender, urgent tone, fake links, poor grammar, suspicious attachments.  
- **Email Spoofing =** Forging sender address.  
- **Danger =** Credential theft, malware, ransomware, BEC.  
- **Verify =** Headers + SPF/DKIM/DMARC + link hovering.  

