# 🛡️ Task 2: Phishing Email Analysis

<div align="center">

![Security](https://img.shields.io/badge/Security-Phishing%20Analysis-red?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)
![Day](https://img.shields.io/badge/Internship-Day%202-blue?style=for-the-badge)

**Cyber Security Internship | ElevateLabs**

</div>

---

## 📖 About This Project

This project demonstrates a complete **phishing email analysis** workflow. It covers:

- 📧 Analyzing suspicious email content
- 🔍 Investigating email headers for authentication failures
- 🔗 Examining malicious URLs
- 🧠 Identifying social engineering tactics
- 📝 Documenting findings in a professional report

---

## 📁 Project Structure

```
📂 Task-2-Phishing-Email-Analysis/
│
├── 📄 phishing_email_sample.txt   # Raw phishing email content
├── 📄 email_headers.txt           # Email authentication headers
├── 📄 report.md                   # Detailed analysis report
├── 📄 README.md                   # Project documentation
│
└── 📂 screenshots/
    ├── 🖼️ headers_screenshot.png  # MXToolbox header analysis
    └── 🖼️ link_screenshot.png     # VirusTotal URL scan
```

---

## 🚀 Quick Start

### Step 1: Review the Threat
Open [`phishing_email_sample.txt`](phishing_email_sample.txt) to see the original suspicious email.

### Step 2: Check the Headers
Review [`email_headers.txt`](email_headers.txt) for technical evidence of spoofing.

### Step 3: Read the Full Report
Open [`report.md`](report.md) for a comprehensive breakdown including:

| Section | Content |
|---------|---------|
| 📋 Executive Summary | Quick verdict and key findings |
| 📨 Header Analysis | SPF/DKIM/DMARC failures explained |
| 🔗 Link Analysis | Malicious URL breakdown |
| 🧠 Social Engineering | Psychological tactics identified |
| ⚡ Risk Assessment | Severity and impact analysis |
| ✅ Recommendations | Actionable security steps |

---

## 🔍 Key Findings

| Indicator | Status | Description |
|-----------|--------|-------------|
| 📧 **Sender Domain** | 🔴 Fake | `paypa1` instead of `paypal` |
| 🔐 **SPF Check** | 🔴 FAIL | Unauthorized sender IP |
| ✍️ **DKIM Signature** | 🔴 None | No email signature |
| 🛡️ **DMARC Policy** | 🔴 FAIL | Authentication failed |
| 🔗 **URL Reputation** | 🔴 Malicious | Flagged by 6+ vendors |

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| 🔧 **MXToolbox** | Email header analysis |
| 🔧 **VirusTotal** | URL reputation scanning |
| 📝 **Markdown** | Report documentation |

---

## 📸 Screenshots

<details>
<summary>📊 Click to view Header Analysis</summary>

![Header Analysis](screenshots/headers_screenshot.png)

</details>

<details>
<summary>🔗 Click to view URL Scan</summary>

![URL Scan](screenshots/link_screenshot.png)

</details>

---

## 👨‍💻 Author

**Cyber Security Intern**  
📅 December 2025  
🏢 ElevateLabs Internship Program

---

<div align="center">

⭐ **If this helped you, give the repo a star!** ⭐

</div>
