# PHISHING EMAIL ANALYSIS — SIMULATED SAMPLE

## Sample Name
Fake PayPal Account Alert (simulated)

## Date Analyzed
2025-10-21

## Analyst
Sagar Saini

---

## 📁 Evidence Included
- `email-original.txt` — raw headers
- `header-analysis.txt` — MXToolbox results
- `links.txt` — suspicious hrefs
- `attachments.txt` — phishing attachment
- `domain-checks.txt` — domain mismatch notes
- `screenshots/` — email and link hover images
- `reports.txt` — summary report

---

## 🧠 Summary
This simulated email displays multiple phishing indicators: misspelled sender domain, SPF/DKIM/DMARC failures, mismatched visible link vs actual href, urgent threat language, and an HTML attachment — classify as phishing.

---

## 🔍 Observations

| Indicator         | Evidence / File                | Why Suspicious |
|------------------|--------------------------------|----------------|
| From Address      | support@paypall.com            | Misspelled domain |
| Return-Path       | bounce@mailer-example.net      | Bounce domain mismatch |
| SPF               | header-analysis.txt — FAIL     | Unauthorized sender IP |
| DKIM              | header-analysis.txt — none     | No signature |
| DMARC             | header-analysis.txt — FAIL     | Policy not satisfied |
| Link href         | links.txt — mismatched URL     | Redirects to fake domain |
| Attachment        | attachments.txt — HTML file    | Likely phishing form |
| Language/Tone     | screenshots/ — urgent threat   | Social engineering |

---

## ✅ Conclusion
This email contains clear technical and behavioral signs of phishing. It should be flagged, reported, and deleted.

---

## 🔒 Recommended Actions
- Mark as phishing and delete
- Do not click links or open attachments
- If credentials were entered, change password and enable 2FA
- Report to PayPal’s phishing address

---

## 📦 Files Included
- `email-original.txt`
- `header-analysis.txt`
- `links.txt`
- `attachments.txt`
- `domain-checks.txt`
- `screenshots/`
- `reports.txt`
