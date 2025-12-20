# 🏛️ Govt Health Schemes Bot (Telegram + n8n)

A conversational Telegram bot made using **n8n** that helps users discover **Indian Government Health & Welfare Schemes**.  
Users answer a few simple questions (Age, Gender, Caste, State), and the bot filters matching schemes from **Google Sheets** and shows results with **scoring + pagination**.

---

## 🚀 Features

- Collects Age with validation  
- Gender selection using inline buttons  
- Caste selection via inline buttons  
- State input  
- Reads data dynamically from Google Sheets  
- Scores schemes based on eligibility match  
- Shows paginated results with "Show More"  
- Restart anytime using `/start`  
- No credentials included in repo

---

## 🧩 What’s Inside

This repo contains **one JSON workflow** that includes:

- Telegram Trigger
- User state management
- Google Sheets read operation
- JavaScript scoring & filtering
- Messenger replies with markup
- Pagination logic

When you import in n8n, you will need to **add your own credentials** for Telegram and Google Sheets.

---

## 🛠 Requirements

### **n8n**
- Local or hosted  
- Version 1.x recommended

### **Telegram Bot**
- Create using **@BotFather**  
- Add token to n8n Telegram credentials

### **Google Sheet**
- The workflow already points to a Google Sheet that contains all scheme data  
- Users do **not** need to create an Excel or a new Google Sheet again  
- They only need to connect their own Google Sheets credentials in n8n  
- Once credentials are added, the workflow will read from the same sheet automatically

---

## 📥 How to Use

1. Download JSON workflow from this repo  
2. Open n8n → **Workflows → Import**  
3. Select the JSON file  
4. Assign your Telegram + Google Sheets credentials  
5. Activate the workflow  
6. Open Telegram and send `/start` to begin

---

## 🔒 Security Notes

- No tokens or secrets are included in this repo  
- Credentials must be configured locally in n8n  
- Never publish Telegram or Google credentials publicly

---

## 🧪 Ideas for Improvement

- Income-based filtering  
- Hindi / multilingual responses  
- More categories (e.g., Widow, Disability, Farmer)  
- Scheme bookmarking / sharing  
- Database storage for chat data

---

## 🤝 Contributions Welcome

- Fork it  
- Open issues  
- Submit pull requests  

Suggestions are appreciated!

---

## 📜 License

Free for learning, modification, and personal use.
