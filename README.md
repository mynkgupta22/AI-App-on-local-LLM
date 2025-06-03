# Local AI Writer: Blog Intro Generator

## 📝 App Type Selected
**AI Writer** – Generates a compelling blog introduction from a user-provided topic using a local LLM.

---

## 🚀 Features

- **Prompt input box:** Enter your blog topic.
- **Model output display:** See the generated blog introduction.
- **Temperature setting:** Adjust creativity/randomness of the output.
- **Loading UI:** Spinner and button state during generation.
- **Output logging:** Output is shown in the UI and logged to the browser console.

---

## 🧠 Model Used

- **Default:** `llama3` (can be changed in the code)
- **Backend:** [Ollama](https://ollama.com/) (runs the LLM locally)

---

## 🖥️ How to Run Locally

### 1. Install Ollama

- Download and install Ollama from [https://ollama.com/download](https://ollama.com/download)
- Start Ollama (it runs as a background service)

### 2. Download the Model

Open a terminal and run:
```
ollama pull llama3
```
*(Or replace `llama3` with your preferred model, e.g., `mistral`, `phi`, etc.)*

### 3. Run the App

1. Open `index.html` in your browser (double-click or use a local server).
2. Make sure Ollama is running and the model is downloaded.
3. Enter a topic, adjust temperature if desired, and click **Generate Blog Intro**.

---

## ⚙️ Setup Instructions

1. **Clone this repository:**
   ```
   git clone <your-repo-url>
   cd <repo-folder>
   ```

2. **Start Ollama** (if not already running):
   ```
   ollama serve
   ```

3. **Open `index.html`** in your browser.

---

## 📝 Notes

- The app communicates with Ollama at `http://localhost:11434/api/generate`.
- Ensure your browser allows requests to `localhost:11434`.
- If you want to use a different model, change the `modelName` variable in the script section of `index.html`.

