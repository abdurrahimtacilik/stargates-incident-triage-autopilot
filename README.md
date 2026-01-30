# StarGates – Incident Triage Autopilot

StarGates is an agentic AI proof-of-concept built with IBM watsonx Orchestrate that automatically transforms unstructured incident alerts into structured, actionable operational outputs.

---

## 🚀 Project Overview (EN)

Enterprise operations teams spend significant time manually triaging incidents:
- Interpreting unstructured alerts
- Searching runbooks
- Collecting logs and metrics
- Creating incident tickets

StarGates automates this workflow using a multi-agent architecture orchestrated by IBM watsonx Orchestrate.

Given a single alert, the system:
1. Determines severity and business impact  
2. Selects the most relevant runbook  
3. Collects supporting evidence via tools  
4. Generates root-cause hypotheses  
5. Produces an action checklist and ticket draft  

This project demonstrates how agentic AI can be applied to real enterprise workflows beyond traditional chatbots.

---

## 🧠 Architecture

StarGates uses a multi-agent architecture:
- **Sentinel Agent** – Alert analysis and orchestration
- **Evidence Collector Agent** – Log and metric collection
- **RCA Agent** – Root-cause hypothesis generation

IBM watsonx Orchestrate serves as the orchestration core.

See: `docs/architecture.md`

---

## 🎥 Demo

A full video demonstration is available here:  
👉 *(xxxx add public video URL)*

---

## 📁 Repository Contents

- `/agents` – Agent role definitions  
- `/tools` – Tool specifications (mocked)  
- `/knowledge` – Synthetic runbooks and incident data  
- `/docs` – Architecture and demo documentation  

---

## ⚠️ Disclaimer

This project uses fully synthetic and mock data for demonstration purposes only.  
No personal or sensitive data is included.

---

## 🏆 Hackathon Submission

Built for the IBM AI Demystified Hackathon using IBM watsonx Orchestrate.

---

## 📜 License

MIT License
