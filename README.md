## Lead Generation Automation using ChatGPT (Perplexity) + Google Sheets + Email

This project automates cold email outreach using Google Sheets, Perplexity AI (ChatGPT), and SMTP email sending — all built using **Make.com**.

## Overview

This automation helps you:

- Read new leads from a Google Sheet.
- Generate personalized cold emails using **Perplexity AI**.
- Send the emails automatically via Gmail/Outlook.
- Mark each lead as "sent" to avoid duplicates.

---

##  Tools & Services Used

- **Make.com** – No-code automation platform.
- **Google Sheets** – Lead storage and tracking.
- **Perplexity AI (LLaMA 3)** – Used for writing personalized emails.
- **SMTP (Gmail/Outlook)** – For sending emails.

---

## Workflow Breakdown

### 1. Step 1: Find Contact
- Reads rows from Google Sheet.
- Filters for rows where:
  - Email column is **not** “N/A”
  - Status column = **"not sent"**

### 2. Step 2: Write the Email (Perplexity AI)
- Takes the contact name, company name, and website.
- Sends a prompt to Perplexity AI to generate a cold email using this format:

### 3. Step 3: Send the Email
- Email is sent to the contact using SMTP (Gmail or Outlook).
- Subject: `FYI to {{Name}} - something for your business`

### 4. Step 4: Update the Sheet
- Once the email is sent, the status is updated from **“not sent”** to **“sent”** in the Google Sheet.


---

## How to Use

1. Import the `.json` workflow into your Make instance.
2. Connect:
   - Your **Google Sheets account**
   - Your **SMTP email account**
   - Your **Perplexity AI API key**
3. Update spreadsheet and field mappings as needed.
4. Run manually or schedule it daily for automated cold outreach.





