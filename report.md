# Phishing Email Analysis Report

## 1. Overview
**Date:** 2025-12-09
**Analyst:** Cyber Security Intern
**Subject:** Urgent: Your PayPal account is locked!
**Sender:** support@paypa1-security.com

This report outlines the analysis of a suspicious email claiming to be from PayPal. The email warns of account suspension to incite urgency and requests the user to click a verification link.

## 2. Header Analysis
The email headers indicate that the email did not originate from official PayPal infrastructure.

- **From Address:** `support@paypa1-security.com`
  - **Analysis:** The domain is typosquatted. It uses the number `1` instead of the letter `l` in "paypal". The official domain is `paypal.com`.
- **SPF (Sender Policy Framework):** `FAIL`
  - **Meaning:** The sending server IP is not authorized to send emails on behalf of this domain.
- **DKIM (DomainKeys Identified Mail):** `None`
  - **Meaning:** The email lacks a digital signature to verify its integrity.
- **DMARC:** `FAIL`
  - **Meaning:** The email failed authentication checks and should be treated as suspicious or rejected.
- **Received IP:** `192.0.2.45`
  - **Analysis:** The IP address does not belong to PayPal's authorized mail server range.

## 3. Link Analysis
**URL in Email:** `https://paypal.verify-login-security.com`

- **Domain:** `verify-login-security.com`
- **Subdomain:** `paypal`
- **Analysis:** The attacker uses a deceptive subdomain (`paypal`) to mislead the victim. The actual root domain is `verify-login-security.com`, which is not owned by PayPal.
- **URL Reputation:** This URL is flagged as malicious by multiple security vendors (see screenshots).

## 4. Social Engineering Indicators
The email employs several psychological triggers common in phishing attacks:

1.  **Urgency:** "Failure to act in the next 24 hours will result in permanent suspension." This creates panic.
2.  **Authority:** Claims to be from "PayPal Security Team".
3.  **Generic Greeting:** "Dear Customer" instead of the user's name, indicating a mass-sent campaign.
4.  **Suspicious Request:** Asking for immediate identity verification via an external link.

## 5. Risk Assessment
- **Severity:** High
- **Potential Impact:** Credential theft (username/password), financial loss, and potential identity theft if the user provides personal details on the landing page.

## 6. Conclusion
The email is a confirmed **Phishing Attempt**.
- It fails all authentication checks (SPF/DKIM/DMARC).
- It uses a typosquatted sender domain (`paypa1`).
- It directs users to a fraudulent website.

**Recommendation:**
- Do not click any links.
- Mark the email as spam/phishing.
- Block the sender domain.
