# Manvik Talwar — building AI systems that hold up outside the notebook

I'm a third-year CS student at Manipal University Jaipur, specializing in AI/ML. Most of my time goes into Generative AI and RAG pipelines — not the toy demos, but the kind that need to handle real data, real latency constraints, and real users. I did my first full production deployment at Path Infotech, which taught me more about what "done" actually means than any course has. I'm still early in the journey, but I'm building things I'm genuinely proud of.

**Currently:** Exploring how retrieval systems can be made more trustworthy — better citations, less hallucination, more honest failure modes. Also thinking about what it takes to make deep learning models hold up under adversarial conditions.

---

### Projects

**Interview Mirror**
Helps people practice interviews by analyzing their body language and stress signals in real time — not just what they say, but how they present. The core challenge was building a low-latency inference pipeline over 543 MediaPipe landmarks that could process a live webcam feed without lag.
`MediaPipe` · `Google Gemini` · `OpenCV` · `Python` · `<100ms latency`

**FloatChat (ARGO)**
A local RAG system I built to query over 100k+ oceanographic science records without sending sensitive data to a cloud API. The interesting problem was making semantic search feel fast over a large specialty corpus where standard chunking strategies fall apart.
`Qwen` · `ChromaDB` · `FAISS` · `FastAPI` · `<2s query time`

**Deep Learning Watermarking**
Invisible copyright protection for digital images using a CNN trained alongside Discrete Wavelet Transform. The real constraint was maintaining perceptual quality (PSNR > 40dB) while achieving 96% robustness against compression — you can't just brute-force one at the expense of the other.
`PyTorch` · `TensorFlow` · `OpenCV` · `DWT` · `NumPy`

**Sofia — Enterprise AI Assistant** *(Path Infotech)*
A RAG chatbot deployed internally at Path Infotech for their internal knowledge base. Built with Azure OpenAI and Cognitive Search, with citation tracking so users could verify where answers came from. Deployed behind a Next.js frontend with a FastAPI backend and MySQL for session state.
`Azure OpenAI` · `Cognitive Search` · `FastAPI` · `Next.js` · `MySQL`

---

### Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)

---

### GitHub Activity

<a href="https://github.com/CodexManvik">
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=CodexManvik&show_icons=true&theme=default&hide_border=true&count_private=true" />
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=CodexManvik&layout=compact&theme=default&hide_border=true" />
</a>

---

If something here looks interesting or you want to talk about RAG systems, watermarking, or anything else — reach me at [manvik.talwar@gmail.com](mailto:manvik.talwar@gmail.com) or on [LinkedIn](https://linkedin.com/in/manvik-talwar). Portfolio at [codexmanvik.github.io](https://codexmanvik.github.io).
