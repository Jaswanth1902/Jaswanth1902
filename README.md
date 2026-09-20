# Hey, I'm Jaswanth 👋

I build lightweight tools for Windows, AI coding workflows, and low-level runtimes in C++ and Python. Most of what I make starts because an existing tool was too slow, ate too much memory, or cost $50/month for simple API calls.

[Email](mailto:jaswanthreddy1537@gmail.com) • [LinkedIn](https://www.linkedin.com/in/kannali-sai-jaswanth-reddy-aa3678337/) • [GitHub](https://github.com/Jaswanth1902)

---

## Featured Projects

### 🏝️ [Notch](https://github.com/Jaswanth1902/Notch) — Windows 11 Dynamic Island & Ambient HUD
*A bezel-flush status HUD that doesn't steal focus.*
- **Why**: Background Electron widgets eat 200MB+ of RAM just to display a few status badges.
- **How**: Built in native C#, WPF, and PowerShell with global hotkeys (`Shift+Enter`) to confirm background tasks without task switching.
- **Footprint**: **0.0% idle CPU**, `<25MB RAM`.
- **Stack**: C#, Win32, WPF, PowerShell • `Apache 2.0`

### 🗺️ [Cartograph](https://github.com/Jaswanth1902/Omnia-codebase-memory) — Fast AST Codebase Mapmaker & MCP Server
*Give coding agents an instant structural map instead of grepping thousands of lines.*
- **Why**: AI coding assistants burn through context windows and generate hallucinated imports when reading raw files blindly.
- **How**: An MCP server that parses code into deterministic AST symbol graphs with SQLite WAL caching.
- **Benchmark**: **<10ms** symbol lookup, cuts agent context token burn by **>90%**.
- **Stack**: Python 3.10+, AST, MCP Protocol, SQLite • `Apache 2.0`

### ⚡ [DWEL](https://github.com/Jaswanth1902/dwel) — Loop Detector for AI Coding Agents
*Catch non-progressing agent loops before they drain API credits.*
- **Why**: Autonomous agents often get trapped in retry cycles, repeating failing tool calls until context runs out.
- **How**: Hashes actions and models execution history as a directed graph to detect back-edges and cycles in real time.
- **Benchmark**: **<1ms** cycle fingerprinting, saves up to **42%** of token budgets.
- **Stack**: Python 3.10+, DAG Trajectory Engine • `Apache 2.0`

### 🔒 [mem-shred](https://github.com/Jaswanth1902/mem-shred) — Compiler-Safe RAM Zeroization
*Wipe sensitive keys and credentials from memory without compilers optimizing the wipe away.*
- **Why**: Standard `free()`, `delete`, or `memset()` calls are frequently stripped by modern compilers via Dead Store Elimination.
- **How**: Header-only C++20 library and Python module enforcing hardware memory barriers and 3-pass DoD 5220.22-M overwrites.
- **Benchmark**: **0.08 µs** cache-line purge, zero forensic plaintext leakage.
- **Stack**: C++20 Header-Only, Python ctypes • `Apache 2.0`

### ⚡ [InstaFlow](https://github.com/Jaswanth1902/InstaFlow) — Local-First Instagram DM Automation
*Send links and automate DM leads without third-party SaaS subscriptions.*
- **Why**: Tools like ManyChat cost $50+/month and require full cloud access tokens just to send automated links.
- **How**: Zero-dependency Python CLI and direct API agent with sub-16ms dispatch and an interactive terminal simulator.
- **Benchmark**: **<16ms** message dispatch, `<25MB RAM`, $0 SaaS fees.
- **Stack**: Python 3.10+, Direct Web API • `Apache 2.0`

### 🧠 [Profiler](https://github.com/Jaswanth1902/Profiler) — Focus & Session Intent Engine
*Prime AI coding agents with your actual working context instead of starting from scratch.*
- **Why**: Task lists fall out of date within 48 hours, and coding agents have zero idea what you were just working on or what broke.
- **How**: Merges active window pulses with recent session log mining to produce an instant context brief.
- **Benchmark**: **<0.5ms** pulse merge, streams session logs in **<12ms**, emits a **<80 token** agent prompt prime.
- **Stack**: Python stdlib, Win32 ctypes • `Apache 2.0`

---

## At a Glance

| Project | What It Solves | Key Number | Tech |
| :--- | :--- | :--- | :--- |
| [Notch](https://github.com/Jaswanth1902/Notch) | Ambient HUD without focus stealing | 0.0% idle CPU • <25MB RAM | C#, WPF, Win32 |
| [Cartograph](https://github.com/Jaswanth1902/Omnia-codebase-memory) | Instant AST codebase symbol indexer | <10ms lookup • >90% token cut | Python, AST, MCP |
| [DWEL](https://github.com/Jaswanth1902/dwel) | Traps infinite agent execution loops | <1ms check • 42% token cut | Python, Graph Trajectory |
| [mem-shred](https://github.com/Jaswanth1902/mem-shred) | Compiler-safe RAM credential wipe | 0.08 µs purge • 0 leakage | C++20, ctypes |
| [InstaFlow](https://github.com/Jaswanth1902/InstaFlow) | Local-first Instagram DM lead runner | <16ms dispatch • $0 SaaS fees | Python, Direct API |
| [Profiler](https://github.com/Jaswanth1902/Profiler) | Derives context prime from session logs | <80 tokens • <0.5ms merge | Python, Win32 |

---

## Other Projects

| Project | Description | Stack |
| :--- | :--- | :--- |
| [Academic-ideation-platform](https://github.com/Jaswanth1902/-Academic-ideation-platform) | Research citation graph explorer powered by local Ollama models | React, Vite, Python, Ollama |
| [Autism_Screening_Agent](https://github.com/Jaswanth1902/Autism_Screening_Agent) | Clinical screening questionnaire with SHAP explainability trees | Streamlit, Gemini API, ReportLab |
| [DAA_EL](https://github.com/Jaswanth1902/DAA_EL) | In-browser Delaunay image triangulation with 3D OBJ export | Vanilla JS, Web Workers, Canvas |
| [Hospital-Database](https://github.com/Jaswanth1902/Hospital-Database) | 3NF relational clinical schema with ACID transaction isolation | PostgreSQL, Node.js, Express |
| [Queue-Drop](https://github.com/Jaswanth1902/Queue-Drop) | Token-bucket rate limiter with dead-letter queue isolation | Python, AsyncIO |
| [Z_Forge](https://github.com/Jaswanth1902/Z_Forge) | Dual C99 and Python LZW compression algorithm profiler | C99, Python, ctypes |

---

## Engineering Rules of Thumb

- **Standard library first**: Zero third-party dependencies when language primitives do the job.
- **Low memory ceilings**: Keep background processes under 25MB RAM.
- **Local and private**: No sending local context or credentials to unnecessary cloud backends.
- **Real benchmarks over marketing**: Measure latencies in microseconds and milliseconds, not vague adjectives.

---

## Getting in Touch

- **Email**: [jaswanthreddy1537@gmail.com](mailto:jaswanthreddy1537@gmail.com)
- **LinkedIn**: [linkedin.com/in/kannali-sai-jaswanth-reddy-aa3678337](https://www.linkedin.com/in/kannali-sai-jaswanth-reddy-aa3678337/)
- **GitHub**: [github.com/Jaswanth1902](https://github.com/Jaswanth1902)
