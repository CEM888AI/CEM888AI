# CEM888 — Sovereign, Provider-Neutral Agent Runtime

**State decides what is true. Models decide what to do about it.**

[![Benchmarks](https://img.shields.io/badge/MemoryAgentBench_AR-99.9%25-1f6feb?style=flat-square)](https://github.com/CEM888AI/benchmarks)
[![Case studies](https://img.shields.io/badge/engineering-case_studies-238636?style=flat-square)](https://github.com/CEM888AI/runtime-case-studies)
[![Sponsor](https://img.shields.io/badge/sponsor-this_work-db61a2?style=flat-square)](https://ko-fi.com/cem888ai)

CEM888 is a local-first state and control layer that runs *underneath* AI agents: deterministic memory, tool governance, and verification, with the reasoning model treated as a replaceable driver rather than the source of truth. Agents that hold their state across sessions and across providers — Claude, GPT, DeepSeek, Gemini, or fully local — instead of drifting, over-calling tools, or reporting completion that never happened.

---

## Built by one person, funded by one person

I'm Chandler Morone. I build CEM888 alone.

Before software I was a dressage trainer and a TIG fabricator — years spent on work where a bad weld doesn't throw an exception, it fails in someone's hands. That's the mindset the runtime is built on: verify the claim, don't trust the report.

I sold my dressage horse to fund the runtime. That paid for the build. It doesn't pay for what comes next.

**If the numbers below are worth something to you, sponsoring is how this keeps going.**

→ **[Sponsor on Ko-fi](https://ko-fi.com/cem888ai)** · [One-time](https://donate.stripe.com/cNi28q5WA3l4bVQaqnfbq02) · [Monthly](https://donate.stripe.com/6oU14m3Os3l47FA41Zfbq03)

---

## The problem

Most agent frameworks let the model hold the state: what happened, what's true right now, whether a task actually finished. Every new session starts blind, every provider swap resets context, and "the agent said it's done" is the only completion signal you get.

CEM888 inverts that. An external, deterministic runtime owns state, memory, and verification. The model is called in to reason and act, and its output is **checked against that state** rather than trusted at face value.

## In numbers

| Measurement | Result |
|---|---|
| MemoryAgentBench AR — live agent, no answer-key access | **99.9%** (1,998/2,000) · next-best published: 71.8% · [data →](https://github.com/CEM888AI/benchmarks) |
| Runaway context window, backward-search anchoring bug | **207 messages → 1,010-token** bounded packet · [case study →](https://github.com/CEM888AI/runtime-case-studies/blob/main/case-study-context-window-bounding.md) |
| Live workflow, tool-schema surface scoped to the turn | **4 calls / 25.6s → 1 call / 15.7s**, from 84 tools (~29.3K schema tokens) · [case study →](https://github.com/CEM888AI/runtime-case-studies/blob/main/case-study-tool-schema-scoping.md) |

Every number above links to raw, reproducible data. None of it is a marketing claim.

## What sponsorship actually pays for

Not a tip jar. Specific line items, in priority order:

1. **Model API and compute** — the benchmark suite and regression runs that produce the numbers above cost real money to re-run on every change. Unfunded, they run less often, and the evidence goes stale.
2. **Publishing the runtime** — packaging, installer signing, and the security review needed before the flagship goes public and installable.
3. **Keeping me building full-time** — I have no salary, no co-founder, no investor. Every hour funded is an hour on the runtime instead of contract work.

## Sponsor tiers

| Tier | Monthly | What you get |
|---|---|---|
| **Supporter** | $5 | Name in SPONSORS.md. You're keeping the benchmarks running. |
| **Backer** | $25 | Above, plus the build log — what shipped, what broke, what it cost. |
| **Believer** | $100 | Above, plus early access to the flagship release before it's public. |
| **Company** | $500 | Above, plus your logo in this README and on cem888.ai. |
| **Commercial** | — | Using CEM888 in a product? [creator@cem888.ai](mailto:creator@cem888.ai) — that's a license, not a sponsorship. |

**Sponsoring a personal account on GitHub carries no platform fee** — 100% arrives.

## Evidence

| What | Where |
|---|---|
| Memory retrieval benchmarks — raw, reproducible, sourced | [CEM888AI/benchmarks](https://github.com/CEM888AI/benchmarks) |
| Engineering case studies — problem → root cause → fix → measurement | [CEM888AI/runtime-case-studies](https://github.com/CEM888AI/runtime-case-studies) |
| Reliability & control-layer evidence from production runs | [CEM888AI/agent-systems-lab](https://github.com/CEM888AI/agent-systems-lab) |
| Conceptual architecture | [architecture.md](https://github.com/CEM888AI/runtime-case-studies/blob/main/architecture.md) |
| Terms, Privacy, EULA, IP | [CEM888AI/legal](https://github.com/CEM888AI/legal) |
| Live product | [cem888.ai](https://cem888.ai) |

## Why the engine isn't here yet

CEM888's runtime internals, memory indexing, tool-governance logic, and provider routing are proprietary and stay private for now. What's public is the evidence: benchmarks with raw data and case studies with real measurements from the running system — without shipping the implementation that produces them.

The flagship goes public when it's installable and safe to install. Sponsorship is what shortens that gap.

---

→ [cem888.ai](https://cem888.ai) · [creator@cem888.ai](mailto:creator@cem888.ai) · [LinkedIn](https://linkedin.com/in/chandler-morone-a8010174)
