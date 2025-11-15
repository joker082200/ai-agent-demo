# ai-agent-demo

# AI Agent Demo — Autonomous Research & Report Generator

This project demonstrates a minimal **AI Agent** that can  
**plan tasks, use external tools, gather information, and generate a final report automatically**.

Unlike a normal ChatGPT API call (which only generates text),  
this agent **thinks, decides, and acts** through a multi-step loop.

---

## ✨ Key Features (Agent-Specific)

### ✔ 1. Task Planning  
The agent automatically breaks down vague user requests into actionable steps.

Example:  
**“Create a report on recent AI Agent frameworks.”**  
The agent will determine on its own:

1. What topics to research  
2. What keywords to search  
3. How to structure the report  
4. How to finalize it in Markdown  

---

### ✔ 2. Autonomous Tool Use  
The agent can call external tools **without being explicitly told when**.

It uses:

- **SerpAPI** for web search  
- **Local file output** to store results

This showcases behavior that standard ChatGPT API calls cannot perform on their own.

---

### ✔ 3. Multi-Step Reasoning & Action Loop  
The agent follows a loop of:

**Think → Act → Observe → Decide Next Step**

During one request, it may:

- Execute multiple web searches  
- Aggregate data  
- Summarize and reorganize information  
- Write the final report as a file (`report.md`)

---

### ✔ 4. Report Output as a File  
The final report is saved locally (Markdown format).  
The agent decides *when* to write the file and *what* to include.

---

## 🏗 Architecture

- **LLM:** OpenAI API  
- **Agent Framework:** LangChain (ReAct-style agent)  
- **Tooling:** SerpAPI (web search)  
- **Output:** Markdown report stored locally

---

## 📦 Requirements

- Python 3.9+
- Required packages (see `requirements.txt`):

