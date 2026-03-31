![image alt](https://github.com/nikhil-ai-insights/daily-hr-referral-cold-email-system-v2/blob/7d9c74e7459ca3d2eecf1566d2a27016e89227a2/asset.png)
# 🤖 Daily HR Referral Cold Email System v2 🚀

## Overview

**Daily HR Referral Cold Email System v2** is an advanced AI-powered automation workflow built with **n8n** that automates personalized cold email outreach to HR professionals.

This system combines **automation + AI (LLM)** to generate unique, human-like emails for each recipient — significantly improving engagement and response rates compared to traditional bulk emailing.

---

## 🌟 Key Highlights

- 🤖 AI-generated personalized emails (LLM-based)
- 📊 Google Sheets as dynamic database
- 🎯 Smart filtering of relevant HR contacts
- ⚡ Controlled email sending (anti-spam safe)
- ⏳ Human-like delays between emails
- ✅ Automatic tracking of sent emails
- 🔁 Zero duplicate outreach

---

## 🔄 Workflow Architecture

```
Schedule Trigger → Get Data → Filter → Limit → AI Agent → Send Email → Wait → Update Sheet
```

---

## 🧠 How It Works (Step-by-Step)

### ⏰ 1. Schedule Trigger
Automatically runs the workflow daily at a predefined time.

### 📊 2. Fetch Data (Google Sheets)
Retrieves HR contact details:
- Name
- Email
- Company
- Status

### 🔍 3. Filter Contacts (IF Node)
Selects only:
- Contacts not yet emailed
- Valid entries
- Targeted recipients

### ⚡ 4. Limit Node
- Controls number of emails sent per run
- Helps avoid Gmail spam detection

### 🤖 5. AI Agent (Core Engine)
Uses an LLM (e.g., OpenAI) to:
- Generate personalized email content
- Customize message for each contact

> 👉 Every email is **unique and human-like**

### 📨 6. Send Email (Gmail Node)
Sends AI-generated email to each recipient.

### ⏳ 7. Wait Node
- Adds delay between emails
- Simulates natural sending behavior

### ✅ 8. Update Google Sheet
- Marks contact as **Emailed**
- Prevents duplicate outreach

---

## 🏗️ Tech Stack

| Component | Tool |
|---|---|
| Automation Platform | n8n |
| AI Model | OpenAI (LLM) |
| Email Service | Gmail API |
| Database | Google Sheets |
| Logic Control | IF, Limit, Wait Nodes |

---

## 📁 Google Sheet Format

| Name | Email | Company | Status | Last Contacted |
|---|---|---|---|---|
| John Doe | john@email.com | ABC Corp | Pending | - |

---

## ✉️ AI Email Example

```
Subject: Opportunity at {{Company}}

Hi {{Name}},

I came across your work at {{Company}} and wanted to reach out regarding
potential opportunities.

I'd love to connect and explore how I can contribute to your team.

Looking forward to your response.

Best regards,
[Your Name]
```

---

## ⚙️ Setup Instructions

### 1️⃣ Import Workflow
Import the `.json` file into n8n.

### 2️⃣ Configure Google Sheets
- Add credentials
- Connect your sheet

### 3️⃣ Setup Gmail
- Enable Gmail API
- Connect via OAuth2

### 4️⃣ Setup AI Model
- Add OpenAI API key
- Connect to AI Agent node

### 5️⃣ Configure Schedule
Set workflow timing (daily recommended).

---

## 🛡️ Anti-Spam & Safety Measures

- ✅ Email rate limiting
- ✅ Delay between emails
- ✅ AI personalization (no bulk copy-paste)
- ✅ Duplicate prevention system

---

## 📊 Use Cases

- 💼 Job seekers (HR outreach & referrals)
- 🤝 Professional networking
- 📈 Lead generation
- 🚀 AI automation portfolio projects

---

## 🔮 Future Improvements

- 📊 Email analytics dashboard
- 🔁 Automated follow-up sequences
- 📎 Resume auto-attachment
- 🌐 Multi-language email generation
- 🧠 Smarter AI personalization

---

## ⚠️ Disclaimer

This project is intended for **ethical and professional use only**.
Do not use for spam or unsolicited mass outreach. Always follow email regulations and best practices.

---

## 🤝 Contributing

Contributions are welcome! Check the [`CONTRIBUTING.md`](CONTRIBUTING.md) file for guidelines.

---

## 🔐 Security

For reporting vulnerabilities, refer to [`SECURITY.md`](SECURITY.md).

---

## 🙌 Author

**Nikhil** 🚀 Building AI-powered automation systems

🔗 [github.com/nikhil-ai-insights](https://github.com/nikhil-ai-insights)

---

## ⭐ Support

If you like this project:
- ⭐ Star the repo
- 🍴 Fork it
- 🤝 Contribute

---

## 🚀 Why This Project Matters

This project showcases how AI-powered automation can turn repetitive outreach into a scalable, personalized system — improving efficiency, and impact.
