# Below-the-App-Layer × AI Infrastructure Roadmap (2026 → 2030)

A five-year plan to build an insurmountable technical moat at the intersection of **systems programming** and **AI infrastructure** — the layer where AI agents are weakest and industry demand is highest.

> **Thesis.** In the AI era, the bottleneck is compute and inference efficiency. The scarcest, highest-leverage skills live below the application layer — GPU kernels, distributed training, AI compilers, inference engines, custom silicon. Systems skills alone are commoditizable; AI skills alone are oversupplied. The **fusion** is the moat.

---

## The Plan at a Glance

| Year | Theme | Systems Track | AI Track | Capstone |
|------|-------|---------------|----------|----------|
| [2026](./2026.md) | Foundations | C, Rust, CSAPP, Linux kernel, xv6 | nanoGPT, transformer math, attention from scratch | CPU-only LLM inference engine |
| [2027](./2027.md) | Parallel & Distributed | CUDA, PMPP, NCCL, Raft, RDMA | Training dynamics, quantization, MoE | GPU inference engine with paged KV |
| [2028](./2028.md) | Compilers & Serving | LLVM, MLIR, Triton, DB internals | Speculative decoding, agent frameworks, RLHF | Production inference stack with novel optimization |
| [2029](./2029.md) | Silicon & Scale | Chisel, FPGA, RISC-V, datacenter | TPU/Groq/Tenstorrent architectures, systolic arrays | FPGA accelerator for attention |
| [2030](./2030.md) | Apex | Research, OSS leadership | Frontier contributions | Published paper + merged upstream contribution |

---

## Why AI Is Woven Into Every Year

Detaching AI from systems in the AI era would be malpractice. Each year pairs a systems track with an AI track that informs it:

- **2026:** you write a toy Linux scheduler *and* a toy transformer — so 2027's CUDA kernels have both systems and model intuition behind them.
- **2027:** you write CUDA matmul *and* understand why FlashAttention's tiling strategy matters for training dynamics.
- **2028:** you write compiler passes *and* understand which speculative-decoding tricks the compiler should fuse.
- **2029:** you design FPGA dataflow *and* understand why TPUs chose systolic arrays for transformers.
- **2030:** you publish at the intersection.

---

## Execution Model

- **Schedule:** 04:00 – 10:00 daily. 6 focused hours. ~2,000 deep-work hours per year.
- **Sleep:** 20:00 → 03:45. Non-negotiable.
- **Rhythm:** 2 h theory · 2 h hands-on code · 1 h papers · 1 h review/writing.
- **Weekly artifact:** one commit, one blog post, or one merged PR. Public moat compounds only when visible.
- **Quarterly review:** reread this roadmap, update status, adjust.

## Tooling

| Tool | Best Use |
|------|----------|
| Claude Max | Socratic tutor, paper→code translator, kernel oops decoder, writing coach |
| Gemini CLI | Long-context paper reading, whole-repo code archaeology |
| Codex / OpenCode / Copilot | Grunt code acceleration only — **never** for code you need to deeply learn |
| OpenRouter | Model comparison for specific tasks; fallback when rate-limited |
| Kindle Paperwhite | Deep reading of canon books; no distraction |
| Anki | Daily spaced repetition on architecture, CUDA, kernel facts |

## The AI-Tool Trap

The danger of this toolkit is **illusion of competence** — AI writes working code, you think you understand. Defenses:

1. **Closed-book rewrites** weekly — redo this week's kernel or algorithm by hand.
2. **Feynman-Claude sessions** — you teach the topic, Claude attacks weak spots.
3. **No-AI coding blocks** — one session per week, timer on, unassisted.

Hard rule: *AI tutors you. AI does not do for you.*

---

## Status Tracking

Each year file ends with a checklist. Tick items as they're done. At year end, snapshot the artifacts (GitHub repos, blog posts, merged PRs, papers) and write a retrospective.

## Meta-Rules

- **Depth over breadth.** The moat compounds in the deep end.
- **Build after every chapter.** Reading without building is recreational.
- **Public artifacts only.** Private progress does not compound.
- **Canon before frontier.** Master the classics, then the latest paper hits harder.
- **One primary project.** If mo-code is shipping hard, the roadmap slows, and vice-versa. Do not half-do both.

---

Start → [2026](./2026.md)
