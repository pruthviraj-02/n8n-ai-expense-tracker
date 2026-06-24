# 🤖 AI Expense Tracker Bot

An AI-powered personal finance assistant built with n8n, Groq, Telegram, and Google Sheets.

Track expenses through natural conversation, receive financial insights, monitor budgets, and generate spending reports — all from Telegram.

## ✨ Features

* 💬 Natural language expense tracking
* 📊 Automated spending summaries
* 🧠 AI-generated financial insights
* 🎯 Budget monitoring and tracking
* 🗂 Automatic expense categorization
* 📝 Real-time storage in Google Sheets
* 🧠 Conversation memory for contextual responses
* ⚡ Fully automated workflow powered by AI agents

---

## Example Usage

### Log an Expense

```text
User: spent 250 on lunch

Bot:
✅ Expense Logged Successfully

📅 Date: 17-Jun-2026
💰 Amount: ₹250
📂 Category: Food
📝 Description: lunch
```

### Get a Summary

```text
User: summary

Bot:
📊 Financial Report

💸 Total Spent: ₹2,840

🔥 Top Categories:
1. Food - 45%
2. Transport - 20%
3. Education - 15%
```

### Set a Budget

```text
User: set budget 10000

Bot:
🎯 Budget Set: ₹10,000/month

Daily Limit: ₹333
Weekly Limit: ₹2,500
```

---

## 🏗 Architecture

```text
Telegram
    │
    ▼
AI Agent (Groq Llama 3.3)
    │
 ┌──┴──────────┐
 ▼             ▼
Save Expense   Read History
(Google Sheet) (Google Sheet)
 └──────┬──────┘
        ▼
 Telegram Reply
```

---

## 🛠 Tech Stack

| Component  | Technology           |
| ---------- | -------------------- |
| Automation | n8n                  |
| AI Model   | Groq (Llama 3.3 70B) |
| Messaging  | Telegram Bot API     |
| Storage    | Google Sheets        |
| Memory     | n8n Buffer Memory    |
| Hosting    | Railway              |

---

## 🚀 Setup

1. Import `workflow.json` into n8n
2. Create a Telegram bot using BotFather
3. Generate a Groq API key
4. Create a Google Sheet with the following columns:

```text
Date | Amount | Category | Description
```

5. Configure Google Sheets credentials
6. Replace placeholder values inside the workflow
7. Activate the workflow

---

## 📚 What I Learned

* AI Agent design and tool calling
* Prompt engineering for structured outputs
* Workflow automation using n8n
* Google Sheets integration
* API authentication and management
* Stateful conversations using memory
* Building reliable AI-powered automations

---

## 🔒 Security

This repository does not contain:

* API keys
* Telegram credentials
* Google OAuth credentials
* Personal spreadsheet IDs

All sensitive information has been removed before publishing.

---

## 🎯 Future Improvements

* Multi-user support
* Monthly PDF reports
* Spending trend visualizations
* Expense approval workflows
* Database integration (PostgreSQL)
* Web dashboard

---

## 👨‍💻 Author

**Pruthviraj Chaudhari**

Computer Engineering Student | Cloud & AI Enthusiast

If you found this project useful, feel free to ⭐ the repository.

---

Built with ❤️ using n8n, Groq, Telegram, and Google Sheets.
