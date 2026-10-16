<h1 align="center">Hi, I'm Vishwesh Murali 👋</h1>

<p align="center">
  <b>Data Science M.S. · AI / Data Engineer</b><br/>
  I build agentic AI and data systems that are <b>tested, measured, and honest about their limits</b>.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/vishwesh-murali-5236671a8/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <img src="https://img.shields.io/badge/Based%20in-Bloomington%2C%20IN-555555?logo=googlemaps&logoColor=white" alt="Location"/>
  <img src="https://img.shields.io/badge/Open%20to-AI%20%2F%20Data%20roles-2EA043" alt="Open to roles"/>
</p>

---

## 👨‍💻 About me

- 🎓 **M.S. in Data Science**, Indiana University Bloomington (2024 – 2026). B.E. in Computer Science, Sri Venkateswara College of Engineering.
- 🔬 **Faculty Assistant (Deep Learning)** at Indiana University since Jan 2026: a video-based behavior-analysis pipeline using RNNs and DeepLabCut computer vision, with statistical validation of the results.
- 💼 **Programmer Analyst at Cognizant** (2022 – 2024): Python/SQL data pipelines and data-quality automation, plus performance engineering for high-traffic enterprise web applications (JMeter, LoadRunner, Neoload; AWS IAM/EC2).
- 🧪 I care about **evaluation**. Every project below ships with tests and an honest *Limitations* section, including where my own numbers fall short.
- 🌱 Currently exploring: agentic workflows, MCP servers, RAG evaluation (RAGAS), and prompt-injection defenses.

---

## 🚀 Featured projects

### 🧭 [SkillMapper](https://github.com/VishweshMurali/skillmapper): agentic RAG resume ↔ job evaluator
Compares a resume against a job description, retrieves supporting evidence, and returns a structured verdict. Low-confidence cases escalate to a human reviewer.
- **Hybrid retrieval:** BM25 + ChromaDB dense search fused with Reciprocal Rank Fusion, written by hand so the fusion math is unit-testable.
- **Section-first chunking:** a measured fix for chunks that straddled resume sections (RAGAS comparison is reproducible from the repo).
- **Two architectures:** an in-process LangGraph agent with retry/escalate routing, *and* a 5-server MCP design (one server per pipeline stage) driven by an orchestrator.
- **Verified:** 64 unit tests + 11 live Ollama integration tests, runs fully local, no paid API keys.
- **Stack:** Python · LangGraph · ChromaDB · rank_bm25 · MCP · Ollama · RAGAS · Streamlit

### 🧾 [HILT](https://github.com/VishweshMurali/hilt): human-in-the-loop invoice verification
An LLM extracts invoice fields, but **deterministic validators, not the model's confidence, decide** whether to auto-approve or escalate to a reviewer.
- **Red-teamed on purpose:** I broke my own first version with a prompt-injection invoice, then fixed it: source-text grounding, injection detection, and duplicate-invoice checks.
- **48-case labeled eval** (including 8 adversarial) plus 41 offline unit tests. The README states plainly what that score does and does not prove.
- LangGraph `interrupt()` pauses on escalation and resumes from a Streamlit reviewer UI with a full audit trail.
- **Stack:** Python · LangGraph · Groq · Pydantic · SQLite · Streamlit

### 🎤 [InterviewPrep](https://github.com/VishweshMurali/InterviewPrep): adaptive interview tutor
Generates questions from your own notes, resume, and a target job description, then scores answers with a **panel of LLM judges** and targets your weak concepts next.
- RAG over your materials, multi-judge scoring with disagreement flagging, adaptive difficulty (logistic regression), and a prerequisite knowledge graph.
- **Stack:** Python · Streamlit · FastAPI · LangChain · ChromaDB · sentence-transformers · scikit-learn

### 💬 [Insightify](https://github.com/VishweshMurali/Insightify): multilingual review sentiment dashboard
Loads product reviews (CSV or scraped), classifies sentiment across languages, and surfaces trends, word clouds, and the aspects customers praise or complain about.
- **Stack:** Python · Streamlit · Hugging Face Transformers · scikit-learn · langdetect

---

## 🛠️ Toolbox

| | |
|---|---|
| **Languages** | ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?logo=postgresql&logoColor=white) ![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white) ![R](https://img.shields.io/badge/R-276DC3?logo=r&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black) |
| **GenAI / Agents** | ![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?logo=langchain&logoColor=white) ![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?logo=langchain&logoColor=white) ![MCP](https://img.shields.io/badge/MCP-000000) ![Ollama](https://img.shields.io/badge/Ollama-000000?logo=ollama&logoColor=white) ![ChromaDB](https://img.shields.io/badge/ChromaDB-FF6446) ![RAGAS](https://img.shields.io/badge/RAGAS-6E40C9) |
| **ML / Data** | ![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white) ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white) ![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?logo=huggingface&logoColor=black) |
| **Apps & APIs** | ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?logo=streamlit&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=white) |
| **Cloud / Tools** | ![AWS](https://img.shields.io/badge/AWS-232F3E?logo=amazonwebservices&logoColor=white) ![GCP](https://img.shields.io/badge/Google%20Cloud-4285F4?logo=googlecloud&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white) ![JMeter](https://img.shields.io/badge/JMeter-D22128?logo=apachejmeter&logoColor=white) |

**Certification:** Google Cloud Digital Leader

---

## 🧰 How I work

- **Measure before claiming.** I benchmark, then report the result even when it's unflattering (my async-embedding optimization gave *no* speedup, and the README says so).
- **Attack my own systems.** Adversarial test cases and prompt-injection checks go in alongside the happy path.
- **Keep a human in the loop** where a wrong answer is costly, and make escalations explain *why*.
- **Document the limits.** Every repo has a *Limitations* section.

---

## 📬 Let's connect

I'm open to **AI engineering, GenAI, and data engineering** roles (open to relocation within the US).
The best way to reach me is [LinkedIn](https://www.linkedin.com/in/vishwesh-murali-5236671a8/).

<p align="center"><i>Thanks for stopping by. If a project here is useful, a ⭐ is always appreciated.</i></p>
