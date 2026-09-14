# n8n-telegram-multitool-ai-agent

An advanced n8n AI agent workflow that connects Telegram to multiple productivity and research tools, allowing you to manage documents, calendar events, spreadsheets, emails, and web searches seamlessly through chat.

## ⚡ Quick Architecture

[ Telegram Trigger ] ──► [ AI Agent ] ──► [ Telegram Response ]
│
┌──────────────────┼──────────────────────────────────────┐
▼                  ▼        ▼             ▼        ▼      ▼
[ OpenAI Model ] [ Simple Memory ] [ Google Docs ] [ Calendar ] [ Sheets ] [ Gmail ] [ SerpApi ]

## ✨ Features

* **Multi-Tool Integration:** Execute tasks across Google Workspace and the web using natural language.
* **Conversational Memory:** Retains chat history and context across turns using Simple Memory.
* **Document & Data Management:** Update Google Docs, append rows in Google Sheets, and schedule Google Calendar events.
* **Communication & Search:** Send emails via Gmail and fetch live web data using SerpApi.

## 🛠️ Prerequisites & Setup

1. **n8n Instance:** Self-hosted or cloud-based n8n environment.
2. **Credentials Needed:**
   * **Telegram Bot Token** (from [@BotFather](https://t.me/BotFather))
   * **OpenAI API Key**
   * **Google OAuth2 Credentials** (for Docs, Calendar, Sheets, and Gmail)
   * **SerpApi API Key** (for Google Search)


## 🚀 Installation

1. Import the workflow JSON file into your n8n dashboard.
2. Link your **Telegram**, **OpenAI**, **Google Workspace**, and **SerpApi** credentials to their respective nodes.
3. Toggle the workflow to **Active**.
4. Start chatting with your Telegram bot to test out your multi-tool agent!
