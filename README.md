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
> If you like poking holes in scheduler designs, memory allocators, or distributed worker protocols, check out [`TechieSamosa/Atlas`](https://www.google.com/search?q=https://github.com/TechieSamosa) — issues, architecture discussions, and PRs are wide open.

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

---

## 🎓 Recognition & Background

* **M.Tech CSE** *(Computational & Data Science)* — **VIT Bhopal University** (2027 Batch)
* **Intel AI4Youth National Finalist** *(Top 125 out of 52,000+ national entries)*
* **Smart India Hackathon (SIH) National Finalist** *(2024)*

### 💡 Let's Build Something Serious

Whether it's distributed runtimes, agentic RL, or low-level systems optimizations, I'm always open to technical discussions and collaboration.
