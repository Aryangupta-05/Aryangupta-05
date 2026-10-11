<div align="center">

# 👨‍💻 Aryan Gupta
### **Software Engineer · Backend & Distributed Systems · Applied AI & Full-Stack**

[![Portfolio](https://img.shields.io/badge/Portfolio-aryanportfolio--theta.vercel.app-6366F1?style=for-the-badge&logo=vercel&logoColor=white)](https://aryanportfolio-theta.vercel.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-aryan--gupta-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aryan-gupta-871577240/)
[![LeetCode](https://img.shields.io/badge/LeetCode-Knight%20(1943)-FFA116?style=for-the-badge&logo=leetcode&logoColor=white)](https://leetcode.com/u/aryangupta_/)
[![CodeChef](https://img.shields.io/badge/CodeChef-3★%20(1639)-5B4638?style=for-the-badge&logo=codechef&logoColor=white)](https://www.codechef.com/users/itss_levi)
[![Codeforces](https://img.shields.io/badge/Codeforces-Pupil%20(1246)-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white)](https://codeforces.com/profile/aryangupta_)
[![Email](https://img.shields.io/badge/Email-aryangupta050903%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:aryangupta050903@gmail.com)

<p align="center">
  🎓 <b>Birla Institute of Technology (BIT), Mesra</b> · B.Tech in Electronics and Communication Engineering (2023 – 2027) · <b>CGPA: 8.49 / 10</b><br/>
  💼 Software Developer Intern at <b>QOE Technologies and Services</b> (Soul Consciousness Lab)<br/>
  🎯 Actively seeking <b>Software Engineering (SDE), Backend, Full-Stack, and AI/ML Internship Opportunities</b>
</p>

---

</div>

## 📌 About Me

I am a software engineer focused on building **high-throughput backend architectures**, **applied GenAI / RAG pipelines**, and **low-latency network systems**. My engineering approach emphasizes robust API design, caching layers, database indexing, and writing clean, scalable code. 

- 🏎️ **Backend & Systems**: Deep experience with **FastAPI, Node.js/Express, C++17, PostgreSQL, Redis, and MongoDB**, designing RESTful APIs and multithreaded network engines.
- 🤖 **Applied AI & RAG**: Built production-grade Retrieval-Augmented Generation workflows with **LangChain, SentenceTransformers, and FAISS**, leveraging Redis caching to drop inference query latency from **2.5s to under 15ms**.
- 💡 **Algorithmic Problem Solving**: **750+ DSA problems solved**, **Knight on LeetCode (Rating 1943, Top 3.5%)**, **3-Star on CodeChef (Max Rating 1639)**, and **Pupil on Codeforces (1246)**, with contest finishes in the **Global Top 285** on LeetCode and **Round 2 Qualifier** in **Google The Big Code 2026**.

---

## 🏆 Competitive Programming & Achievements

<div align="center">

| Platform | Achievement / Max Rating | Global Standing / Highlights |
|:---|:---|:---|
| **LeetCode** | **Knight** (Max Rating **1943**) | **Top 3.5%** globally · **Global Rank 285** (Weekly Contest 502) · **Global Rank 1,488** (Biweekly 184) |
| **CodeChef** | **3-Star** (Max Rating **1639**) | Handle: [`itss_levi`](https://www.codechef.com/users/itss_levi) |
| **Codeforces** | **Pupil** (Rating **1246**) | Handle: [`aryangupta_`](https://codeforces.com/profile/aryangupta_) |
| **Google The Big Code** | **Round 2 Qualifier (2026)** | **Top 1,500** nationwide qualifier |
| **Problem Solving** | **750+ Problems Solved** | Strong foundations in Trees, Graphs, DP, Sorting/Searching, Flow Networks |
| **JEE Main 2023** | **Top 3% Nationwide** | Out of 1.2+ Million Candidates |
| **Leadership** | **Captain, BIT Mesra Football Team** | (2025 – Present) Leading squad strategy, fitness, and team coordination |

<br/>

<a href="https://leetcode.com/u/aryangupta_/">
  <img src="https://leetcard.jacoblin.cool/aryangupta_?theme=dark&font=baloo" alt="Aryan Gupta LeetCode Stats" height="190" />
</a>
<a href="https://github.com/Aryangupta-05">
  <img src="https://github-readme-stats.vercel.app/api?username=Aryangupta-05&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true" alt="Aryan Gupta GitHub Stats" height="190" />
</a>

</div>

---

## 🚀 Featured Engineering Projects

### 1. [DocuMind — End-to-End RAG Document Assistant](https://github.com/Aryangupta-05/document-qa-rag-Documind)
> **AI / RAG · FastAPI · PostgreSQL · Redis · FAISS · LangChain · React · Docker**  
> 🔗 **[GitHub Repository](https://github.com/Aryangupta-05/document-qa-rag-Documind)** · 🎥 **[Video Demo Walkthrough](https://drive.google.com/file/d/1PqMBUXxCzTodIP-RXzxcH-pqV_ddzhz_/view?usp=sharing)**

- **End-to-End RAG Pipeline**: Ingests multi-format documents (PDF, DOCX, TXT) with LangChain recursive chunking, generates embeddings with HuggingFace `SentenceTransformers`, and performs top-$k$ semantic retrieval using an in-memory `FAISS` vector store.
- **FastAPI REST Backend**: Built with Pydantic validation, SQLAlchemy ORM, and PostgreSQL for document metadata, query logs, and analytics.
- **Multi-Turn Conversational Q&A**: Maintains session-aware conversation context, streams responses to the React UI in real-time, and asynchronously triggers 3 smart follow-up suggestions per answer.
- **High-Performance Caching**: Integrated **Redis query caching (1-hour TTL)** and rate limiting, drastically dropping repeated query latency from **2.5s down to under 15ms** (~99.4% latency reduction). Fully containerized with Docker & Docker Compose.

```
[User Document (PDF/DOCX/TXT)] ──► [LangChain Chunker] ──► [SentenceTransformers] ──► [FAISS Vector Index]
                                                                                              │ Top-k Chunks
[User Query] ──► [Redis Cache Check] ──(Miss)──► [FastAPI Backend] ──► [LLM + Context] ───────┘
                     │ (Hit: <15ms)                                      │
                     └──────────────────── Streamed Response ────────────┴──► [React UI + Follow-Ups]
```

---

### 2. [DPI Engine — Deep Packet Inspection & Network Firewall](https://github.com/Aryangupta-05/Packet_Analyser)
> **C++17 · PCAP Parsing · Multithreading · TLS SNI · 5-Tuple Flow Tracking · CMake**  
> 🔗 **[GitHub Repository](https://github.com/Aryangupta-05/Packet_Analyser)**

- **High-Throughput C++17 Core**: Co-engineered an offline Deep Packet Inspection engine from scratch with zero heavy external dependencies, featuring a custom PCAP reader and Ethernet, IPv4, TCP, UDP, and ICMP header parsers.
- **Multithreaded Architecture**: Utilized thread-safe queues and producer-consumer pipelines capable of processing **10,000+ packets/sec on a single CPU core**.
- **Traffic Classification**: Extracts Server Name Indication (SNI) from TLS 1.2/1.3 Client Hello packets, decodes HTTP Host headers, and resolves DNS queries to accurately identify web and application protocols.
- **5-Tuple Flow Tracking & Filtering**: Built a bidirectional stateful flow tracker (`src_ip`, `dst_ip`, `src_port`, `dst_port`, `protocol`) with a rule engine that filters traffic by IP, wildcard domains, applications, and ports, exporting filtered PCAP captures and HTML audit dashboards.

```
[.pcap Capture] ──► [PCAP Reader] ──► [Ethernet / IPv4 / TCP / UDP / ICMP Parsers]
                                                        │
                                            [Thread-Safe Queue]
                                                        │
                      ┌─────────────────────────────────┴─────────────────────────────────┐
                      ▼                                                                   ▼
       [TLS SNI / HTTP Host / DNS Classifier]                              [5-Tuple Stateful Flow Tracker]
                      │                                                                   │
                      └───────────────────────────────┬───────────────────────────────────┘
                                                      ▼
                                           [DPI Rule Engine]
                                   (Block by IP / Domain / App / Port)
                                                      │
                            ┌─────────────────────────┴─────────────────────────┐
                            ▼                                                   ▼
                [Filtered .pcap File]                              [JSON / CSV / HTML Dashboard]
```

---

### 3. [Tweetie — Full-Stack Scalable Social Media Platform](https://github.com/Aryangupta-05/Tweetie)
> **React.js · Node.js · Express.js · MongoDB · JWT · AWS S3 · AWS EC2 · PM2 · TanStack Query**  
> 🔗 **[GitHub Repository](https://github.com/Aryangupta-05/Tweetie)** · 🌐 **[Live Demo](https://tweetie-five.vercel.app/login)**

- **Full-Stack MERN Architecture**: Engineered a responsive social platform featuring user authentication, post creation, comments, likes, following relationships, and user profile management.
- **Stateless JWT Security**: Implemented JWT authentication stored in HTTP-only cookies to eliminate XSS-based token theft vulnerabilities.
- **Algorithmic Feed Personalization**: Implemented a custom HackerNews-inspired time-decay scoring formula:
  $$\text{Score} = \frac{(\text{Likes} \times 1) + (\text{Comments} \times 5)}{(\text{AgeInHours} + 2)^{1.5}}$$
- **$O(1)$ Read Latency via Cron Worker**: Deployed an asynchronous `node-cron` background job that periodically precomputes trending scores in MongoDB, ensuring lightning-fast feed retrieval regardless of post volume.
- **Cloud Infrastructure**: Integrated **AWS S3** for scalable media storage, TanStack React Query for intelligent client-side caching, and deployed the production backend on an **AWS EC2 (Ubuntu)** instance with **PM2** for process clustering and zero downtime.

---

### 4. [Listing Website — Full-Stack Rental Platform](https://github.com/Aryangupta-05/Listing-wesbite)
> **Node.js · Express.js · MongoDB · EJS · Cloudinary · Render**  
> 🔗 **[GitHub Repository](https://github.com/Aryangupta-05/Listing-wesbite)** · 🌐 **[Live Demo](https://listing-website-modc.onrender.com/)**

- Full-stack accommodation booking and rental listing application built with Node.js, Express, MongoDB, and EJS templating.
- Includes user registration, authentication, full CRUD listing management, review & rating systems, and Cloudinary media upload integration.

---

## 💼 Work Experience

### 🏢 Software Developer Intern · **QOE Technologies and Services**
*May 2026 – June 2026 · Remote*
- Engineered core full-stack features for **Soul Consciousness Lab** using React.js, Node.js, Express.js, and MongoDB.
- Built production-ready RESTful APIs with strict request validation, structured error handling, and robust CRUD capabilities.
- Profiled frontend components to eliminate redundant API invocations, minimize unnecessary React re-renders, and implemented code-splitting with lazy loading to significantly boost page load speeds.

---

## 🛠️ Technical Skills

<div align="center">

| Domain | Technologies & Frameworks |
|:---|:---|
| **Programming Languages** | `C++ (C++17)`, `Python`, `JavaScript (ES6+)`, `SQL` |
| **Backend & APIs** | `Node.js`, `Express.js`, `FastAPI`, `RESTful APIs`, `JWT Authentication`, `SQLAlchemy`, `Mongoose` |
| **Databases & Caching** | `PostgreSQL`, `MongoDB`, `MySQL`, `Redis (Caching & Rate Limiting)` |
| **AI, ML & Vector Search** | `Generative AI`, `LLMs`, `RAG Pipelines`, `LangChain`, `SentenceTransformers`, `FAISS`, `Vector Search` |
| **Frontend Development** | `React.js`, `Vite`, `Tailwind CSS`, `TanStack Query (React Query)`, `Zustand`, `EJS` |
| **Cloud & DevOps** | `AWS (EC2, S3)`, `Docker`, `Docker Compose`, `GitHub Actions (CI/CD)`, `PM2`, `Vercel`, `Render` |
| **Developer Tools** | `Git`, `GitHub`, `Linux (Bash)`, `Postman`, `CMake`, `CTest` |
| **Core Computer Science** | `Data Structures & Algorithms`, `Object-Oriented Programming (OOP)`, `Operating Systems`, `DBMS`, `Computer Networks`, `System Design` |

</div>

---

## 📬 Let's Connect

I am actively looking for **Software Engineering (SDE), Backend, Full-Stack, and AI/ML internship roles**. If you have an opening or would like to discuss engineering and collaboration, please reach out!

<div align="center">

[![Email](https://img.shields.io/badge/Email-aryangupta050903%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:aryangupta050903@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-aryan--gupta-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aryan-gupta-871577240/)
[![Portfolio](https://img.shields.io/badge/Portfolio-aryanportfolio--theta.vercel.app-6366F1?style=for-the-badge&logo=vercel&logoColor=white)](https://aryanportfolio-theta.vercel.app)
[![LeetCode](https://img.shields.io/badge/LeetCode-aryangupta__-FFA116?style=for-the-badge&logo=leetcode&logoColor=white)](https://leetcode.com/u/aryangupta_/)
[![CodeChef](https://img.shields.io/badge/CodeChef-itss__levi-5B4638?style=for-the-badge&logo=codechef&logoColor=white)](https://www.codechef.com/users/itss_levi)
[![Codeforces](https://img.shields.io/badge/Codeforces-aryangupta__-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white)](https://codeforces.com/profile/aryangupta_)

</div>
