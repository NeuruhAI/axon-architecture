# AXON

**An edge-sovereign architecture for agentic AI.**

Most "AI agent" systems are cloud wrappers with a nice UI. The moment the model provider ships a new feature, the product is redundant.

AXON is the opposite bet: a **local-first agentic pipeline** with a hardened permission layer, dual-memory, and cross-model routing that treats cloud APIs as optional accelerators — not load-bearing dependencies.

- **$0 marginal inference cost** on owned hardware
- **5.3 GB VRAM operational ceiling** (runs on a consumer M1 Mac Mini)
- **SAL Engine** — fragment-based token budget fitting so context never overflows the model
- **Dual memory:** Obsidian vault (private cognition) + Notion (shared persistence)
- **Tailscale relay** for secure mobile-to-local command without exposing the box to the public internet
- **Model-agnostic** — routes to local Bonsai/Gemma or Claude/GPT/Groq as needed

## Read

- [**Executive Summary**](./EXECUTIVE_SUMMARY.md) — one-page pitch for investors, partners, serious operators
- [**Full White Paper**](./WHITEPAPER.md) — the 8-section architecture deep dive
- [**Diagrams**](./diagrams/) — Mermaid source you can drop into any doc

## The Cloud API Trap

Every cloud-only agentic stack ships with three non-negotiable failure modes:

1. **Billing walls** — intelligence gated behind per-token costs that kill autonomous ops at scale
2. **Latency** — every hop is a round trip to someone else's datacenter
3. **Privacy** — your proprietary context leaves your building on every request

AXON starts from the other side: compute is local, memory is local, routing is explicit. Cloud calls happen only when they earn the trip.

## Status

- **Phase 1** — Gateway shipped. Tool Interface Standard, Permission Guard, Registry live. [`NeuruhAI/neuruh-axon`](https://github.com/NeuruhAI/neuruh-axon)
- **Phase 2** — Coordinator + Memory (in progress)
- **Phase 3** — Prompt Composer + Cost Tracker
- **Phase 4** — Adapter SDK
- **Phase 5** — Public Gateway API

## Built by

[Neuruh](https://neuruh.com) — Jeramie Hicks. Solo founder, Benton Harbor MI.

No VC. No co-founder. Two live clients. 370+ IP entries. An AI-operated business, not an AI-assisted one.

If this resonates — star the repo, share the white paper, and come build with us.

## License

Documentation and diagrams: [CC BY 4.0](./LICENSE). You can reference, remix, and build on AXON — just credit Neuruh.

Runtime code lives in the main AXON Gateway repo under its own license.
