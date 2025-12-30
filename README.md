# NLP_Agent_Project
An autonomous ReAct Agent for Aviation Flight Operations using RAG, Groq LLM, and Open-Meteo API
## ✈️ Aviation ReAct Dispatcher Agent

This project transforms a static Language Model into an **Autonomous ReAct Agent** specialized for Aviation Dispatch operations. Powered by **Llama-3.3-70B**, the agent reasons, decides, and solves complex flight planning problems by interacting with technical documents and real-time external APIs.

## 🎯 Project Goal
The primary objective is to assist flight dispatchers in verifying safety limits and calculating operational costs. Unlike a standard LLM, this agent follows the **Thought -> Action -> Observation** cycle to ensure every decision is backed by technical data or live environmental conditions.

## 🏗️ System Architecture
Below is the logical flow of the agent's decision-making process:



```mermaid
graph TD
    User([User Query]) --> LLM[Llama-3.3-70B ReAct Engine]
    LLM --> Thought{Thought: Reasoning}
    Thought --> Action[Action: Tool Selection]
    Action --> Tools{External Tools}
    
    Tools --> RAG[(Knowledge Base - RAG)]
    Tools --> Weather[Weather API]
    Tools --> Finance[Finance API]
    Tools --> Calc[Calculator]
    
    RAG --> Obs[Observation: Raw Data]
    Weather --> Obs
    Finance --> Obs
    Calc --> Obs
    
    Obs --> LLM
    LLM --> Final[Answer: Final Dispatch Report]

---
## Architecture Diagram: 
<img width="2065" height="1160" alt="diagram_agent" src="https://github.com/user-attachments/assets/b13d3c19-7e56-40e7-9cb2-1b667092a480" />

---
