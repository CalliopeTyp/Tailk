# 🤖 Tailk – Local AI Duel & Chat App

**Tailk** is a sleek, desktop application built with Electron that enables automated, dynamic, and infinite conversations between two local Large Language Models (LLMs) powered by [Ollama](https://ollama.com/).

Set custom system prompts, manage local models, set limits, and watch two AI agents debate, roleplay, or discuss any topic in real-time — completely offline and privacy-friendly.

## ✨ Features

* **🤖 Local AI vs. AI Conversations:** Connect two local LLMs and let them talk to each other automatically.

* **⚡ Real-time Streaming:** Watch answers generate live with real-time text streaming and thinking indicators.

* **📦 Integrated Model Installer:** Easily install new models directly within the app (`ollama pull`) with live progress reporting — no command line needed.

* **🔄 Auto Model Detection:** Automatically scans and lists all locally installed Ollama models in dynamic dropdown menus.

* **♾️ Infinite Chat Mode:** Enable infinite chat mode for never-ending conversations, or set a specific number of turns.

* **🎛️ Full Control & Customization:**

  * Adjustable System Prompts for both Model A and Model B.

  * Customizable initial start message / prompt.

  * Set response token limits (`max_tokens`).

  * Timeout protection per turn.

  * Global **Pause**, **Resume**, and **Cancel / Clear** controls.

* **💬 Modern UI:** Dark-themed responsive design with chat bubbles, copy-to-clipboard buttons, and status logs.

* **📦 All-in-One Installer:** Windows packaging (`.exe`) via `electron-builder` & NSIS, including silent auto-installation of Ollama if missing.

## 📖 Complete User & Setup Guide

### 🚀 Part 1: Installation Guide for End Users

1. **Download the Setup:**

   * Grab the latest release (`Tailk Setup 1.0.0.exe`) from the repository releases or your build output.

2. **Run the Installer:**

   * Double-click `Tailk Setup 1.0.0.exe`.

   * *Note on Windows SmartScreen:* If Windows displays a warning (*"Windows protected your PC"*), click **More info** and then select **Run anyway**.

3. **Automatic Prerequisites:**

   * The setup will check in the background if Ollama is installed on your system.

   * If missing, it will automatically install Ollama for you in the background.

4. **Launch Tailk:**

   * Open the application via the desktop shortcut created during setup.

### 🛠️ Part 2: Installing & Managing Local LLMs

Before running an AI-to-AI chat, you need at least two local models installed on your computer.

1. **Find a Model:**

   * Click **Browse Model Library ↗** inside the app (or visit [ollama.com/library](https://ollama.com/library)).

   * Pick models suited for your hardware (e.g., `qwen2:0.5b`, `llama3`, `mistral`, or `phi3`).

2. **Install via the In-App Interface:**

   * Locate the **Install model** bar at the top of the app.

   * Enter the exact model tag (e.g., `llama3` or `qwen2:0.5b`).

   * Press **Enter** or click **Install**.

   * Monitor the live download progress bar in the main panel. Once finished, your dropdown menus will update automatically.

### 💬 Part 3: Running Your First AI Duel

1. **Select Models:**

   * Choose your first model from the **Model A** dropdown.

   * Choose your second model from the **Model B** dropdown.

2. **Configure Parameters:**

   * **Turns:** Define how many messages the models will exchange (e.g., `6` turns).

   * **Max. Length (Tokens):** Limit the length of each response (e.g., `150` tokens for punchy replies).

   * **Timeout (sec.):** Maximum response wait time per turn.

   * **Infinite Chat:** Check this box if you want the conversation to run indefinitely until stopped manually.

3. **Set Persona & Topic:**

   * **First Message / Start Topic:** Provide the initial statement or question Model A will react to.

   * **System Prompt A & B:** Define the behavioral persona or rules for each AI agent (e.g., *Skeptical Scientist vs. Optimistic Futurist*).

4. **Control the Execution:**

   * Click **Start** to begin the automated conversation.

   * Use **Pause** and **Resume** to pause or continue the live loop.

   * Click **Cancel / Clear** to stop execution immediately and clean up the conversation feed.

## 🛠️ Developer Setup & Build Instructions

### Prerequisites

* **Node.js (v18 or higher recommended):** Download and install Node.js from [nodejs.org](https://nodejs.org/). Verify your installation in terminal via `node -v` and `npm -v`.

* **Ollama:** Download and install [Ollama](https://ollama.com/) running locally.

### Local Development

1. **Clone the repository:**

   ```bash
   git clone https://github.com/YOUR-USERNAME/tailk-app.git
   cd tailk-app
   ```

2. **Install Node dependencies:**

   ```bash
   npm install
   ```

3. **Launch the desktop application:**

   ```bash
   npm start
   ```

### Building the Standalone `.exe` Installer

1. Download `OllamaSetup.exe` from [Ollama Download](https://ollama.com/download) and place it inside the `installer/` directory:

   ```text
   tailk-app/
   ├── installer/
   │   └── OllamaSetup.exe
   ```

2. Run the packaging command:

   ```bash
   npm run build
   ```

3. Locate your compiled setup file inside the `dist/` directory (e.g., `dist/Tailk Setup 1.0.0.exe`).

## 📜 License

This project is open-source and released under the [MIT License](LICENSE).