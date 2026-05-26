# FUTURE_CS_02 — Phishing Email Detection & Awareness Report

**Future Interns · Cyber Security Internship · Task 2**  
CIN: `FIT/APR26/CS8070` · Intern: Romano · Date: 05 May 2026

---

## 🎯 Overview

This repository contains the deliverables for **Task 2** of the Future Interns Cyber Security internship:  
a **Phishing Email Detection & Awareness Report** analysing real phishing patterns and providing employee awareness guidance.

---

## 📊 Analysis Summary

| Email | Subject (Summary) | Verdict | Risk |
|---|---|---|---|
| E-01 | Urgent: Account Will Be Locked | 🔴 PHISHING | HIGH |
| E-02 | PayPal Payment of $847 Processed | 🔴 PHISHING | HIGH |
| E-03 | IT Dept: Mandatory Password Reset | 🔴 PHISHING | HIGH |
| E-04 | Pending Package Delivery | 🟡 SUSPICIOUS | MEDIUM |
| E-05 | GitHub Actions Workflow Completed | 🟢 SAFE | LOW |

**3 Phishing · 1 Suspicious · 1 Legitimate (comparison sample)**

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| **Google Admin Toolbox** | Email header parsing and authentication analysis |
| **MXToolbox Header Analyser** | SPF / DKIM / DMARC verification |
| **Browser DevTools** | Safe URL and domain inspection |
| **VirusTotal** | Link reputation check against threat databases |
| **Public phishing datasets** | Source of educational sample emails |

---

## 🔍 Analysis Approach

1. Collected phishing email samples from public educational datasets
2. Analysed email headers using Google Admin Toolbox and MXToolbox
3. Inspected sender domains for spoofing and typosquatting
4. Verified link URLs for lookalike domains and suspicious destinations
5. Checked SPF, DKIM, and DMARC authentication results
6. Identified phishing indicators and classified each email
7. Documented findings and created prevention guidelines

---

## 🚩 Key Phishing Indicators Found

- Fake / lookalike domains (paypa1.com, account-verify-secure.com)
- SPF / DKIM / DMARC authentication failures
- Urgency and fear-based language ("24 hours", "account will be locked")
- Generic greetings ("Dear User" instead of real name)
- Mismatched or suspicious URLs
- Brand impersonation (PayPal, DHL, IT Department)
- Reply-To address mismatch

---

## 📁 Repository Structure

```
FUTURE_CS_02/
├── README.md
├── FUTURE_CS_02_Phishing_Awareness_Report.html   ← full report (open in browser)
├── FUTURE_CS_02_Phishing_Awareness_Report.pdf    ← Canva export
└── evidence/
    ├── email_samples/
    │   ├── E-01_account_lock_phish.txt
    │   ├── E-02_paypal_phish.txt
    │   ├── E-03_it_password_reset_phish.txt
    │   ├── E-04_dhl_suspicious.txt
    │   └── E-05_github_safe.txt
    ├── header_analysis_E01_google_toolbox.png
    ├── header_analysis_E02_mxtoolbox.png
    └── virustotal_url_check.png
```

---

## 🛡️ Top Prevention Tips

1. Always check the sender's full email address (not just display name)
2. Hover over links before clicking to see the real destination
3. Enable MFA on all accounts — stops attackers even if they steal your password
4. When in doubt, call the sender directly using a number you already know
5. Report suspicious emails — don't just delete them

---

## 📚 References

- [Google Admin Toolbox — Header Analyser](https://toolbox.googleapps.com/apps/messageheader/)
- [MXToolbox Email Header Analyser](https://mxtoolbox.com/EmailHeaders.aspx)
- [VirusTotal](https://www.virustotal.com)
- [Phishing Email Examples (GitHub)](https://github.com/autinerd/phishing-mail-examples)
- [Phishing Dataset](https://github.com/rf-peixoto/phishing_pot)

---

*Submitted as part of the Future Interns Cyber Security Internship Programme.*  
*All samples are from public educational datasets. No real accounts or systems were accessed.*
