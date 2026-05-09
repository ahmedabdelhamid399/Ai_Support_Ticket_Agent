# 🤖 AI Support Ticket Agent

> An intelligent automation workflow that automatically summarizes support tickets using AI and sends professional email reports — built with n8n, Groq (Llama 3), Airtable, and Gmail.

---

## 🎯 Project Overview

This project automates the entire support ticket lifecycle:

1. **Detects** new support tickets in Airtable automatically
2. **Validates** ticket data before processing
3. **Summarizes** tickets using Groq AI (Llama 3.3-70b)
4. **Generates** professional HTML email reports
5. **Sends** automated emails to the support manager
6. **Logs** all results back to Airtable with full audit trail

---

## ⚙️ Tech Stack

| Technology | Purpose |
|---|---|
| **n8n** | Workflow automation engine |
| **Groq (Llama 3.3-70b)** | AI ticket summarization |
| **Airtable** | Ticket database and logging |
| **Gmail** | Email delivery |

---

## ✨ Features

- ✅ Fully automated — zero manual intervention
- ✅ Processes multiple tickets per cycle
- ✅ Prevents duplicate processing with lock mechanism
- ✅ AI-generated priority detection
- ✅ Professional HTML email template
- ✅ Complete audit trail in Airtable
- ✅ Error handling and logging
- ✅ Free AI with Groq — no OpenAI costs

---

## 🚀 Setup Guide

### Prerequisites
- n8n installed (local or cloud)
- Airtable account (free)
- Groq account (free)
- Gmail account

### Step 1 — Airtable Setup
1. Create base called `Support Ticket Agent`
2. Create table called `Tickets`
3. Add all fields from [schema.md](airtable/schema.md)
4. Generate API token with read/write access

### Step 2 — Groq Setup
1. Create account at console.groq.com
2. Generate API key
3. Model: `llama-3.3-70b-versatile`

### Step 3 — n8n Setup
1. Import `workflow/AI_Support_Ticket_Agent.json`
2. Add credentials:
   - Airtable API token
   - Groq API key
   - Gmail OAuth
3. Activate the workflow

---

## 📁 Project Structure
Ai_Support_Ticket_Agent/
│
├── README.md
├── .env.example
├── workflow/
│   └── AI_Support_Ticket_Agent.json
├── assets/
│   ├── workflow-overview.png
│   ├── execution-success.png
│   ├── airtable-results.png
│   └── email-output.png
└── airtable/
└── schema.md

---

## 🧠 What I Learned

- Building production-grade n8n workflows
- Integrating free AI APIs (Groq/Llama 3)
- Professional error handling in automation
- Airtable as a backend database
- HTML email template design
- Preventing duplicate processing in loops

---

## 👨‍💻 Author

**Ahmed Abdelhamid**
Automation Engineer | n8n | APIs | AI Integration

---

## 📄 License

MIT License
