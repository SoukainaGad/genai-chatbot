# 💬 GenAI Chatbot

### 🧠 Overview

**Soukaina’s GenAI Chatbot** is a conversational AI web app built with **Streamlit** and **LangChain**, powered by **Groq’s Llama-3.3-70B model**.
It provides fast, context-aware, and conversational responses directly in your browser — no backend setup required.

The chatbot supports **multi-turn conversations**, remembering previous messages in the same session for natural, human-like interaction.

---

### ✨ Featureeeeees

*  **Conversational Memory** — remembers previous messages in the chat.
*  **Groq Llama-3.3-70B** — high-speed reasoning and response generation.
*  **LangChain Integration** — modular, extendable, and easy to customize.
*  **Streamlit UI** — clean, responsive, and browser-ready.
*  **Secure API Key Handling** via `.env` and `python-dotenv`.

---

### ⚙️ How It Works

1. The user sends a message in the Streamlit chat interface.
2. The chatbot records the conversation in memory (`st.session_state`).
3. Each new message is passed to the **Llama-3.3-70B model** using LangChain’s `ChatGroq` wrapper.
4. The model returns a context-aware reply, which is displayed instantly in the Streamlit app.

---

### 🧰 Tech Stack

*  **Python 3.10+**
*  **Streamlit** — interactive web app interface
*  **LangChain** — conversation orchestration
*  **Groq API** — Llama-3.3-70B model for ultra-fast inference
*  **python-dotenv** — secure environment variable management

---

### 🛠️ Setup Instructions (Local)

**1. Clone the repository**

```bash
git clone https://github.com/SoukainaGd/genai-chatbot.git
cd genai-chatbot
```

**2. Create a virtual environment**

```bash
python -m venv venv
source venv/bin/activate   # Mac/Linux  
venv\Scripts\activate      # Windows
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

**4. Create a `.env` file**

```bash
GROQ_API_KEY=your_groq_api_key_here
```

**5. Run the app**

```bash
streamlit run app.py
```

---

### ☁️ Streamlit Cloud Deployment

1. Connect your GitHub repo to **Streamlit Cloud**.
2. Go to **Settings → Secrets** and add your key:

   ```
   GROQ_API_KEY = your_groq_api_key_here
   ```
3. Streamlit will automatically deploy your chatbot.

---

### 💡 Example Use Cases

* Q&A assistant for websites or portfolios
* Teaching / learning aid
* Knowledge-base or documentation chatbot
* Lightweight front-end for LLM experimentation

---

### ⚖️ Disclaimer

This chatbot uses **AI-generated responses** and should not be treated as professional, legal, or medical advice.
Its purpose is to demonstrate **responsible and transparent GenAI application design**.
