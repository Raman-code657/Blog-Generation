# 📝 Blog Generation App

The **Blog Generation App** is an AI-powered project that automatically generates blog content using **Large Language Models (LLMs)**.  
It is designed with a **graph-based architecture** that connects different components like nodes, states, and workflows for flexible and extensible content creation.

---

## 🚀 Features
- **AI Blog Writing** – Generate structured blog posts from topics, keywords, or JSON prompts.  
- **Graph-Based Workflow** – Uses modular `nodes`, `states`, and `graphs` to manage the flow of text generation.  
- **Custom LLM Integration** – Powered by **Groq LLM** (`groqllm.py`) for fast and efficient text output.  
- **Extensible Architecture** – Add new nodes, states, or LLM providers without breaking the workflow.  
- **Configurable** – Define workflows with `langgraph.json` and control input prompts with `request.json`.  

---

## 📂 Project Structure
bloggeneration/
├── .gitignore             # Git ignore file
├── .python-version        # Python version tracking
├── app.py                 # Entry point for running the app
├── main.py                # Alternative main script for execution
├── langgraph.json         # Defines workflows and graph configuration
├── request.json           # Example request payload for blog generation
├── requirements.txt       # Python dependencies
├── pyproject.toml         # Project metadata and dependencies
├── uv.lock                # Lockfile for uv (dependency manager)
├── src/
│   ├── init.py
│   ├── graphs/
│   │   ├── init.py
│   │   └── graph_builder.py    # Builds the workflow graph
│   ├── llms/
│   │   ├── init.py
│   │   └── groqllm.py          # Groq LLM integration
│   ├── nodes/
│   │   ├── init.py
│   │   └── blog_node.py        # Blog generation node
│   └── states/
│       ├── init.py
│       └── bloggeneration.py   # Blog state management
└── README.md              # Project documentation
