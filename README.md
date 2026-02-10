# 🌌 VOID — Anti-Gravity similar AI Agent with IDE

> *Intelligence floating beyond conventional limits.*

![VOID Banner](https://img.shields.io/badge/VOID-Anti--Gravity%20AI-00c8ff?style=for-the-badge&logo=anthropic&logoColor=white)
![Claude](https://img.shields.io/badge/Powered%20by-Claude%20Sonnet%204.5-7b3fff?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-00ff9d?style=for-the-badge)
![HTML](https://img.shields.io/badge/Built%20with-HTML%2FJS%2FCSS-ffaa00?style=for-the-badge)

---

## ✦ Overview

**VOID** is a sleek, futuristic single-file AI agent chat interface built with pure HTML, CSS, and JavaScript. It features a fully customizable AI persona, multi-model selection, a live memory core, and a stunning deep-space aesthetic — all powered by the [Anthropic Claude API](https://docs.anthropic.com).

---

## 🚀 Features

- **⚡ Multi-Model Selection** — Switch between Claude Sonnet 4.5, Qwen 3, and Gemini Pro personas
- **🧠 Memory Core** — Live right-panel that extracts and displays conversation context nodes (fact, preference, goal, context)
- **🎨 Persona Customization** — Change the agent's name, emoji avatar, and role in real time
- **💬 Rich Chat UI** — Animated messages, typing indicators, code block formatting, and auto-resizing input
- **⭐ Quick Actions & Chips** — One-click prompt starters for common tasks (debug, summarize, ideate, plan)
- **🌌 Deep-Space Aesthetic** — Animated starfield, floating orbs, glassmorphism panels, and glowing Orbitron typography
- **📊 Session Stats** — Tracks message count, memory nodes, and context window usage
- **📱 Single-File App** — Everything in one `.html` file, zero dependencies, no build step

---

## 🖥️ Demo Preview

```
┌─────────────────────────────────────────────────────────┐
│  VOID  [Agent] [Modules] [Deploy] [Logs]    ● ONLINE    │
├──────────────┬──────────────────────┬───────────────────┤
│  PERSONA     │                      │  🧠 MEMORY CORE   │
│  ┌────────┐  │   ✦ Chat Messages    │  ┌─────────────┐  │
│  │  🤖   │  │                      │  │ [goal] ...  │  │
│  │  VOID  │  │                      │  │ [fact] ...  │  │
│  └────────┘  │                      │  │ [pref] ...  │  │
│              │                      │  └─────────────┘  │
│  Quick       ├──────────────────────┤  Context: 12%     │
│  Actions     │  [Input Bar]  [Send] │  Nodes: 3         │
└──────────────┴──────────────────────┴───────────────────┘
```

---

## 🛠️ Setup & Usage

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/void-ai-agent.git
cd void-ai-agent
```

### 2. Add Your Anthropic API Key

Open `index.html` and locate the fetch call inside `sendMessage()`:

```javascript
const response = await fetch('https://api.anthropic.com/v1/messages', {
  method: 'POST',
  headers: {
    'Content-Type': 'application/json',
    'x-api-key': 'YOUR_API_KEY_HERE',        // ← Add your key
    'anthropic-version': '2023-06-01'
  },
  ...
});
```

> ⚠️ **Security Note:** Never commit your API key to a public repository. For production use, proxy requests through a backend server.

### 3. Open in Browser

```bash
open index.html
# or simply double-click the file
```

No server required — runs entirely in the browser.

---

## 🎛️ Customization

| Feature | How To |
|---|---|
| Agent Name | Type in the name field in the left sidebar |
| Agent Emoji | Click the avatar to open the emoji picker |
| Agent Role | Edit the role field below the avatar |
| Active Model | Use the dropdown in the top bar |
| Quick Actions | Edit the `.qa-btn` buttons in the HTML |
| Prompt Chips | Edit the `.chip` spans in the HTML |

---

## 🤖 AI Models

| Model | Persona Style | Backend |
|---|---|---|
| ⚡ Claude Sonnet 4.5 | Futuristic & confident | Anthropic API |
| 🔮 Qwen 3 | Precise & analytical | Anthropic API (persona-simulated) |
| ✦ Gemini Pro | Creative & multimodal | Anthropic API (persona-simulated) |

> **Note:** Qwen 3 and Gemini Pro selections simulate those models' personalities via system prompts. To use the actual model endpoints, you would need their respective API keys and a backend proxy.

---

## 📁 Project Structure

```
void-ai-agent/
│
├── index.html        # Complete single-file application
└── README.md         # This file
```

---

## 🔧 Tech Stack

- **Frontend:** Vanilla HTML5, CSS3, JavaScript (ES2020+)
- **Fonts:** [Orbitron](https://fonts.google.com/specimen/Orbitron) & [Space Mono](https://fonts.google.com/specimen/Space+Mono) via Google Fonts
- **AI:** [Anthropic Messages API](https://docs.anthropic.com/en/api/messages)
- **Design:** Glassmorphism, CSS animations, CSS Grid layout

---

## 📄 License

MIT License — feel free to fork, remix, and launch into the void.

---

## 🌌 Acknowledgements

Built with the [Anthropic Claude API](https://anthropic.com). Inspired by the endless expanse of deep space and the idea that intelligence should know no gravity.

---

<p align="center">
  <em>Transmit your queries into the void.</em><br>
  <strong>◎ VOID — Anti-Gravity Intelligence ◎</strong>
</p>
