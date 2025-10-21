# phishing-email-analysis
> This project was created as part of my cybersecurity internship to demonstrate the process of detecting and reporting phishing emails.
# 🛡️ Phishing Email Analysis Report

**Intern Name:** Dorapally Karthik  
**Internship Title:** Cybersecurity Internship  
**Objective:** Identify phishing characteristics in a suspicious email sample.  

---

#  Objective
To identify common phishing indicators from a suspicious email sample using open-source tools and manual analysis.

---

# Tools Used
- Email client (Gmail) or saved email file (.eml/.txt)  
- [MxToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)
- https://lookup.icann.org/en
- https://www.redirect-checker.org/
- Web browser (for checking URLs and verifying domains)

---

# Sample Phishing Email
**Subject:** `URGENT: Your Account Has Been Suspended – Verify Now!`  
**Claimed Sender:** `PayPal Support (support@paypaI.com)`

**Description:**  
The email claimed the recipient’s PayPal account would be suspended unless they verified their account within 24 hours.

---

## 🕵️‍♂️ Analysis Steps

## 1. Sender Email Address
- **Displayed:** `support@paypaI.com`  
- **Actual Domain:** `paypaI.com` (uses uppercase “I” instead of lowercase “l”)  
✅ **Indicator:** Spoofed email domain.

---

## 2. Email Header Analysis
- **SPF/DKIM checks:** Failed  
- **Return-Path:** `info@secure-update-check.com`  
- **Origin IP:** Unrelated to PayPal mail servers  
✅ **Indicator:** Header inconsistencies show the message wasn’t from PayPal.

---

## 3. Suspicious Links or Attachments
- “Verify Account” button linked to  
  `http://paypal-verification-securelogin.com`  
- Attached file: `Account_Verification_Form.zip`  
✅ **Indicator:** Malicious link and attachment detected.

---

### 4. Urgent or Threatening Language
> “Your account will be permanently suspended within 24 hours if you don’t verify now!”

✅ **Indicator:** Urgency and fear tactics to force user action.

---

## 5. Mismatched URLs
- Visible link: `www.paypal.com`  
- Hover link: `paypal-verification-securelogin.com`  
✅ **Indicator:** Mismatched URL redirection.

---

## 6. Spelling and Grammar Errors
> “We regreat to infrom you about your acccount suspenion.”  
✅ **Indicator:** Poor grammar and spelling errors.

---

# Summary of Phishing Indicators

| Indicator | Description |
|------------|-------------|
| Spoofed Sender | Fake “PayPal” address using similar characters |
| Header Failures | SPF/DKIM mismatch, fake return path |
| Fake Link | Directs to non-official domain |
| Urgent Tone | Threat of suspension |
| Suspicious Attachment | ZIP file with fake verification form |
| Grammar Errors | Multiple typos |
| Mismatched URLs | Link text and destination differ |

---

# Conclusion
The analyzed email clearly demonstrates multiple **phishing traits** including spoofed domains, header mismatches, urgency-based language, and fake URLs.  
**Recommendation:** Do not click any links or download attachments. Report the email as **phishing**.![Uploading Screenshot 2025-10-21 181912.png…]()
<img width="1920" height="1080" alt="Screenshot 2025-10-21 183311" src="https://github.com/user-attachments/assets/e5f3ed37-0762-49c9-8349-75b92d6360a4" />
<img width="1920" height="1080" alt="Screenshot 2025-10-21 183328" src="https://github.com/user-attachments/assets/451dc15d-f94b-42a4-8b2a-8c1dc21e592c" />
<img width="1920" height="1080" alt="Screenshot 2025-10-21 183341" src="https://github.com/user-attachments/assets/76e489f2-0936-49c4-8344-2c7d510865aa" />
<img width="1920" height="1080" alt="Screenshot 2025-10-21 183353" src="https://github.com/user-attachments/assets/6581bfd0-485f-4421-9c1a-861f090d3042" />
<img width="1920" height="1080" alt="Screenshot 2025-10-21 183406" src="https://github.com/user-attachments/assets/305c6742-c279-48b3-ac1c-92d4420c096c" />
<img width="1920" height="1080" alt="Screenshot 2025-10-21 183428" src="https://github.com/user-attachments/assets/da5aba2c-3eb7-48fc-af0e-b4ab0903fffd" />
[phishing-email-analysis.zip](https://github.com/user-attachments/files/23021597/phishing-email-analysis.zip)
