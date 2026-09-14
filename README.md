# CEM888

### Tell your agents once.

**STATE decides what is true. MODELS decide what to do about it.**

---

## ⭐ The project lives here → **[github.com/CEM888AI/cem888](https://github.com/CEM888AI/cem888)**

**[CEM888AI/cem888](https://github.com/CEM888AI/cem888)** is the flagship repository — source, install, and the star button.
First public beta, AGPL-3.0, shipped September 14 2026.

**[⭐ Star it](https://github.com/CEM888AI/cem888)** · **[⬇️ Install](https://github.com/CEM888AI/cem888#install)** · **[💗 Sponsor](https://ko-fi.com/cem888ai)** · **[🏢 Commercial](mailto:creator@cem888.ai)**

Everything else on this account is supporting evidence for that one repo.

---

[![MemoryAgentBench AR](https://img.shields.io/badge/MemoryAgentBench_AR-99.9%25-1f6feb?style=flat-square)](https://github.com/CEM888AI/benchmarks)
[![Local-first](https://img.shields.io/badge/local--first-your_machine-238636?style=flat-square)](https://cem888.ai)
[![Model-agnostic](https://img.shields.io/badge/models-Claude_·_GPT_·_DeepSeek_·_local-8957e5?style=flat-square)](#)
[![Sponsor](https://img.shields.io/badge/sponsor-keep_this_independent-db61a2?style=flat-square)](https://ko-fi.com/cem888ai)

---

## The 10-second version

Your agent forgets. Every new session starts blind. Switch models and the work resets. And when it says "done," you have no way to know whether it actually happened.

CEM888 moves identity, state, continuity, authority, retrieval, execution control, and verification **outside the model**. The model becomes a replaceable driver. Swap Claude for GPT for a local model mid-project — the agent keeps its state, its permissions, and its work.

**Runs on your machine, against your own model keys. No central server holds your state.**

---

## Where this sits

The agent-memory space is crowded and most of it solves a different problem.

| | Approach | Who holds authority |
|---|---|---|
| Memory layers (Mem0, Zep, Graphiti) | Store and retrieve facts for the model | The model |
| Stateful runtimes (Letta/MemGPT) | Model self-edits tiered memory blocks | The model |
| **CEM888** | **Runtime owns state, governs tool access, and verifies completion against evidence** | **The runtime** |

Memory is necessary and not sufficient. An agent that remembers perfectly can still call the wrong tool, exceed its scope, or report a task complete that never ran. CEM888 treats state, authority, and verification as one control layer — and keeps it local.

## Proof, not claims

| Measurement | Result |
|---|---|
| MemoryAgentBench AR — live agent, no answer-key access | **99.9%** (1,998/2,000) · next-best published: **71.8%** · [raw data →](https://github.com/CEM888AI/benchmarks) |
| Runaway context from a backward-search anchoring bug | **207 messages → 1,010-token** bounded packet · [case study →](https://github.com/CEM888AI/runtime-case-studies/blob/main/case-study-context-window-bounding.md) |
| Workflow with tool-schema surface scoped per turn | **4 calls / 25.6s → 1 call / 15.7s**, from 84 tools (~29.3K schema tokens) · [case study →](https://github.com/CEM888AI/runtime-case-studies/blob/main/case-study-tool-schema-scoping.md) |

Every number links to raw, reproducible data. Case studies include the failures, root causes, and what the fix cost — not just the wins.

## Explore

| | |
|---|---|
| **Benchmarks** — raw, reproducible, sourced | [CEM888AI/benchmarks](https://github.com/CEM888AI/benchmarks) |
| **Case studies** — problem → root cause → fix → measurement | [CEM888AI/runtime-case-studies](https://github.com/CEM888AI/runtime-case-studies) |
| **Reliability evidence** from production runs | [CEM888AI/agent-systems-lab](https://github.com/CEM888AI/agent-systems-lab) |
| **Architecture** | [architecture.md](https://github.com/CEM888AI/runtime-case-studies/blob/main/architecture.md) |
| **Live product** | [cem888.ai](https://cem888.ai) |
| **Legal** — Terms, Privacy, EULA, IP | [CEM888AI/legal](https://github.com/CEM888AI/legal) |

## How this is funded

**The community runtime is free.** It stays free. Revenue comes from two places that don't tax the people using it: commercial licensing for proprietary enterprise productization, and custom enterprise/private integration work.

**Enterprise or custom integration?** → [creator@cem888.ai](mailto:creator@cem888.ai)

## Built and funded by one person

I'm Chandler Morone. I build CEM888 alone, and I paid for it myself.

My background isn't a CS degree — it's dressage, TIG welding, CNC programming, and reading blueprints against what metal actually does under heat. Years of work where a bad weld doesn't throw an exception; it fails in someone's hands. That's the engineering mindset underneath this: verify the claim, don't trust the report.

I sold my dressage horse to keep building. That funded the runtime. It doesn't fund what comes next.

I'm building this because agent infrastructure is consolidating into a handful of clouds that own your state and your lock-in. Local-first is the alternative, and it needs to exist before the window closes.

**Sponsoring keeps it independent and keeps it free.**

→ **[Ko-fi](https://ko-fi.com/cem888ai)** · [One-time](https://donate.stripe.com/cNi28q5WA3l4bVQaqnfbq02) · [Monthly](https://donate.stripe.com/6oU14m3Os3l47FA41Zfbq03)

| Tier | Monthly | |
|---|---|---|
| **Supporter** | $5 | Name in SPONSORS.md — you're keeping the benchmarks running |
| **Backer** | $25 | Build log: what shipped, what broke, what it cost |
| **Believer** | $100 | Early access to the runtime before public release |
| **Company** | $500 | Logo in this README and on cem888.ai |

Sponsorship pays for model API and compute on the benchmark suite, packaging and security review for the public release, and hours spent on the runtime instead of contract work.

---

→ [cem888.ai](https://cem888.ai) · [creator@cem888.ai](mailto:creator@cem888.ai) · [LinkedIn](https://linkedin.com/in/chandler-morone-a8010174)
