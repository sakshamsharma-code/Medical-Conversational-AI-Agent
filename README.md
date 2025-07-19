# 🏥 Medical AI Agent using LangGraph & Gemini

This project is a **stateful conversational AI agent** designed for the **healthcare domain**, developed as part of the **IBM SkillBuild program** – _"From Learner to Builder: Become an AI Agent Architect"_.

It uses **LangGraph** to structure conversation flows and **Google Gemini (via LangChain)** as the LLM backend to generate smart, context-aware responses based on user inputs about symptoms and health conditions.

---

## 🔍 Project Overview

The AI agent simulates a medical assistant that:

1. **Greets the user** and asks for symptoms  
2. **Asks follow-up questions** like how long they've had the symptom and other relevant information  
3. **Uses memory** to store responses  
4. **Passes the full context** to Google Gemini (LLM)  
5. **Generates a medically coherent reply**, simulating a basic triage or health guidance

---

## 💻 Tech Stack

- **Python**
- **LangChain**
- **LangGraph**
- **Google Gemini** (via `langchain_google_genai`)
- **Jupyter Notebook**

---

## 🚀 How It Works

- Each step of the conversation (symptom input, duration, extra info) is represented as a **node** in a `LangGraph`.
- As the user responds, their answers are stored in a `state` dictionary.
- Finally, all stored data is combined and passed to **Gemini**, which returns a meaningful medical-style response.

---

## 🧪 Example Use Case

```
User: "I have a sore throat"
Agent: "Since how many days are you experiencing it?"
User: "For 3 days"
Agent: "Please provide more information about your condition"
User: "Also have a mild fever and difficulty swallowing"
Agent (LLM): [Gemini responds with a coherent summary or advice]
```

---

## 🧠 Why This Matters

This project demonstrates:
- How to build **stateful, multi-turn AI agents**
- How to apply **LLMs to real-world domains** like healthcare
- How **LangGraph** can structure decision flows like a finite state machine

---

## 📂 Run It Yourself

1. Clone the repo  
2. Install dependencies  
```bash
   pip install langgraph langchain langchain-google-genai google-generativeai
```
3. Run the Jupyter Notebook
4. Enter your Google Gemini API Key when prompted

---

## 📌 Author
Developed by Saksham Sharma under IBM Skill Builds learning program

---

## 📄 License
This project is licensed under the MIT License.
