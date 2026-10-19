# CEM888

### Tell your agents once.

**STATE decides what is true. MODELS decide what to do about it.**

**Start here:** **[cem888.ai](https://cem888.ai/register.html)** → **[Current engineering status](https://github.com/CEM888AI/runtime-case-studies/blob/main/current-engineering-status.md)** → **[Benchmarks](https://github.com/CEM888AI/benchmarks)** → **[Runtime case studies](https://github.com/CEM888AI/runtime-case-studies)**

---

## ⭐ The product → **[cem888.ai](https://cem888.ai/register.html)**

**The runtime source is private.** The `cem888` repository holds the proprietary implementation, licensing and audit record; it is not published, and source access is granted to licensees and design partners rather than opened publicly. This account publishes the evidence layer around it.

First public beta shipped September 14, 2026; the current release line is **v1.0.46**. Every release is licensed under the **CEM888 Source-Available Commercial License** — source-available to licensees, never converts. No CEM888 release has ever been published under an open-source licence; v1.0.3 is the audit record, not a published engine.

**To evaluate CEM888 or use it personally/non-commercially: create an account at [cem888.ai](https://cem888.ai/register.html), sign in, and download it for your machine. Business production use requires a commercial license from CEM Unlimited LLC.**

**[🚀 Create a free account & download](https://cem888.ai/register.html)** · **[📋 Current status](https://github.com/CEM888AI/runtime-case-studies/blob/main/current-engineering-status.md)** · **[🏢 Commercial](mailto:creator@cem888.ai)**

Everything else on this account is supporting evidence for that product.

---

[![BEAM-10M](https://img.shields.io/badge/BEAM--10M-77.2%25-1f6feb?style=flat-square)](https://github.com/CEM888AI/benchmarks)
[![Local-first](https://img.shields.io/badge/local--first-your_machine-238636?style=flat-square)](https://cem888.ai)
[![Model-agnostic](https://img.shields.io/badge/models-Claude_·_GPT_·_DeepSeek_·_local-8957e5?style=flat-square)](#)

---

## The 10-second version

Long-running agents can lose current state, carry stale decisions forward, repeat work after retries, or report success without external proof.

CEM888 moves identity, authoritative state, continuity, action authority, verification, and **receipts** outside the model. The runtime is designed so model/provider changes do not have to own the agent's durable operational truth; each host/provider path is certified separately and should not be assumed equivalent until measured.

**Runs on customer-controlled machines or infrastructure, against the customer's chosen model path. CEM888 does not centrally execute customer agents.**

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
| **BEAM-10M** (benchmark of record) — live agent, no answer-key access | **77.2%** (154.4 / 200) · [method + per-question data →](https://github.com/CEM888AI/benchmarks) |
| Independent runtime evaluation — durable state, kill-and-recover, model swap, verified execution, authority boundary, unknown state, provenance, contradiction/freshness, failure recovery | **9 / 9 pass** · [evaluation →](https://huggingface.co/datasets/CEM888AI/cem888-independent-runtime-evaluation) |
| Runaway context from a backward-search anchoring bug | **207 messages → 1,010-token** bounded packet · [case study →](https://github.com/CEM888AI/runtime-case-studies/blob/main/case-study-context-window-bounding.md) |
| Workflow with tool-schema surface scoped per turn | **4 calls / 25.6s → 1 call / 15.7s**, from 84 tools (~29.3K schema tokens) · [case study →](https://github.com/CEM888AI/runtime-case-studies/blob/main/case-study-tool-schema-scoping.md) |
| MemoryAgentBench AR — **retrieval only**, not end-to-end memory | 99.9% (1,998 / 2,000) · [raw data →](https://github.com/CEM888AI/benchmarks) |

The runtime evaluation was run by an AI engineering assistant on Hugging Face Jobs infrastructure on September 18, 2026 (Debian 13, DeepSeek, CEM888 v1.0.x). Its full method and terms are on the dataset page.

Every number links to its supporting evidence. Case studies show the real engineering: root causes, fixes, and measurements.

## Explore

| | |
|---|---|
| **Current status** — shipped, in progress, and explicitly not claimed | [runtime-case-studies/current-engineering-status.md](https://github.com/CEM888AI/runtime-case-studies/blob/main/current-engineering-status.md) |
| **Get CEM888** — free account, sign in, download | [cem888.ai](https://cem888.ai/register.html) |
| **Benchmarks** — raw, reproducible, sourced | [CEM888AI/benchmarks](https://github.com/CEM888AI/benchmarks) |
| **Case studies** — problem → root cause → fix → measurement | [CEM888AI/runtime-case-studies](https://github.com/CEM888AI/runtime-case-studies) |
| **Reliability evidence** from production runs | [CEM888AI/agent-systems-lab](https://github.com/CEM888AI/agent-systems-lab) |
| **Architecture** | [runtime-case-studies/architecture.md](https://github.com/CEM888AI/runtime-case-studies/blob/main/architecture.md) |
| **Legal** — Terms, Privacy, EULA, IP | [CEM888AI/legal](https://github.com/CEM888AI/legal) |

## Licensing

**Current and future CEM888 releases are licensed under the CEM888 Source-Available Commercial License.** It grants use, copying, distribution and modification **for personal, non-commercial use** to those issued the software or granted source access, and it **never converts into an open-source license.** **Nothing that makes money, or builds a business, is free:** business production use, paid client work, embedding, white-labeling, resale, hosted or managed service use, and OEM use all require a **paid commercial license from CEM Unlimited LLC** (negotiated terms). Release history: one licence across every release — no CEM888 release has ever been published under an open-source licence, and no runtime engine source has ever been published.

**Enterprise or custom integration?** → [creator@cem888.ai](mailto:creator@cem888.ai)

## Built by Chandler Morone, Founder

I'm Chandler Morone, founder of CEM888.

My engineering background spans agent infrastructure, fabrication, TIG welding, CNC programming, blueprints, and competitive dressage. The common thread is simple: the result has to match the claim.

That principle became part of CEM888's architecture. Models can propose actions and describe outcomes; the runtime owns state, verifies consequential work against evidence, and preserves **receipts** showing what actually happened.

I built and funded the runtime independently because agent infrastructure should not require surrendering persistent state and control to a single model provider or cloud.

---

→ [cem888.ai](https://cem888.ai) · [creator@cem888.ai](mailto:creator@cem888.ai) · [LinkedIn](https://linkedin.com/in/chandler-morone-a8010174) · [Sponsors](https://github.com/CEM888AI/CEM888AI/blob/main/SPONSORS.md)
