# 🤖 Agentic Multi-Source Research Assistant

## 📌 Overview
This project implements an AI-powered research assistant that answers user queries by dynamically selecting and interacting with multiple external data sources.

Unlike traditional LLM-based systems, this solution follows an **agentic approach**, where the model decides *what action to take* and *which tool to use* based on the query.

---

## 🎯 Problem Statement
LLMs often produce hallucinated or incomplete answers when relying only on internal knowledge.

This project addresses this limitation by:
- Enabling real-time information retrieval
- Integrating multiple external knowledge sources
- Allowing the model to reason and act dynamically

---

## ⚙️ Architecture Flow

User Query → LLM Agent → Tool Selection → Tool Execution → Response Generation → Output

---

## 🧠 Core Concept: Agentic AI (ReAct Framework)

The system follows the **ReAct (Reason + Act)** paradigm:

1. **Thought** → Analyze the query  
2. **Action** → Select appropriate tool  
3. **Observation** → Retrieve data  
4. **Final Answer** → Combine and respond  

---

## 🔧 Tools Integrated

- 🌐 Web Search (DuckDuckGo) → real-time information  
- 📚 Wikipedia API → general knowledge  
- 📄 Arxiv API → research papers  

---

## 🚀 Key Features

- Dynamic tool selection based on query intent  
- Multi-source data retrieval for higher accuracy  
- Reduced hallucination compared to standalone LLMs  
- Transparent reasoning with intermediate steps  
- Interactive UI for real-time responses  

---

## 🛠️ Tech Stack

- **LLM**: Groq (LLaMA 3.1)
- **Framework**: LangChain
- **Frontend**: Streamlit
- **APIs**: Wikipedia, Arxiv, DuckDuckGo
- **Concepts**: Agentic AI, ReAct, Prompt Engineering

---

## 📊 Results

- Improved answer accuracy using multi-source retrieval  
- Reduced hallucination through tool-based grounding  
- Handles diverse queries across domains (research, general knowledge, real-time data)

---

## 🧪 How to Run

```bash
git clone https://github.com/Aniket58-tech/Agentic-Multi-Source-Research-Assistant.git
cd Agentic-Multi-Source-Research-Assistant
pip install -r requirements.txt
streamlit run app.py
