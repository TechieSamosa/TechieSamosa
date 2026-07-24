<div align="center">

<!-- Top Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,30:1a1b26,65:7aa2f7,100:00f5d4&height=170&section=header&text=Hey,%20I'm%20Aditya%20Khamitkar%F0%9F%93%A1&fontSize=42&fontColor=ffffff&fontAlignY=36&animation=fadeIn&desc=Architecting%20the%20Intersection%20of%20Data%2C%20AI%20%26%20Distributed%20Systems&descSize=18&descAlignY=60&descColor=00f5d4" width="100%"/>

```text
 █████╗ ██████╗ ██╗████████╗██╗   ██╗ █████╗ 
██╔══██╗██╔══██╗██║╚══██╔══╝╚██╗ ██╔╝██╔══██╗
███████║██║  ██║██║   ██║    ╚████╔╝ ███████║
██╔══██║██║  ██║██║   ██║     ╚██╔╝  ██╔══██║
██║  ██║██████╔╝██║   ██║      ██║   ██║  ██║
╚═╝  ╚═╝╚═════╝ ╚═╝   ╚═╝      ╚═╝   ╚═╝  ╚═╝
```

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=17&duration=3200&pause=1000&color=7AA2F7&center=true&vCenter=true&width=760&lines=Software+Engineer+%E2%80%94+AI%2C+ML+%26+Distributed+Systems;Currently%3A+building+Atlas%2C+a+C%2B%2B20+distributed+runtime;Previously%3A+ISRO+telemetry+models%2C+RLHF+on+Gemini;Incoming+SDE+Intern+%40+Bosch+GST+(2026)" alt="typing" />

<a href="https://adityakhamitkar.vercel.app"><img src="https://img.shields.io/badge/PORTFOLIO-0d1117?style=for-the-badge&logo=vercel&logoColor=00f5d4"/></a>
<a href="mailto:khamitkaraditya@gmail.com"><img src="https://img.shields.io/badge/EMAIL-0d1117?style=for-the-badge&logo=gmail&logoColor=7AA2F7"/></a>
<a href="https://www.linkedin.com/in/adityakhamitkar/"><img src="https://img.shields.io/badge/LINKEDIN-0d1117?style=for-the-badge&logo=linkedin&logoColor=0A66C2"/></a>
<a href="https://github.com/TechieSamosa"><img src="https://img.shields.io/badge/GITHUB-0d1117?style=for-the-badge&logo=github&logoColor=white"/></a>
<a href="https://kaggle.com/flickeringtubelight"><img src="https://img.shields.io/badge/KAGGLE-0d1117?style=for-the-badge&logo=kaggle&logoColor=20BEFF"/></a>

</div>

---

### ⚡ TL;DR

I build systems — from raw hardware-adjacent execution runtimes to production ML pipelines. Right now, I'm deep in the trenches designing **Atlas**, a high-performance distributed execution engine built from scratch.

> *"I care more about how systems execute under heavy load than hype cycles."*

---

## 🏗️ Spotlight: Atlas Architecture

**Atlas** is an open-source distributed ML and data runtime engineered in **C++20** with high-throughput **Pybind11** zero-copy Python bindings. No wrappers around Ray, Spark, or Celery — every thread pool, memory arena, and DAG execution pipeline is built from first principles.

```text
 ┌─────────────────────────────────────────────────────────────────┐
 │                       Python User API                           │
 │               @atlas.task | DAG Flow Definition                 │
 └────────────────────────────────┬────────────────────────────────┘
                                  │  (Pybind11 Zero-Copy Bridge)
 ┌────────────────────────────────▼────────────────────────────────┐
 │                      C++20 Runtime Engine                       │
 │  ┌─────────────────────────────┐   ┌─────────────────────────┐  │
 │  │    Dynamic DAG Scheduler    │   │ Lock-Free Thread Pools  │  │
 │  └──────────────┬──────────────┘   └────────────┬────────────┘  │
 │                 │                               │               │
 │  ┌──────────────▼──────────────┐   ┌────────────▼────────────┐  │
 │  │ Memory Arenas (Zero-Alloc)  │   │ Multi-Node Transport    │  │
 │  └─────────────────────────────┘   └─────────────────────────┘  │
 └────────────────────────────────┬────────────────────────────────┘
                                  │  (Asynchronous Worker Protocol)
 ┌────────────────────────────────┼────────────────────────────────┐
 │  Worker Node 01 (C++ Execution)│  Worker Node 02 (C++ Execution)│
 └────────────────────────────────┴────────────────────────────────┘
```

#### 🛠️ What's inside right now:

* **Custom Dynamic DAG Execution Engine:** Low-overhead task dependency graph resolution in pure C++20.
* **Lock-Free Concurrency Primitives:** Custom thread pools and ring buffers designed for high-throughput task queuing.
* **Zero-Copy Serialization Boundary:** Seamless bridging between Python objects and C++ contiguous memory buffers.

> 🤝 **Looking for Collaborators & Reviewers!**
> If you like poking holes in scheduler designs, memory allocators, or distributed worker protocols, check out [`TechieSamosa/Atlas`](https://github.com/TechieSamosa/Atlas) — issues, architecture discussions, and PRs are wide open.

---

## 🧭 Career Timeline & Impact

```text
2024 ── 🚀 ISRO (Satish Dhawan Space Centre)
        ├─ Engineered PyTorch/TF LSTM models for launch vehicle telemetry (PSLV/SSLV)
        └─ Cut manual anomaly review time by 40% under real-time signal noise.

2025 ── 🤖 Deccan AI (MAITRIX / Shield / Bluebird)
        ├─ Designed RLHF evaluation rubrics & multi-tool agentic environments for Gemini
        └─ Boosted instruction-following accuracy by +15% across production corpora.

2026 ── 🏭 Bosch Global Software Technologies (Incoming)
        ├─ Incoming Software Engineering Intern — Enterprise Applications
        └─ Focus: Distributed application backends & cloud enterprise systems (Aug 2026 – May 2027)

2026 ── ⚡ Atlas Runtime Engine
        └─ Architecting a distributed C++20 execution runtime in the open.
```

---

## 🧰 Technical Arsenal

**Languages & Core**
<br>
<img src="https://img.shields.io/badge/-Python-7AA2F7?style=flat-square&logo=python&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-Modern%20C++20-00f5d4?style=flat-square&logo=cplusplus&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-SQL-F7C548?style=flat-square&logo=postgresql&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-Bash-9ECE6A?style=flat-square&logo=gnubash&logoColor=0d1117" />

**Machine Learning & GenAI**
<br>
<img src="https://img.shields.io/badge/-PyTorch-E63980?style=flat-square&logo=pytorch&logoColor=white" />
<img src="https://img.shields.io/badge/-TensorFlow-FF6B35?style=flat-square&logo=tensorflow&logoColor=white" />
<img src="https://img.shields.io/badge/-scikit--learn-7AA2F7?style=flat-square&logo=scikitlearn&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-XGBoost-00f5d4?style=flat-square&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-RLHF%20%26%20LLM%20Eval-BB9AF7?style=flat-square&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-LangChain%2FLangGraph-9ECE6A?style=flat-square&logo=langchain&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-HuggingFace-F7C548?style=flat-square&logo=huggingface&logoColor=0d1117" />

**Data Science & Engineering**
<br>
<img src="https://img.shields.io/badge/-Pandas%2FNumPy%2FSciPy-7AA2F7?style=flat-square&logo=pandas&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-Apache%20Spark-E63980?style=flat-square&logo=apachespark&logoColor=white" />
<img src="https://img.shields.io/badge/-PySpark-FF6B35?style=flat-square&logo=apachespark&logoColor=white" />
<img src="https://img.shields.io/badge/-ETL-00f5d4?style=flat-square&logoColor=0d1117" />

**Systems & Backend**
<br>
<img src="https://img.shields.io/badge/-Pybind11-BB9AF7?style=flat-square&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-gRPC-9ECE6A?style=flat-square&logo=googlecloud&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-Distributed%20Systems-F7C548?style=flat-square&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-FastAPI-7AA2F7?style=flat-square&logo=fastapi&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-REST%20APIs-E63980?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/-SQLite-00f5d4?style=flat-square&logo=sqlite&logoColor=0d1117" />

**Cloud, DevOps & Tools**
<br>
<img src="https://img.shields.io/badge/-AWS-FF6B35?style=flat-square&logo=amazonaws&logoColor=white" />
<img src="https://img.shields.io/badge/-Docker-7AA2F7?style=flat-square&logo=docker&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-Kubernetes-BB9AF7?style=flat-square&logo=kubernetes&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-Git-9ECE6A?style=flat-square&logo=git&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-Linux-F7C548?style=flat-square&logo=linux&logoColor=0d1117" />
<img src="https://img.shields.io/badge/-Streamlit-00f5d4?style=flat-square&logo=streamlit&logoColor=0d1117" />

---

## 🗂️ Engineering Works

| Project | Description | Key Tech Stack |
| --- | --- | --- |
| ⚡ **Atlas** | Open-source distributed runtime engine with dynamic DAG execution and worker communication. | `C++20` `Pybind11` `gRPC` `Python` |
| 🦷 **DentalOS** | Modular, offline-first desktop app for clinical management engineered for zero-latency operations. | `Python` `PySide6` `SQLite` |
| ⚙️ **Synapse.cpp** | Bare-metal neural network engine built from scratch (forward/backward prop, Adam, Dropout, gradient clipping). | `C++17` `RAII` `Zero-Deps` |
| 🌕 **Project AETHER** | GAN + Self-Supervised Masked Autoencoder to enhance lunar PSR imagery with **+86 dB SNR** improvement. | `PyTorch` `GDAL` `Rasterio` |
| 🌾 **AgriSat AI** | Satellite crop-health classification engine running soft-voting ensembles with **92%+ accuracy**. | `PySpark` `AWS S3` `Scikit-Learn` |

---

## 📊 Activity & Telemetry

<div align="center">

<img src="https://github-stats-extended.vercel.app/api?username=TechieSamosa&show_icons=true&theme=tokyonight&hide_border=true&hide_rank=true&include_all_commits=true" height="165"/>
<img src="https://github-stats-extended.vercel.app/api/top-langs/?username=TechieSamosa&layout=compact&theme=tokyonight&hide_border=true" height="165"/>

<img src="https://streak-stats.demolab.com/?user=TechieSamosa&theme=tokyonight&hide_border=true&background=0D1117&ring=7AA2F7&fire=00F5D4&currStreakLabel=BB9AF7" width="90%"/>

</div>

---

## 🎓 Recognition & Background

* **M.Tech CSE** *(Computational & Data Science)* — **VIT Bhopal University** (2027 Batch)
* **Intel AI4Youth National Finalist** *(Top 125 out of 52,000+ national entries)*
* **Smart India Hackathon (SIH) National Finalist** *(2024)*

---

### 💡 Let's Build Something Serious

Whether it's distributed runtimes, agentic RL, or low-level systems optimizations, I'm always open to technical discussions and collaboration.

<div align="center">

<a href="mailto:khamitkaraditya@gmail.com"><img src="https://img.shields.io/badge/open%20to%20SDE%20%2F%20AI%20infra%20roles-00f5d4?style=for-the-badge&labelColor=0d1117"/></a>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00f5d4,65:7aa2f7,100:0d1117&height=110&section=footer"/>
