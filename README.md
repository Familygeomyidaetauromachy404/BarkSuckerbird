# 🤖 BarkSuckerBird 

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Telegram Bot](https://img.shields.io/badge/Telegram-Bot-blue?logo=telegram)](https://core.telegram.org/bots)
[![Flask](https://img.shields.io/badge/Flask-Server-black?logo=flask)](https://flask.palletsprojects.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Active-success)](#)
[![Deployed on](https://img.shields.io/badge/Hosted%20on-Koyeb-2F8D46?logo=koyeb&logoColor=white)](https://www.koyeb.com/)

---

## 🧠 Overview  

A powerful **Telegram AI bot** that integrates **multiple AI models**, live **web search via DuckDuckGo + Groq**, and an **admin texting system**.  
It’s designed for **24/7 uptime** using Flask’s keep-alive mechanism — perfect for deployment on **Replit**, **Render**, **Koyeb** or **Railway**.  


---

## 🚀 Features  

### 💬 Chat & Group AI Assistant  
- `/chat` — Activate the bot in a group.  
- `/stop` — Deactivate it.  
- `/ask <query>` — Ask anything directly from AI.  
- `/reset` — Clear your chat history.  
- `/help` — Show available commands.  

### 🌐 Web Search + Groq AI  
- `/web <query>` — Searches the web using **DuckDuckGo** and summarizes results using **Groq’s LLaMA 3-70B** model.  

### 🔐 Text Broadcast System  
For the bot **owner and authorized users** only:  
- `/txt <recipients> \`\`\`message\`\`\`` — Send a message to users/groups listed in `userss.json`.  
- `/auth <username>` — Authorize a user for `/txt`.  
- `/revoke <username>` — Remove authorization.

### 🧑‍💻 Owner-Only Commands  
- `/auth <username>` — Grant /txt permission.  
- `/revoke <username>` — Revoke /txt permission.  
- `/txt <users> \````message```` — Send message to one or more users.  

### 🧠 Contextual AI Chat  
- Maintains individual user histories for contextual replies.  
- Supports system prompts (`CONTEXT_AI`) for custom behavior.  
- Uses **OpenRouter (OpenAI-compatible)** free-tier models.  

---

## 🛠️ Tech Stack  

| Component | Description |
|------------|-------------|
| **Python** | Core language |
| **Flask** | Web server for keep-alive |
| **Telegram Bot API** | Interaction layer |
| **OpenRouter API** | AI completions |
| **Groq API** | Web answer generation |
| **DuckDuckGo Search (DDGS)** | Search provider |
| **Nest AsyncIO** | Async compatibility |

---

## ⚙️ Environment Variables  

| Variable | Purpose |
|-----------|----------|
| `BOT` | Telegram bot token |
| `API_KEY_BA` | OpenRouter API key |
| `MODEL` | Model name (e.g. `openai/gpt-3.5-turbo` or `mistralai/mixtral-8x7b`) |
| `CONTEXT_AI` | Base system message for AI |
| `GROQ` | Groq API key |


---

## 🧩 File Overview  
<pre>
├── main.py           # Main bot logic
├── userss.json       # Stores user & group chat IDs
├── requirements.txt  # Dependencies
└── README.md         # This file
</pre>

## 💙 Credits

Built with ❤️ by **Arush Baluni**
Refactored and enhanced by 🤖 **GPT-4o**
Powered by **Python**, **Groq**, **OpenRouter**, and **Telegram API**.

