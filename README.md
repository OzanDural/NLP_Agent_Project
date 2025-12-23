# NLP_Agent_Project
An autonomous ReAct Agent for Aviation Flight Operations using RAG, Groq LLM, and Open-Meteo API
# ✈️ Aviation Flight Operations Agent (ReAct)

**An autonomous AI Agent designed to simulate a Flight Operations Dispatcher using the ReAct (Reasoning + Acting) architecture.**

This project transforms a standard LLM into an intelligent decision-support system that can query technical documents (RAG), fetch real-time weather data (API), and perform mathematical calculations to make "Go/No-Go" flight decisions.

---

## 🚀 Features

- **🧠 ReAct Architecture:** The agent follows a `Thought` -> `Action` -> `Observation` loop to solve complex problems step-by-step.
- **📚 RAG (Retrieval-Augmented Generation):** Uses a vector-based retrieval system to fetch static aircraft limitations (e.g., Boeing 737 Crosswind Limits) from a knowledge base.
- **☁️ Real-Time Data:** Integrates with **Open-Meteo API** to fetch live wind speed and temperature data for any global airport.
- **🧮 Robust Math Logic:** Includes a calculator tool to compute safety margins (e.g., `Limit - Current Wind`) accurately.
- **🛡️ Hallucination Control:** Implements specific system prompts and error handling to prevent syntax errors and manage non-existent locations.

---

## 📂 Repository Structure

- **`ReAct_Agent.ipynb`**: The main Python notebook containing the Agent logic, RAG engine, and Tool definitions.
- **`aircraft_dataset.txt`**: The knowledge base file containing technical limits for Boeing 737, Airbus A320, and Cessna 172.
- **`requirements.txt`**: List of Python dependencies required to run the project.
---

## 🛠️ Tools & Technologies

| Component | Technology | Description |
|-----------|------------|-------------|
| **LLM** | **Groq (Llama-3)** | The "Brain" responsible for reasoning and tool selection. |
| **API** | **Open-Meteo** | Provides real-time meteorological data without an API key. |
| **Vector Search** | **Cosine Similarity** | Custom `SimpleRAG` class for semantic search. |
| **Language** | **Python 3.10+** | Core programming language. |

---
## Architecture Diagram: 
<img width="2065" height="1160" alt="diagram_agent" src="https://github.com/user-attachments/assets/b13d3c19-7e56-40e7-9cb2-1b667092a480" />
---
