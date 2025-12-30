# NLP_Agent_Project
An autonomous ReAct Agent for Aviation Flight Operations using RAG, Groq LLM, and Open-Meteo API
## ✈️ Aviation ReAct Dispatcher Agent

This project transforms a static Language Model into an **Autonomous ReAct Agent** specialized for Aviation Dispatch operations. Powered by **Llama-3.3-70B**, the agent reasons, decides, and solves complex flight planning problems by interacting with technical documents and real-time external APIs.

## 🎯 Project Goal
The primary objective is to assist flight dispatchers in verifying safety limits and calculating operational costs. Unlike a standard LLM, this agent follows the **Thought -> Action -> Observation** cycle to ensure every decision is backed by technical data or live environmental conditions.
##Key Features
-ReAct Reasoning: Uses the "Reasoning and Acting" framework to decompose complex aviation queries into logical steps.

-Custom RAG Engine: A built-from-scratch Retrieval-Augmented Generation system using Cosine Similarity and TF-IDF style vectorization.

-Infinite Loop Protection: Includes a unique state-tracking mechanism to prevent the agent from repeating the same failed actions.

-Live External APIs: * Open-Meteo: For real-time wind speed and weather conditions.

-Exchange Rate API: For live USD to TRY currency conversions.

-Cost Tracking: Real-time monitoring of token usage and operational costs ($).

<img width="2065" height="1160" alt="mermaid-diagram-2025-12-30-152734" src="https://github.com/user-attachments/assets/4c5eb83d-1f1e-4e58-91ee-09b06f4511de" />
