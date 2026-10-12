#  Tailk – Local AI Duel & Chat App

**Tailk** is a sleek, polished desktop application built with Electron that enables automated, dynamic, and infinite conversations between two local Large Language Models (LLMs) powered by [Ollama](https://ollama.com/).

Set custom system prompts, manage local models, set limits, and watch two AI agents debate, roleplay, or discuss any topic in real-time — completely offline and privacy-friendly.

---

## ✨ Features

- **🤖 Local AI vs. AI Conversations:** Connect two local LLMs and let them talk to each other automatically.
- **⚡ Real-time Streaming:** Watch answers generate live with real-time text streaming and thinking indicators.
- **📦 Integrated Model Installer:** Easily install new models directly within the app (`ollama pull`) with live progress reporting — no command line needed.
- **🔄 Auto Model Detection:** Automatically scans and lists all locally installed Ollama models in dynamic dropdown menus.
- **♾️ Infinite Chat Mode:** Enable infinite chat mode for never-ending conversations, or set a specific number of turns.
- **🎛️ Full Control & Customization:**
  - Adjustable System Prompts for both Model A and Model B.
  - Customizable initial start message / prompt.
  - Set response token limits (`max_tokens`).
  - Timeout protection per turn.
  - Global **Pause**, **Resume**, and **Cancel / Clear** controls.
- **💬 Modern UI:** Dark-themed responsive design with chat bubbles, copy-to-clipboard buttons, and status logs.
- **📦 All-in-One Installer:** Windows packaging (`.exe`) via `electron-builder` & NSIS, including silent auto-installation of Ollama if missing.

---

## 🛠️ Tech Stack

- **Framework:** [Electron](https://www.electronjs.org/) (Node.js)
- **AI Engine:** [Ollama JavaScript Library](https://github.com/ollama/ollama-js)
- **Packaging:** `electron-builder` + NSIS Scripting

---

## 🚀 Getting Started

### Prerequisites

Make sure you have [Node.js](https://nodejs.org/) installed on your machine.
For running models locally, [Ollama](https://ollama.com/) should be installed and running in the background.

### Installation & Development

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR-USERNAME/tailk-app.git](https://github.com/YOUR-USERNAME/tailk-app.git)
   cd tailk-app
