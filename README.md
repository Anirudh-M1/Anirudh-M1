# Hi, I'm Anirudh Moholkar 👋 
**Computer Engineering @ UIUC | James Scholar | Dean's List | Fiddler Innovation Awardee**  
**SWE Intern @ Zebra Technologies** | *Distributed Systems • Systems Programming • Scalable Infrastructure*

---

### 🚀 Professional Summary
I am a Junior at the **University of Illinois Urbana-Champaign** focused on building high-performance, fault-tolerant systems. With a strong foundation in memory management and concurrency, I’m passionate about solving complex infrastructure challenges in Big Tech and High-Frequency Trading environments.

- 🔭 **Currently Working On:** Optimizing low-level microprocessor designs and kernel-level projects.
- ⚡ **Technical Focus:** Distributed Systems, SystemVerilog, C/C++, and Stream Processing.
- 🛠️ **Experience:** Incoming Data Engineering Intern @ **Zebra Technologies** (Summer 2026).
- 🏛️ **Leadership:** Director of Operations and Technology for **Design for America (UIUC Chapter)**.

---

### 🛠️ Technical Stack & Tools

![My Skills](https://skillicons.dev/icons?i=cpp,c,python,java,go,postgres,docker,linux,git,githubactions)

#### **Technical Skills**
* **Languages:** C, C++, Python, Java, Go, SystemVerilog, SQL  
* **Systems & Infrastructure:** Distributed Systems (HyDFS, RainStorm), Operating System & Kernel Development, RISC Architecture, System Design, Multithreading/Concurrency, Memory Management  
* **Tools & Platforms:** Git, GitHub, CI/CD Pipelines (GitHub Actions, Jenkins), Docker, Linux/Unix, gRPC, REST APIs, Jira, BI Analytics (PowerBI, Tableau)  
* **AI & Agentic Systems:** LangChain, Agentic Workflows (ReAct/Reflection), RAG Architecture, Vector Databases (Pinecone, Milvus), Prompt Evaluation (Evals), LLM Observability

---

### 🤖 AI & Agentic Systems

#### 🛠️ [CodeSense: LLM-Powered Developer Assistant](https://github.com/Anirudh-M1/llm-dev-assistant)
**The Challenge:** Build a scalable Retrieval-Augmented Generation (RAG) system capable of performing semantic search and reasoning across large, multi-repo codebases.
* **Key Tech:** `Python`, `LangChain`, `OpenAI / LLaMA`, `FAISS (Vector DB)`, `FastAPI`, `AsyncIO`
* **Advanced Code Retrieval:** Engineered a specialized chunking pipeline using **Abstract Syntax Trees (AST)** to split code by functional boundaries (classes/methods) rather than naive line counts.
* **Scalable Ingestion:** Implemented an **asynchronous ingestion pipeline** to parallelize embedding generation, maintaining sub-second retrieval latency across 10+ concurrent repositories.
* **Production Engineering:** Developed a **FastAPI backend** with integrated logging to track query-to-explanation performance and retrieval accuracy.

---

### 🧬 Distributed Systems Portfolio

#### 📂 HyDFS: Hybrid Distributed File System
**The Challenge:** Designed and implemented a custom, fault-tolerant DFS from scratch to maintain high availability and eventual consistency across a multi-node cluster.
* **Key Tech:** `C++`, `RPC (Control Flow)`, `HTTP (Data Flow)`, `Concurrent Programming`
* **Replication & Reliability:** Implemented a replication factor of 3 ($log(N)$) using concurrent write requests to ensure zero data loss during node failures.
* **Consistency Engine:** Engineered a **background merge mechanism** that runs every 3 seconds to reconcile file blocks and restore consistency after network partitions or crashes.
* **Performance:** Optimized the architecture by separating the control flow (metadata via RPC) from the data flow (actual transfers via HTTP).

#### 🌊 RainStorm: Distributed Stream-Processing Engine
**The Challenge:** Built a lightweight, scalable stream-processing system capable of handling complex execution topologies with exactly-once delivery semantics.
* **Key Tech:** `Go`, `Goroutines/Channels`, `Distributed Task Scheduling`, `State Management`
* **Architecture:** Designed a **Leader-Worker model** where the leader performs load-based scheduling using a synchronized `MachineAvailability` map to balance tasks across the cluster.
* **Fault Tolerance:** Developed a custom **Ping/Ack channel system** for real-time task monitoring and automatic failure recovery (`RestartTask`).
* **Traffic Management:** Implemented diverse routing semantics (**Shuffle, Broadcast, Fields-grouping**) to manage high-throughput tuple flows.

<details>
<summary><b>View More Distributed Infrastructure Projects</b></summary>

#### 📡 Gossip-Style Group Membership Protocol
**The Challenge:** Developed a highly scalable membership protocol to detect node failures in a distributed system with low false-positive rates under packet loss.
* **Key Tech:** `UDP`, `Gossip Heartbeating`, `SWIM-style Ping-Ack`
* **Advanced Detection:** Implemented a **Suspicion Mechanism** where nodes transition to a `SUSPICIOUS` state before being declared `FAILED`, allowing nodes to refute false failure claims via incarnation increments.
* **Optimization:** Optimized for a 3-second detection time ($T_{detect}$) and 6-second global dissemination ($T_{all}$).

#### 🔍 Distributed Log Querier
**The Challenge:** Created a distributed "grep" tool to query multi-gigabyte log files across a virtual machine cluster with sub-second latency.
* **Key Tech:** `Go`, `Bidirectional RPC`, `Parallel Execution`
* **Efficiency:** Engineered a system that establishes **bidirectional RPC connections** to aggregate results from remote servers in parallel, minimizing query latency to **~100ms**.

</details>

---

### 💻 Low-Level & Systems Engineering

#### 🐧 [Unix-like Kernel Implementation](https://github.com/yourusername/kernel-project)
**The Challenge:** Developed core OS functionalities by extending a teaching kernel to support full process lifecycles, virtual memory, and hardware abstraction.
* **Key Tech:** `C`, `x86 Architecture`, `GDB`, `Assembly`, `Low-level Memory Management`
* **Process Management:** Engineered **context switching** and scheduling mechanisms to facilitate concurrent user-mode execution.
* **Virtual Memory:** Implemented robust **page table handling** with **lazy page allocation** and optimized mapping logic for process-specific stack segments.
* **System Infrastructure:** Designed an **ELF Loader** and developed **Pipes** for Inter-Process Communication (IPC) and I/O redirection.

#### 💻 SLC-3.2: 16-bit RISC Microprocessor
* **The Challenge:** Implementation of a 16-bit RISC microprocessor using **SystemVerilog**, focusing on instruction cycle timing and memory interfacing.

---

### 📫 Let's Connect
- 💼 [LinkedIn](https://www.linkedin.com/in/yourprofile)
- 📧 [Email](mailto:your-email@illinois.edu)
- 📄 [View My Resume](./path-to-your-resume.pdf)

*"Currently deep-diving into lock-free concurrency and preparing for Summer 2026 SWE roles."*
