# 🔎 LangChain Research Assistant Agent (Streamlit + Groq)

This project is an interactive AI-powered research assistant that can search the web, query Wikipedia, and retrieve academic papers from arXiv. It uses LangChain agents with Groq-hosted LLMs and provides a real-time chat interface built with Streamlit.

The assistant is designed to act like a smart research companion that reasons, searches, and explains results in natural language while showing its internal thought process using Streamlit callbacks.

---

## 🚀 Project Overview

The Research Assistant Agent integrates multiple external knowledge sources and a powerful LLM to answer user queries intelligently. It supports:

- Web search using DuckDuckGo  
- Academic paper retrieval from arXiv  
- Knowledge lookup from Wikipedia  
- Real-time reasoning and streaming responses  
- Interactive chat UI with memory  

This makes it ideal for students, researchers, and developers who want fast, AI-assisted research insights.

---

## 🧠 How It Works

The system uses a **LangChain ReAct agent** to decide which tool to use for each query. The agent dynamically chooses between:

- DuckDuckGo Search  
- Wikipedia API  
- arXiv API  

The Groq-hosted LLaMA 3 model processes the query, reasons about it, calls the appropriate tool, and returns a final answer to the user. Streamlit is used to create a conversational UI and display the agent’s reasoning steps.

---

## 📂 Project Structure

├── app.py # Main Streamlit application
├── .env # Environment variables (Groq API key)
├── requirements.txt # Python dependencies
└── README.md # Project documentation


---

## ⚙️ Installation

### 1. Clone the Repository
```bash
git clone https://github.com/senpaisaul/Research-assistant-agent.git
cd Research-assistant-agent
```

### 2. Install requirements
```bash
pip install -r requirements.txt
```

### 3. Add Groq API Key
```bash
GROQ_API_KEY=your_groq_api_key_here
```

### 4. ▶️ Run the Application
```bash
streamlit run app.py
```

###
