### hey, i'm manvik

final-year cs (ai/ml) at manipal university jaipur. i mostly build llm stuff that has to keep working when nobody's watching: retrieval, agents, local inference, and the unglamorous guardrails around them.

interned at niva bupa (claims adjudication with a local llm), techlearn (backend analytics apis) and path infotech (enterprise rag on azure).

#### things i've built

- **[intelliops](https://github.com/CodexManvik/intelliops)**: aiops platform for the deloitte capstone. groups alert storms into incidents, works out the root cause, fixes things on kubernetes and rolls back if the fix doesn't hold. the llm gets a short list of allowed actions and has to ask a human first. seven services, 860+ tests.
- **[aethel](https://github.com/CodexManvik/Aethel)**: desktop agent that runs entirely on your machine. it writes down how it did each task as a markdown skill, and once a skill has worked the same way three times it skips the llm and just replays it. a small cpu model handles intent routing in ~0.2s (0.91 precision/recall). shipped v2 with an installer.
- **[interview mirror](https://interview-mirror-hy2n.vercel.app)**: mock interviews with a three-person ai panel that actually takes turns, reads your body language in the browser and grades you on evidence from what you said. live, 1,200+ tests, built with [archit](https://github.com/Archit1030).
- **[agentic rag](https://github.com/CodexManvik/Agentic-Rag-for-Distributed-Content)**: langgraph rag that says "not enough evidence" instead of making things up. comes with its own eval harness: 0.69 hit@k, 0.55 mrr, and it blocked every prompt injection in the test set.
- **[deep watermarking](https://github.com/CodexManvik/Deep-Learning-Based-Watermarking)**: hides 256 bits inside an image where you can't see them (37.3 db psnr, 0.97 ssim) and they survive jpeg and noise. trained on 50k images.
- **[floatchat](https://github.com/CodexManvik/FloatChat-AI)**: ask questions about ocean float data in plain english, get sql-backed answers and maps over 88k real measurements. sih 2025 national semi-finalist.

#### right now

- interning at plexuscare
- looking for ai/ml roles, full-time from 2027

#### stack

- **languages:** python · sql · typescript · javascript
- **ml:** pytorch · tensorflow · keras · scikit-learn · numpy · pandas · opencv · mediapipe · hugging face
- **llms:** langgraph · langchain · mcp · llama.cpp · ollama · azure openai · groq · whisper · rag · evals
- **backend & data:** fastapi · flask · websockets · postgres · mysql · redis streams · chromadb · lancedb · pgvector
- **infra:** docker · kubernetes · prometheus · grafana · azure · github actions · vercel · render
- **frontend & desktop:** react · tailwind · tauri · supabase

[portfolio](https://codexmanvik.github.io) · [linkedin](https://linkedin.com/in/manvik-talwar) · [manvik.talwar@gmail.com](mailto:manvik.talwar@gmail.com)
