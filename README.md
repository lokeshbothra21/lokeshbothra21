# Hi, I'm Lokesh 👋

**AI Engineer in Bangalore. I build agentic AI and RAG systems that run in production, and I measure whether they actually work.**

Most of my work is LangGraph multi-agent systems, hybrid retrieval and LLM evaluation (RAGAS plus custom metrics), on FastAPI and Google Cloud.

## 🛡️ Featured: [AegisOps](https://github.com/lokeshbothra21/aegisops)

An autonomous incident-response agent over real OpenTelemetry data. Deterministic rules detect the incident. A LangGraph agent investigates logs, metrics, traces and recent changes. Then **code, not the LLM, checks every claim** before a human approves one of four safe fixes.

- Fault → open incident in **57 s** on a 15-service system, with zero false positives during warm-up
- The verifier caught the model citing a metric that doesn't exist and cut its confidence from **0.86 to 0.57**
- 9 read-only telemetry tools exposed over **MCP**, with every tool result treated as untrusted input
- 17 ADRs, 109 tests (95% coverage), `mypy --strict`, CodeQL and keyless Cloud Run deploys
- Built in public, with a [day-by-day engineering log](https://github.com/lokeshbothra21/aegisops/tree/main/docs/learning) that records what broke as well as what worked

## What I've built at work

| System | What I did |
|---|---|
| **Scientific literature RAG** | Rebuilt the pipeline in LangGraph with sub-question decomposition, confidence-based abstention and prompt-injection isolation. RAGAS answer correctness went from **0.68 → 0.79** and context precision from **0.54 → 0.64**. Uses hybrid BM25 + FAISS search with cross-encoder reranking. |
| **Multi-agent simulation platform** | LangGraph agents that run GROMACS, Quantum ESPRESSO and ORCA on containerised HPC. A self-verification step checks generated artifacts in a sandbox before any response reaches a user. |
| **Text-to-SQL analytics agents** | Gemini agents with MCP access to BigQuery, SQL validation and self-correction loops (**95%+ query accuracy**). AI-generated Plotly code runs in a Docker sandbox, and Entra ID RBAC enforces access per dataset. |
| **Enterprise RAG assistant** | Async document ingestion with Docling and Celery, retrieval over pgvector and Redis, and delta sync of mailboxes through Microsoft Graph. |

Those systems are closed-source. AegisOps is where you can read my code.

## Toolbox

**AI:** LangGraph · LangChain · DeepAgents · Google ADK · MCP · RAG and multimodal RAG · hybrid retrieval · RAGAS  
**Backend:** Python · FastAPI · SQLAlchemy · Celery · PostgreSQL · pgvector · Redis · BigQuery · FAISS · ChromaDB  
**Infra:** GCP (Cloud Run, Cloud Build, Cloud SQL) · Docker · Kubernetes · OpenTelemetry · GitHub Actions

## Certifications

- Google Cloud Professional Cloud Architect (2026)
- Microsoft Certified: Azure AI Engineer Associate (2026)
- Google Cloud Associate Cloud Engineer (2025)

## Get in touch

📫 [lokesh8946891910@gmail.com](mailto:lokesh8946891910@gmail.com) · [LinkedIn](https://www.linkedin.com/in/lokeshbothra/) · [LeetCode](https://leetcode.com/u/lokesh21bothra/)

<sub>he/him</sub>
