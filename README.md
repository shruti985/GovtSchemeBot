
# 🏛️ Govt Health Schemes Bot (n8n + Telegram)

This repository contains an **n8n workflow JSON** that powers a conversational Telegram bot.  
The bot helps users discover **Indian Government Health & Welfare Schemes** based on their basic eligibility inputs.

Users provide:
- Age
- Gender
- Caste Category
- State

The workflow then filters schemes stored in Google Sheets and returns relevant matches.

---

## 🚀 What this bot does

✔️ Collects user info step-by-step through Telegram  
✔️ Validates user inputs (age, strings, etc.)  
✔️ Uses inline buttons for Gender & Caste  
✔️ Fetches data from Google Sheets  
✔️ Scores schemes based on eligibility match  
✔️ Shows results with pagination (Show more)  
✔️ Supports restart via `/start`

---

## 🧩 Workflow Contents

This JSON includes:
- Telegram Trigger
- State-based user flow
- JavaScript scoring logic
- Google Sheets read integration
- Pagination logic
- Clean restart logic

**Note:**  
This repo does **not** include any credentials.  
When you import in n8n, you’ll add your own credentials manually.

---

## 🛠️ Requirements

To use this workflow, you need:

### 🟢 n8n
- Hosted or local  
- Version 1.x or above recommended

### 🟢 Telegram Bot
- Create via **@BotFather**
- Copy token and configure inside n8n credentials

### 🟢 Google Sheet
Your sheet should contain columns for:
