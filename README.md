<!--
  ────────────────────────────────────────────────────────────────
  BEFORE PUBLISHING — fill in or delete every FILL-IN marker below.
  Anything still marked FILL-IN is a claim I have not yet verified.
  Ship with the claim removed rather than with the claim unbacked.
  ────────────────────────────────────────────────────────────────
-->

# Hi, I'm Anirudh Moholkar 👋

**Computer Engineering @ UIUC** | James Scholar | Dean's List | Fiddler Innovation Awardee
**SWE Intern @ Zebra Technologies** — *Distributed Systems • Systems Programming • Agentic AI • Scalable Infrastructure*

---

I'm a senior at the **University of Illinois Urbana-Champaign** who builds fault-tolerant systems and, more recently, agentic AI systems that have to actually be measured rather than demoed. My background spans kernel and RISC architecture work, distributed file systems and stream processing built from scratch, and production LLM tooling in an enterprise environment.

- 🔭 **Currently:** building retrieval and evaluation tooling for code-aware LLM systems
- ⚡ **Focus:** distributed systems, evaluation-driven AI engineering, Go / C++ / Python
- 🛠️ **Experience:** SWE Intern @ **Zebra Technologies** — Cloud & Computing, then AI & Data Engineering
- 🏛️ **Leadership:** Director of Operations, **Design for America** (UIUC Chapter)
- 🎓 **Graduating** May 2027 — seeking full-time SWE roles

---

## Technical Stack

[![My Skills](https://skillicons.dev/icons?i=cpp,c,python,java,go,postgres,docker,linux,git,githubactions,spring)](https://skillicons.dev)

**Languages:** C, C++, Python, Java, Go, SystemVerilog, SQL
**Systems:** Distributed systems, OS/kernel development, RISC architecture, concurrency, memory management
**Infrastructure:** Docker, GitHub Actions, gRPC, REST, Spring Boot, Linux/Unix
**AI Systems:** RAG architecture, agentic workflows (ReAct/reflection), vector search (FAISS, Pinecone), LLM evaluation and observability

---

## Professional Work

At **Zebra Technologies** I've worked across cloud infrastructure and AI/data engineering, building agentic and retrieval systems for internal enterprise use: a human-in-the-loop agent for BI infrastructure hygiene, a retrieval-augmented agent over an enterprise data lake supporting procurement workflows, and an evaluation harness for measuring agent accuracy and hallucination rates across prompt and retrieval changes.

*Source is proprietary and not published here. Happy to discuss design decisions and tradeoffs in conversation.*

---

## Open Source Projects

### 🛠️ [LLM-Powered Code Assistant](https://github.com/Anirudh-M1/llm-dev-assistant)

A retrieval-augmented assistant for querying and explaining Python codebases — built to explore how retrieval design decisions affect answer quality, and instrumented so that question can be answered with numbers instead of vibes.

**Stack:** `Python` · `FAISS` · `Ollama / Llama3` · `FastAPI` <!-- FILL-IN: delete FastAPI if the API layer isn't built -->

- **Structure-aware chunking** — splits code along functional boundaries (classes and methods) via Python's `ast` module rather than fixed-size windows, preserving qualified names and source line ranges as retrieval metadata.
- **Evaluation harness** — a labeled question set with known ground-truth chunks, measuring `recall@k`, `MRR`, and separated retrieval/generation latency. Reproducible with a single command; results and corpus size published in the repo.
- **Measured results** — <!-- FILL-IN: paste the real headline number from eval/RESULTS.md once it exists, e.g. "recall@5 of 0.XX over a XX-file corpus". Delete this bullet entirely if the harness isn't built yet. -->

<!-- FILL-IN: add an async-ingestion bullet ONLY if the async path is implemented AND benchmarked faster than sequential. Otherwise leave it out. -->

---

### ☕ [DFA Workshop — Full-Stack Data Design](https://github.com/Anirudh-M1/Full-Stack-Data-Design-Workshop)

Rebuilt a monolithic single-file teaching application into a decoupled full-stack architecture, as a reference implementation for peers learning both data engineering and layered software design.

**Stack:** `Java 17` · `Spring Boot` · `Spring Data JPA` · `H2` · `JavaScript (ES6)` · `Maven`

- **Layered backend** — strict `Controller → Service → Repository → DB` separation, with DTOs and explicit mapping components preventing JPA entity leakage into the API surface.
- **Structured error handling** — centralized `@ControllerAdvice` handler returning client-safe `ApiError` JSON for validation failures and missing resources, replacing default white-label stack traces.
- **Decoupled frontend** — modularized layout, styling, and logic; async `fetch` pipeline with a local fallback cache so the client degrades gracefully when the API is unavailable.

---

## Distributed Systems & Low-Level Work

> *These are university coursework projects. Source is kept private in accordance with UIUC academic integrity policy — happy to walk through the architecture, failure modes, and design tradeoffs in an interview.*

#### 📂 HyDFS — Hybrid Distributed File System
A fault-tolerant distributed file system built from scratch for high availability and eventual consistency across a multi-node cluster.
`C++` · `RPC` · `HTTP` · `concurrent programming`
Replication factor of 3 with concurrent write propagation; a background merge process reconciling file blocks after partitions or crashes; control flow (metadata over RPC) separated from data flow (transfers over HTTP) to keep coordination off the bulk path.

#### 🌊 RainStorm — Distributed Stream-Processing Engine
A lightweight stream processor supporting arbitrary execution topologies with exactly-once delivery semantics, benchmarked against Spark.
`Go` · `goroutines/channels` · `distributed scheduling` · `state management`
Leader-worker architecture with load-based scheduling over a synchronized availability map; a custom ping/ack channel system for task monitoring and automatic restart on failure; shuffle, broadcast, and fields-grouping routing semantics.

<details>
<summary><b>More systems & low-level projects</b></summary>

<br>

#### 📡 Gossip-Style Group Membership Protocol
Scalable failure detection with low false-positive rates under packet loss.
`UDP` · `gossip heartbeating` · `SWIM-style ping-ack`
Suspicion mechanism with incarnation numbers allowing nodes to refute false failure claims before being declared failed; tuned for 3-second detection and 6-second cluster-wide dissemination.

#### 🔍 Distributed Log Querier
A distributed `grep` across multi-gigabyte logs on a VM cluster, using bidirectional RPC to fan out and aggregate results in parallel.
`Go` · `bidirectional RPC` · `parallel execution`

#### 🐧 Unix-like Kernel Implementation
Extended a teaching kernel to support full process lifecycles, virtual memory, and hardware abstraction.
`C` · `x86` · `assembly` · `GDB`
Context switching and scheduling for concurrent user-mode execution; page table handling with lazy allocation and process-specific stack mapping; ELF loader and pipes for IPC and I/O redirection.

#### 💻 SLC-3.2 — 16-bit RISC Microprocessor
A 16-bit RISC processor in SystemVerilog, focused on instruction cycle timing and memory interfacing.

</details>

---

## Let's Connect

- 💼 [LinkedIn](https://www.linkedin.com/in/amm21)
- 📧 [amm21@illinois.edu](mailto:amm21@illinois.edu)
- 📄 [Resume](https://github.com/Anirudh-M1/Anirudh-M1/blob/main/Anirudh_Moholkar_Resume.pdf)
