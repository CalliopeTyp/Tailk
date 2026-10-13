# Tailk – Local AI Conversation App

**Tailk** is a sleek, local Electron desktop application that enables an automated, infinite conversation or debate between two local AI language models powered by [Ollama](https://ollama.com/).

---

## Features

- **Local AI Duels:** Run debates or conversations between any installed Ollama models (e.g., Llama 3, Mistral, Qwen).
- **Real-Time Streaming:** Watch models generate responses token-by-token in a modern chat bubble interface.
- **In-App Model Management:** Download new models directly inside the UI using `ollama pull` with real-time download progress and status updates.
- **Customizable Settings:** Adjust System Prompts, initial start topics, token length caps, and timeout limits.
- **Infinite Chat Mode:** Switch seamlessly between a fixed number of turns and an endless conversation loop.
- **Full Control:** Pause, resume, or cancel/clear conversations at any time.

---

## Prerequisites

Make sure the following tools are installed on your system before running the application:

1. **Node.js** (includes `npm`):  
   Download and install the LTS version:  
   👉 [https://nodejs.org/](https://nodejs.org/)

2. **Ollama**:  
   Download, install, and run the local LLM runner:  
   👉 [https://ollama.com/](https://ollama.com/)

---

## How to Run from Source

Since this project runs directly from the source folder without a pre-built executable, you can start the application easily via your terminal or PowerShell:

### 1. Open the Project Folder
Go in the projectfolder, copy the bash and bast it in your Terminal/Powershell
```bash
cd "YOUR_COPIED_BASH"

### 2. Install Dependencies
Install all required Node.js packages (Electron, Ollama SDK, etc.):

```bash
npm install

###3. Run it
Type this command in your Terminal/Powershell
```bash
npm start
