# Manvik Talwar

Final-year CS major, AI/ML. I build systems that have to keep working when something goes wrong — and I measure whether they do.

Most of what I write ends up being retrieval, agent orchestration, or local inference — the parts where the model is only one component and everything around it decides whether the thing is usable. Lately that's meant caring a lot about evaluation and about failure modes: benchmark harnesses, ablations, fail-closed defaults, and knowing when a system should refuse to act instead of guessing.

Three engineering internships so far — local LLM inference for insurance claims adjudication, production analytics APIs, and an enterprise RAG deployment.

**Right now:** finishing a first-author paper on deep learning watermarking, and taking IntelliOps from dry-run to real Kubernetes remediation.

---

### Projects

**[Deep Learning Watermarking](https://github.com/CodexManvik/Deep-Learning-Based-Watermarking)** — first author, manuscript in preparation

Invisible 256-bit watermarking that embeds into the Haar DWT LL sub-band via a learned CNN. The interesting part is the attack simulator: JPEG compression is made differentiable with a straight-through estimator on DCT quantisation, so recovery-loss gradients flow back through the attack and train the encoder for robustness against it. Trained across natural photography, chest X-rays and CT — 37.3 dB PSNR, 0.97 SSIM, 3.2% clean bit error rate.

`TensorFlow` · `Keras` · `WaveTF` · `differentiable JPEG` · `50k mixed-domain corpus`

**[IntelliOps CoE](https://github.com/CodexManvik/intelliops)** — agentic AIOps, closed loop

Six services over a Redis Streams event bus that collapse alert storms into Situations, diagnose them, and execute reversible remediation. The whole system is async except one call — `action → governance` approval — so the human-in-the-loop guarantee is enforced by the call graph rather than by policy. Anomaly detection is online: a per-metric running z-score baseline with a warm-up gate, because a cold-started service otherwise flags its own startup as an incident. Remediation outcomes feed back as training data, and playbooks graduate from human-approved to automatic once they've earned it. Remediation is dry-run by default; real Kubernetes execution sits behind a mode switch.

`FastAPI` · `Redis Streams` · `River` · `Kubernetes` · `Prometheus` · `React` · `Docker Compose` · `13 ADRs`

**[Aethel](https://github.com/CodexManvik/Aethel)** — local-first AI agent runtime

A desktop agent running entirely local inference, with a step-budgeted tool loop over filesystem, shell and web. Every mutation goes through a permission manifest and an audit log with one-click rollback. The part I'm most interested in is Reflective Skill Memory — the agent turns finished tasks into readable markdown skills, tracks how they perform, and promotes or retires each one on measured success rate. Behaviour changes without touching weights, and you can read and edit what it learned.

`llama.cpp` · `FastAPI` · `Tauri` · `LanceDB` · `faster-whisper`

**[FloatChat](https://github.com/CodexManvik/FloatChat-AI)** — natural language over oceanographic data

Ask questions in plain English about ARGO ocean float measurements and get charts back. Dual-query backend: ChromaDB handles semantic lookup, and a separate path generates SQL against PostgreSQL on the fly for anything numeric. Dashboard has KPI cards, depth profiles, time series and geospatial maps. Smart India Hackathon 2025 national semi-finalist.

`Streamlit` · `Plotly` · `ChromaDB` · `PostgreSQL` · `Ollama`

**[Interview Mirror](https://github.com/CodexManvik/Interview-Mirror)** — real-time multimodal interview coach

Reads posture, facial signals and speech together while you practise, and streams feedback live rather than scoring you at the end. Getting pose, face and audio pipelines to run concurrently under a latency budget tight enough to feel real-time was most of the work.

`MediaPipe` · `faster-whisper` · `WebSockets` · `FastAPI` · `SQLite`

---

### Stack

`Python` · `TensorFlow` · `PyTorch` · `FastAPI` · `LangGraph` · `llama.cpp` · `Ollama` · `River` · `PostgreSQL` · `LanceDB` · `ChromaDB` · `Redis Streams` · `Kubernetes` · `Prometheus` · `Docker` · `TypeScript` · `React` · `Next.js` · `Azure`

---

Happy to talk about retrieval evaluation, AIOps, local inference, or watermarking — [manvik.talwar@gmail.com](mailto:manvik.talwar@gmail.com) · [LinkedIn](https://linkedin.com/in/manvik-talwar) · [codexmanvik.github.io](https://codexmanvik.github.io)
