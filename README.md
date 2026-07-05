<div align="center">

# 🦇 Alfred AI

### Your Personal AI-Powered Voice Assistant

*"At your service, always listening."*

![Python](https://img.shields.io/badge/Python-100%25-3776AB?style=for-the-badge&logo=python&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-API-412991?style=for-the-badge&logo=openai&logoColor=white)
![Speech Recognition](https://img.shields.io/badge/Speech-Recognition-4CAF50?style=for-the-badge&logo=googleassistant&logoColor=white)
![Platform](https://img.shields.io/badge/platform-Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Hackathon](https://img.shields.io/badge/built%20for-Grid%205.0-ff69b4?style=for-the-badge)

</div>

---

## 🎙️ What is Alfred?

**Alfred AI** is a voice-controlled personal assistant that listens, understands, and talks back — powered by speech recognition and the OpenAI API. Speak naturally, and Alfred will browse the web, launch apps, tell you the time, or just have a conversation with you, Jarvis-style.

> Built for **Grid 5.0**, forked and extended from [Lucifer1811/alfred-AI](https://github.com/Lucifer1811/alfred-AI).

---

## ⚡ Key Features

| Feature | What it does |
|---------|--------------|
| 🗣️ **Voice Interaction** | Understands spoken commands using the `speech_recognition` library |
| 🤖 **AI Conversations** | Powered by the OpenAI API for natural, intuitive chatbot responses |
| 🌐 **Web Browsing** | Opens YouTube, Wikipedia, Netflix, and more on command |
| 🚀 **App Launching** | Launches apps like Discord, WhatsApp, and others via voice |
| 🕐 **Time Reporting** | Tells you the current time on request |
| 🎩 **Personalized Wake Trigger** | Say *"Sir Alfred AI"* to activate the AI chatbot mode |
| ♻️ **Conversation Reset** | Say *"reset chat"* to clear ongoing conversation context |

---

## 🧠 How It Works

```
🎤 Voice Input
      │
      ▼
┌───────────────────────┐
│  speech_recognition     │  ──▶ Converts speech to text
└───────────┬────────────┘
            ▼
┌───────────────────────┐
│  Command Parser          │  ──▶ Detects intent: web / app / time / chat
└───────────┬────────────┘
            ▼
   ┌────────┴─────────┬───────────────┬───────────────┐
   ▼                  ▼               ▼               ▼
🌐 Open Website   🚀 Launch App   🕐 Report Time   🤖 OpenAI Chat
   │                  │               │               │
   └──────────────────┴───────────────┴───────────────┘
                       ▼
              🔊 Spoken / Text Response
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | Python |
| Speech-to-Text | `speech_recognition` |
| AI Engine | OpenAI API |
| App Control (Windows) | `win32com.client` |
| Config | `key_oAI.py` (API key module) |

---

## 🚀 Getting Started

### 1️⃣ Clone the repository

```bash
git clone https://github.com/SohinijRover/alfred-AI_Grid5.0.git
cd alfred-AI_Grid5.0
```

### 2️⃣ Install dependencies

```bash
pip install pywin32 SpeechRecognition openai
```

### 3️⃣ Add your OpenAI API key

Open `key_oAI.py` and replace the placeholder with your own key:

```python
api_key = "YOUR_OPENAI_API_KEY_HERE"
```

> 🔒 **Never commit your real API key.** Keep `key_oAI.py` out of version control if it contains secrets.

### 4️⃣ Run Alfred

```bash
python main.py
```

Alfred will greet you and start listening — just speak naturally!

---

## 💬 Example Commands

| Say this... | Alfred does this |
|-------------|-------------------|
| *"Open YouTube"* | Launches YouTube in your browser |
| *"Open WhatsApp"* | Starts the WhatsApp desktop app |
| *"What's the time?"* | Reads out the current time |
| *"Sir Alfred AI, tell me a fun fact"* | Triggers the AI chatbot for a conversational response |
| *"Reset chat"* | Clears the current conversation context |

---

## ⚠️ Notes & Caution

- Requires proper setup, including a valid OpenAI API key.
- Voice assistants process spoken input — be mindful about sharing sensitive information out loud.
- Currently built with Windows-specific app-launching (`win32com.client`); cross-platform support is a future goal.

---

## 🔭 Future Enhancements

- [ ] Smarter, more context-aware conversations
- [ ] Integration with more web services & third-party apps
- [ ] Cross-platform application launching (macOS/Linux)
- [ ] Improved error handling & user prompts for smoother interactions

---

## 🤝 Contributing

Contributions, feedback, and feature ideas are welcome! Feel free to fork the repo, open a pull request, or raise an issue to help make Alfred smarter.

---

<div align="center">

*"I am not just code — I am at your service."* 🦇

</div>
