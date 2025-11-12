## 🧠 IUFlowGen – Conference Demo

IUFlowGen is a prototype system developed for the **Conference AI Demonstration**.  
It showcases intelligent flowchart generation from text using LLM-based retrieval, semantic embeddings, and complexity-aware node linking.

This repository provides all setup instructions to **install, configure, and run IUFlowGen locally or on a demo server**.

---
## 🔧 Features

- ✅ End-to-end flowchart generation from complex procedural text
- 🧠 Local LLM integration via Ollama (e.g., `phi4`, `deepseek-r1`)
- 🔍 LightRAG: semantic + structural retrieval for context precision
- 🧰 DOT + Graphviz flowchart generation with beautification
- 🧭 Interactive frontend for review, querying, zooming, and toggling layouts
- 🔐 100% local execution — no API keys or internet required

---
## 📂 Folder Structure
Here's a breakdown of the project's directory structure:

-   `backend.py`: The core logic for text processing, RAG implementation, and the algorithms responsible for generating the flowchart graphs.
-   `app.py`: The web application built with Streamlit, providing the user interface and incorporating D3.js for rendering interactive flowcharts.
-   `input/`: Contains sample procedural documents that can be used for testing, demonstration, and training purposes.
-   `README.md`: This file, providing an overview and guide to the IUFlowGen project.

## 🚀 Getting Started

### Requirements

- Python 3.11+
- [Ollama](https://ollama.com) installed and running
- Graphviz installed (`dot` CLI should be available)
- `pip install -r requirements.txt`
### Setup

```bash
# Clone repository
git clone https://github.com/Khim3/Conference_Demo.git
cd Conference_Demo

# Install dependencies
pip install -r requirements.txt

# Fill in the .env file with SSH server details 
INTERMEDIATE_PASS= password_for_intermediate_server
MAIN_PASS= password_for_main_server

# Run application
streamlit run app.py
```
