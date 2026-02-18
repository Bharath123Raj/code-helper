 Code Helper 🤖

**Code Helper** is an AI-powered coding assistant built with LangGraph.

It works like a multi-agent development team that can take a natural language request and transform it into a complete, working project — file by file — using real developer workflows.

---

## 🏗️ Architecture

### Planner Agent
Analyzes your request and generates a detailed project plan.

### Architect Agent
Breaks down the plan into specific engineering tasks with explicit context for each file.

### Coder Agent
Implements each task, writes directly into files, and uses available tools like a real developer.

---

## 🧠 Code Helper Agent Flow

User Prompt
↓
Planner Agent → Project Plan
↓
Architect Agent → File-Level Tasks
↓
Coder Agent → Code Implementation


---

## 🚀 Getting Started

### Prerequisites

- Make sure you have **uv** installed. Follow the official uv installation guide.
- Create a **Groq account** and generate your API key.

---

## ⚙️ Installation and Startup

### 1. Create a virtual environment

```bash
uv venv
source .venv/bin/activate
2. Install dependencies
uv pip install -r pyproject.toml
3. Environment variables
Create a .env file and add the variables listed in .sample_env:

cp .sample_env .env
Then update the values inside .env.

4. Run the application
python main.py
🧪 Example Prompts
Try giving Code Helper prompts like:

Create a to-do list application using HTML, CSS, and JavaScript.

Create a simple calculator web application.

Create a simple blog API in FastAPI with a SQLite database.

✨ Features
Multi-agent workflow (Planner → Architect → Coder)

Converts natural language into full projects

File-by-file implementation

Real developer-style tooling

Modular and extensible design
