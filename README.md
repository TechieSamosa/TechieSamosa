<!-- ═══════════════════════════  HEADER  ═══════════════════════════ -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,40:1a1b26,75:7aa2f7,100:00f5d4&height=200&section=header&text=Aditya%20Khamitkar&fontSize=56&fontColor=ffffff&fontAlignY=38&animation=fadeIn&desc=Data%20%C2%B7%20AI%20%C2%B7%20Distributed%20Systems&descSize=18&descAlignY=60&descColor=c0caf5" width="100%"/>

<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=3000&pause=900&color=00F5D4&center=true&vCenter=true&width=640&lines=Software+Engineer+%E2%80%94+AI%2C+ML+%26+Distributed+Systems;Building+Atlas%3A+a+C%2B%2B20+distributed+runtime;SDE+Intern+%40+Bosch+Global+Software+Technologies;Ex-ISRO+telemetry+ML+%C2%B7+RLHF+on+Gemini" alt="Typing SVG" /></a>

<br/>

<a href="https://adityakhamitkar.vercel.app"><img src="https://img.shields.io/badge/Portfolio-1a1b26?style=for-the-badge&logo=vercel&logoColor=00f5d4"/></a>
<a href="https://www.linkedin.com/in/adityakhamitkar/"><img src="https://img.shields.io/badge/LinkedIn-1a1b26?style=for-the-badge&logo=linkedin&logoColor=7aa2f7"/></a>
<a href="mailto:khamitkaraditya@gmail.com"><img src="https://img.shields.io/badge/Email-1a1b26?style=for-the-badge&logo=gmail&logoColor=f7768e"/></a>
<a href="https://kaggle.com/flickeringtubelight"><img src="https://img.shields.io/badge/Kaggle-1a1b26?style=for-the-badge&logo=kaggle&logoColor=20BEFF"/></a>
<img src="https://komarev.com/ghpvc/?username=TechieSamosa&style=for-the-badge&color=1a1b26&label=PROFILE+VIEWS" />

</div>

<br/>

## 👋 About me

<img align="right" width="380" src="https://github-stats-extended.vercel.app/api?username=TechieSamosa&show_icons=true&theme=tokyonight&hide_border=true&hide_rank=true&include_all_commits=true&bg_color=0d1117" />

I build systems end to end, from low-level execution runtimes to production ML pipelines. Right now I'm designing **Atlas**, a distributed execution engine written from scratch in C++20.

- 🏭 **Now:** SDE Intern at **Bosch Global Software Technologies** (Enterprise Applications)
- ⚡ **Building:** [Atlas](https://github.com/TechieSamosa/Atlas), a C++20 DAG runtime with zero-copy Python bindings
- 🎓 **Studying:** M.Tech CSE (Computational & Data Science), VIT Bhopal, class of 2027
- 💬 **Ask me about:** schedulers, memory allocators, LLM evaluation, time-series ML
- 📫 **Reach me:** [khamitkaraditya@gmail.com](mailto:khamitkaraditya@gmail.com)

> *"I care more about how systems behave under heavy load than about hype cycles."*

<br clear="right"/>

---

## ⚡ Spotlight: Atlas

**Atlas** is an open-source distributed ML and data runtime written in **C++20**, with **pybind11** zero-copy bindings to Python. It doesn't wrap Ray, Spark or Celery: the thread pools, memory arenas and DAG executor are all built from first principles.

```text
╭───────────────────────────────────────────────────────────────╮
│                                                               │
│                        Python User API                        │
│              @atlas.task  ·  DAG flow definition              │
│                                                               │
╰───────────────────────────────┬───────────────────────────────╯
                                │  pybind11 · zero-copy bridge
╭───────────────────────────────▼───────────────────────────────╮
│                      C++20 Runtime Engine                     │
│                                                               │
│ ┌───────────────────────────┐   ┌───────────────────────────┐ │
│ │   Dynamic DAG Scheduler   │   │   Lock-free Thread Pools  │ │
│ └─────────────┬─────────────┘   └─────────────┬─────────────┘ │
│               │                               │               │
│ ┌─────────────▼─────────────┐   ┌─────────────▼─────────────┐ │
│ │ Memory Arenas (zero-alloc)│   │    Multi-node Transport   │ │
│ └───────────────────────────┘   └───────────────────────────┘ │
╰───────────────────────────────┬───────────────────────────────╯
                                │  async worker protocol
╭───────────────────────────────┴───────────────────────────────╮
│      Worker 01 · C++ exec     │      Worker 02 · C++ exec     │
╰───────────────────────────────┴───────────────────────────────╯
```

<table>
<tr>
<td width="33%" valign="top">

**🧠 Dynamic DAG engine**<br/>
<sub>Low-overhead task dependency resolution in pure C++20.</sub>

</td>
<td width="33%" valign="top">

**🔓 Lock-free concurrency**<br/>
<sub>Custom thread pools and ring buffers for high-throughput task queuing.</sub>

</td>
<td width="33%" valign="top">

**📦 Zero-copy boundary**<br/>
<sub>Python objects map straight onto contiguous C++ buffers.</sub>

</td>
</tr>
</table>

> [!TIP]
> **Looking for collaborators and reviewers.** If you enjoy poking holes in scheduler designs, allocators or worker protocols, come break things in [`TechieSamosa/Atlas`](https://github.com/TechieSamosa/Atlas). Issues, design discussions and PRs are all open.

---

## 🧭 Journey

| When | Where | What I did |
|:---:|:---|:---|
| **2024** | 🚀 **ISRO** · Satish Dhawan Space Centre | Built PyTorch/TensorFlow LSTM models for PSLV/SSLV launch-vehicle telemetry; cut manual anomaly review time by **40%** under real-time signal noise. |
| **2025** | 🤖 **Deccan AI** · MAITRIX / Shield / Bluebird | Designed RLHF evaluation rubrics and multi-tool agentic environments for Gemini; lifted instruction-following accuracy by **+15%** across production corpora. |
| **2026 →** | 🏭 **Bosch Global Software Technologies** | SDE Intern, Enterprise Applications (Aug 2026 – May 2027): distributed backends and cloud enterprise systems. |
| **2026 →** | ⚡ **Atlas** | Designing a distributed C++20 execution runtime in the open. |

---

## 🧰 Tech stack

<div align="center">

<img src="https://skillicons.dev/icons?i=py,cpp,postgres,bash,pytorch,tensorflow,sklearn&theme=dark&perline=7" />
<br/><br/>
<img src="https://skillicons.dev/icons?i=fastapi,sqlite,aws,docker,kubernetes,linux,git&theme=dark&perline=7" />

<br/><br/>

<img src="https://img.shields.io/badge/Apache%20Spark-1a1b26?style=flat-square&logo=apachespark&logoColor=E25A1C" />
<img src="https://img.shields.io/badge/PySpark-1a1b26?style=flat-square&logo=apachespark&logoColor=E25A1C" />
<img src="https://img.shields.io/badge/HuggingFace-1a1b26?style=flat-square&logo=huggingface&logoColor=FFD21E" />
<img src="https://img.shields.io/badge/LangChain%20%2F%20LangGraph-1a1b26?style=flat-square&logo=langchain&logoColor=9ece6a" />
<img src="https://img.shields.io/badge/XGBoost-1a1b26?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/pybind11-1a1b26?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/gRPC-1a1b26?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/Streamlit-1a1b26?style=flat-square&logo=streamlit&logoColor=FF4B4B" />
<img src="https://img.shields.io/badge/RLHF%20%26%20LLM%20Eval-1a1b26?style=flat-square&logoColor=white" />

</div>

---

## 🗂️ Selected work

| | Project | What it is | Stack |
|:---:|:---|:---|:---|
| ⚡ | **[Atlas](https://github.com/TechieSamosa/Atlas)** | Distributed runtime with dynamic DAG execution and a custom worker protocol | `C++20` `pybind11` `gRPC` |
| ⚙️ | **Synapse.cpp** | Neural network engine from scratch: backprop, Adam, dropout, gradient clipping, zero dependencies | `C++17` `RAII` |
| 🌕 | **Project AETHER** | GAN + self-supervised masked autoencoder that enhances lunar PSR imagery (**+86 dB SNR**) | `PyTorch` `GDAL` `Rasterio` |
| 🌾 | **AgriSat AI** | Satellite crop-health classifier using soft-voting ensembles (**92%+ accuracy**) | `PySpark` `AWS S3` `scikit-learn` |
| 🦷 | **DentalOS** | Modular, offline-first desktop app for clinic management | `Python` `PySide6` `SQLite` |

---

## 📊 GitHub activity

<div align="center">

<img height="170" src="https://github-stats-extended.vercel.app/api/top-langs/?username=TechieSamosa&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&langs_count=8" />
<img height="170" src="https://streak-stats.demolab.com/?user=TechieSamosa&theme=tokyonight&hide_border=true&background=0D1117&ring=7AA2F7&fire=00F5D4&currStreakLabel=BB9AF7" />

<img width="100%" src="https://github-readme-activity-graph.vercel.app/graph?username=TechieSamosa&theme=tokyo-night&hide_border=true&bg_color=0d1117&color=7aa2f7&line=00f5d4&point=bb9af7&area=true&area_color=00f5d4" />

</div>

---

## 🏆 Recognition

- 🥇 **Intel AI4Youth National Finalist**: top 125 of 52,000+ entries
- 🇮🇳 **Smart India Hackathon National Finalist** (2024)
- **Flipkart Grid Semi-Finalist** (2026)

---

<div align="center">

### 💡 Let's build something serious

Distributed runtimes, agentic RL or low-level performance work: I'm always up for a deep technical conversation.

<a href="mailto:khamitkaraditya@gmail.com"><img src="https://img.shields.io/badge/Open%20to-SDE%20%2F%20AI%20Infra%20roles-00f5d4?style=for-the-badge&labelColor=1a1b26"/></a>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00f5d4,35:7aa2f7,100:0d1117&height=120&section=footer" width="100%"/>
