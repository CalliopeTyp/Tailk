# Tailk – Local AI Conversation App

**Tailk** is a sleek, local Electron desktop application that enables an automated, infinite conversation or debate between two local AI language models powered by [Ollama](https://ollama.com/).

---

## Features

- **Local AI Duels:** Run debates between any installed Ollama models (e.g., Llama 3, Mistral, Qwen).
- **Real-Time Streaming:** Watch models generate responses token-by-token in a modern chat bubble interface.
- **In-App Model Management:** Download new models directly inside the UI using `ollama pull` with real-time download progress.
- **Customizable Dynamics:** Adjust System Prompts, initial start topics, token length caps, and timeout limits.
- **Infinite Chat Mode:** Switch seamlessly between a fixed number of turns and an endless conversation loop.
- **Full Execution Control:** Pause, resume, or cancel/clear conversations at any time.

---

## Prerequisites

Make sure the following tools are installed on your system before running the application:

1. **Node.js** (includes `npm`):  
   Download and install the LTS version:  
   👉 [https://nodejs.org/](https://nodejs.org/)

2. **Ollama**:  
   Download and install the local LLM runner:  
   👉 [https://ollama.com/](https://ollama.com/)

3. **Git** *(optional, for cloning the repository)*:  
   👉 [https://git-scm.com/](https://git-scm.com/)

---

## How to Run (Development Mode)

Since pre-built binary installers (`.exe`) are not distributed with the source code, you can easily run the application directly from your terminal or PowerShell:

### 1. Clone or Download the Repository

Clone this repository or download and extract the ZIP archive:

```bash
git clone [https://github.com/YOUR_USERNAME/tailk-app.git](https://github.com/YOUR_USERNAME/tailk-app.git)
cd tailk-app
