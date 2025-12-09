# Task 2: Phishing Email Analysis

## Project Overview
This project is part of the Day 2 Cyber Security Internship. It involves the analysis of a simulated phishing email to identify indicators of compromise (IOCs) such as header anomalies, malicious links, and social engineering tactics.

## Project Structure
```
Task-2-Phishing-Email-Analysis/
├── phishing_email_sample.txt  # The raw text of the suspicious email
├── email_headers.txt          # Extracted headers showing authentication failures
├── report.md                  # Detailed analysis report
├── README.md                  # Project documentation
└── screenshots/               # Evidence screenshots
      ├── headers_screenshot.png
      └── link_screenshot.png
```

## How to Read the Report
1.  **Start with `phishing_email_sample.txt`** to see the initial threat layout.
2.  **Review `email_headers.txt`** to understand the technical evidence behind the spoofing detection.
3.  **Open `report.md`** for a comprehensive breakdown of findings, including:
    - Sender domain analysis (`paypa1` vs `paypal`)
    - Explanation of SPF/DKIM failures
    - Assessment of the malicious URL structure

## Author
Cyber Security Intern
