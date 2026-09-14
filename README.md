# CEM888.AI — Sovereign, Provider-Neutral Agent Runtime

**State decides what is true. Models decide what to do about it.**

CEM888 is a local-first state and control layer that runs underneath AI agents: deterministic memory, tool governance, and verification, with the reasoning model treated as a replaceable driver rather than the source of truth. The goal is agents — on Claude, GPT, DeepSeek, Gemini, or a fully local model — that behave reliably over long-running, multi-session work instead of drifting, over-calling tools, or reporting completion that never happened.

**→ Full architecture and flagship overview: [CEM888AI/cem888](https://github.com/CEM888AI/cem888)**

## The problem

Most agent frameworks let the model hold the state: what happened, what's true right now, whether a task actually finished. That means every new session starts blind, every provider swap resets context, and "the agent said it's done" is the only completion signal you get. CEM888 inverts that: an external, deterministic runtime owns state, memory, and verification; the model is called in to reason and act, and its output is checked against that state rather than trusted at face value.

## In numbers

- **99.9%** (1,998/2,000) on MemoryAgentBench AR, live agent, no answer-key access — next-best published score on the same benchmark is 71.8%. [Full result →](https://github.com/CEM888AI/benchmarks)
- A runaway **207-message** context window, caused by a backward-search anchoring bug, bounded down to a **1,010-token** task-relevant context packet. [Case study →](https://github.com/CEM888AI/runtime-case-studies/blob/main/case-study-context-window-bounding.md)
- A live workflow cut from **4 model calls / 25.6s** to **1 model call / 15.7s** by scoping the tool schema surface to what the turn actually needed, out of 84 registered tools (~29.3K schema tokens). [Case study →](https://github.com/CEM888AI/runtime-case-studies/blob/main/case-study-tool-schema-scoping.md)

## Where to look

| What | Where |
|---|---|
| Flagship — architecture, and what's shown vs. withheld | [CEM888AI/cem888](https://github.com/CEM888AI/cem888) |
| Memory retrieval benchmarks — raw data, reproducible, sourced | [CEM888AI/benchmarks](https://github.com/CEM888AI/benchmarks) |
| Engineering case studies — problem → root cause → fix → measurement | [CEM888AI/runtime-case-studies](https://github.com/CEM888AI/runtime-case-studies) |
| Reliability & control-layer evidence from production runs | [CEM888AI/agent-systems-lab](https://github.com/CEM888AI/agent-systems-lab) |
| Terms, Privacy, EULA, IP documents | [CEM888AI/legal](https://github.com/CEM888AI/legal) |
| Live product | [cem888.ai](https://cem888.ai) |

## Why the engine itself isn't here

CEM888's runtime internals, memory indexing, tool-governance logic, and provider routing are proprietary and stay private. What's public here is the evidence: benchmarks with raw, reproducible data, and case studies with real measurements from the running system — without shipping the implementation that produces them.

## About

Built solo by **Chandler Morone** — self-taught engineer, founder of CEM888. Background before software: dressage trainer, TIG fabricator, self-taught builder of cars, motorcycles, and businesses. Building CEM888 full-time, using AI coding agents as engineering labor while owning the architecture, debugging, acceptance criteria, and system design directly — that division of labor is part of the engineering story, not something hidden behind it. More: [runtime-case-studies/about.md](https://github.com/CEM888AI/runtime-case-studies/blob/main/about.md)

→ [cem888.ai](https://cem888.ai) · creator@cem888.ai
