# Phishing Email Analysis Report

This repository contains an analysis of a public phishing email sample obtained from PhishTank. The goal is to identify phishing indicators, assess risks, and provide actionable insights for email security.

---

## Sample Overview

- **Source:** Public phishing sample from PhishTank  
- **Subject:** "Urgent: Account Suspension Notice"  
- **Sender:** `support@paypa1.com`

---

## Phishing Indicators

1. **Spoofed Sender Address**  
   - Email: `support@paypa1.com`  
   - Issue: Domain mimics PayPal but uses a fake “1” instead of “l”

2. **Header Discrepancies**  
   - SPF Check: Failed  
   - IP Origin: Unusual location (Russia)  
   - Tool Used: MxToolbox Email Header Analyzer

3. **Suspicious Links**  
   - Displayed URL: `https://paypal.com`  
   - Actual URL: `http://malicious-site.ru/paypal-login`  
   - Technique: Hover reveals mismatched URL

4. **Dangerous Attachment**  
   - File: `AccountUpdate.docm`  
   - Risk: Macro-enabled document could install malware

5. **Urgent Language**  
   - Example: "Your account will be suspended in 24 hours unless you verify your identity."

6. **Grammar Errors**  
   - Example: "We has detected unusual activity."  
   - Example: "Please verify you informations."

---

## Conclusion

This email contains multiple phishing traits including:  

- Spoofed sender  
- Mismatched URLs  
- Urgent tone  
- Malware-laced attachments  

**Action:** Flag and report immediately.

---

## Tools Used

- **MxToolbox Header Analyzer** – for analyzing email headers  
- **Hover-to-reveal URL inspection** – to detect URL mismatches  
- **Manual grammar and tone review** – to spot suspicious content

---

## Disclaimer

This report is for educational and awareness purposes only. Do **not** click links or open attachments in phishing emails.
