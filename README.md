<div align="center">

# 🤖 J.A.R.V.I.S.
### A Local-First AI Desktop Assistant for Windows

<img width="800" height="450" alt="JARVIS Banner" src="https://github.com/user-attachments/assets/04ba818a-bb38-4854-9b55-309c4270c2da" />

<br/><br/>

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-Agent%20Orchestration-1C3C3C?style=for-the-badge)
![ChromaDB](https://img.shields.io/badge/ChromaDB-Vector%20Memory-FF6F00?style=for-the-badge)
![RAG](https://img.shields.io/badge/RAG-Retrieval%20Augmented-4B8BBE?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active%20Development-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

**Your own Jarvis. Running locally. Answering to no cloud but yours.**

</div>

---

## 🧭 Overview

**JARVIS** is a **local-first AI desktop assistant** built for Windows — designed to feel less like a chatbot bolted onto your desktop and more like a genuine second brain sitting quietly in the background. It combines **retrieval-augmented generation (RAG)**, **persistent vector memory**, and a **graph-based agent orchestration layer** to hold context, retrieve knowledge, and act on your behalf — all without shipping your data off to someone else's server by default.

This isn't a wrapper around an API call. It's an evolving system: what started as a single conversational agent is being rebuilt into a **multi-agent architecture**, with specialized agents handling distinct responsibilities (reasoning, retrieval, tool execution, memory management) and coordinating through **LangGraph**.

---

## ✨ Core Features

| | |
|---|---|
| 🧠 **Persistent Memory** | ChromaDB-backed vector store gives JARVIS long-term recall across sessions — it remembers, it doesn't just respond. |
| 🔍 **RAG Pipeline** | Retrieval-augmented generation grounds answers in your own documents and context instead of hallucinated guesses. |
| 🕸️ **Agentic Orchestration** | LangGraph drives multi-step reasoning and tool use as a graph of decisions, not a single linear prompt. |
| 🖥️ **Local-First Design** | Built to run on-device where possible — your data stays on your machine. |
| 🎨 **Themeable Interface** | Multiple UI moods, from clean daylight views to a full dark "Midnight" aesthetic. |
| ⚠️ **System Awareness** | Built-in alerting and status indicators for critical or anomalous events. |

---

## 📸 Gallery

<div align="center">

### 🌓 Midnight Owl — Dark Mode Interface
<img width="800" src="https://github.com/user-attachments/assets/a7605427-fa69-416f-85ec-955ea51490c1" alt="MidnightOwl Dark Theme" />

<br/><br/>

### ⌨️ Typing Master — Command & Input Module
<img width="800" src="https://github.com/user-attachments/assets/f3563df6-be53-4aba-ba97-0066c985e09e" alt="TypingMaster Module" />

<br/><br/>

### ⚠️ Danger Zone — Alert & Anomaly System
<img width="800" src="https://github.com/user-attachments/assets/8af87fe1-ec83-468a-a2ba-d133747e841c" alt="DANGER Alert System" />

<br/><br/>

<table>
<tr>
<td width="50%">

**Dashboard View**
<img src="https://github.com/user-attachments/assets/a7541284-fde4-4acb-9ac2-f95ba078cd60" alt="Dashboard View" width="100%"/>

</td>
<td width="50%">

**Session View**
<img src="https://github.com/user-attachments/assets/03557315-3a10-4bfd-887a-e4f982e0e61d" alt="Session View" width="100%"/>

</td>
</tr>
</table>

### 🧩 Extended Interface View
<img width="800" src="https://github.com/user-attachments/assets/f9ee9640-2428-4a16-bea3-320018b8ee93" alt="Extended Interface" />

</div>

---

## 🏗️ Architecture

```
┌──────────────────────────────────────────────────────────┐
│                      User Interface                       │
└───────────────────────────┬────────────────────────────────┘
                             │
┌───────────────────────────▼────────────────────────────────┐
│                  LangGraph Orchestrator                   │
│   (routes intent → agent, manages graph-based reasoning)  │
└──────┬─────────────┬─────────────┬────────────┬────────────┘
       │             │             │            │
 ┌─────▼────┐  ┌─────▼─────┐ ┌─────▼─────┐ ┌────▼─────┐
 │ Reasoning │  │ Retrieval  │ │   Tool    │ │  Memory   │
 │   Agent   │  │   Agent    │ │  Agent    │ │  Agent    │
 │           │  │  (RAG)     │ │ (actions) │ │ (Chroma)  │
 └───────────┘  └────────────┘ └───────────┘ └───────────┘
```

Each agent owns a narrow responsibility; the orchestrator decides who acts, when, and with what context — the shift from a single monolithic prompt to a coordinated system of specialists.

---

## 🛠️ Tech Stack

- **Core:** Python
- **Agent Orchestration:** LangChain, LangGraph
- **Memory / Retrieval:** ChromaDB, RAG pipelines
- **Serving:** FastAPI
- **ML / Deep Learning:** PyTorch
- **Local Inference:** Ollama, GGUF quantization
- **Persistence:** SQLite
- **Containerization:** Docker
- **Cloud (in progress):** AWS

---

## 🚧 Roadmap — What's Being Built Right Now

- [ ] **Multi-Agent System** — decomposing the single-agent core into specialized, cooperating agents (reasoning, retrieval, tool execution, memory) coordinated via LangGraph
- [ ] **NLP Fine-Tuning** — fine-tuning models for sharper domain-specific understanding and more reliable intent parsing
- [ ] **IDE Integration** — bringing JARVIS into the development workflow directly, as an assistant embedded in the coding environment
- [ ] Expanded local-inference support and quantized model options
- [ ] Deeper long-term memory consolidation strategies

---

## ⚙️ Getting Started

```bash
# Clone the repository
git clone https://github.com/Vedant021004/jarvis.git
cd jarvis

# Set up environment
python -m venv venv
venv\Scripts\activate      # Windows

# Install dependencies
pip install -r requirements.txt

# Run JARVIS
python main.py
```

---

## 📄 License

Released under the **MIT License** — see [LICENSE](LICENSE) for details.

<div align="center">

*Built by [Ved](https://github.com/Vedant021004) — because a good assistant shouldn't need the cloud to know you.*

</div>
