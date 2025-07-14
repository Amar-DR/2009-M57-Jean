# 2009-M57-Jean

# 🕵️ Digital Forensics Case Study – M57 Jean Investigation

This repository contains a full digital forensic analysis of the **M57 Jean Case**, a classic case study often used in forensic education. The case involves the suspicious leak of a sensitive company spreadsheet (`m57biz.xls`) from the workstation of a user named Jean.

## 🎯 Objective
To determine whether Jean was responsible for intentionally leaking the document, or if the data breach was the result of a phishing attack.

## 🔍 Investigation Summary
- **Evidence Source:** Forensic disk image `nps-2008-jean.E01`
- **Tool Used:** Autopsy v4.x
- **Artifacts Analyzed:**
  - File system (location & metadata of `m57biz.xls`)
  - Email archive (`Outlook.pst`)
  - Deleted files
  - Timeline reconstruction

## 🧠 Key Findings
- The spreadsheet was created and accessed on **July 20, 2008 at 08:28**.
- An email was sent at the same timestamp to **tuckgorge@gmail.com**, a spoofed external address.
- The sender believed the email was from Alison, an internal staff member.
- No attempt to delete or conceal evidence was detected.
- Jean was determined to be a **victim of phishing**, not a malicious insider.

## 📁 Contents
- `/Report/` – Final PDF report and Word draft
- `/Screenshots/` – Key evidence screenshots from Autopsy
- `/Timeline/` – CSV export of event timeline
- `/Evidence Notes/` – Tags and annotations made during analysis

## ✅ Conclusion
Jean was **not responsible** for the data exfiltration. The leak was caused by a **sophisticated spoofing email** that exploited trust in internal communications. This case highlights the importance of user awareness and technical controls like SPF/DKIM/DMARC.

## 🛡️ Lessons Learned
- Train users to spot spoofed emails
- Apply domain-level email authentication
- Always verify recipient domains for sensitive file transfers

---

> This repository is for educational and academic purposes only. No real personal information is involved. All data belongs to the original M57 case study project.
