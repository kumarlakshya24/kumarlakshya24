<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="assets/banner-light.png">
  <img alt="Lakshya Kumar. Applied AI Architect. Secure, measurable LLM systems." src="assets/banner-dark.png" width="100%">
</picture>

<div align="center">

**I design and build applied AI systems:** the gateway in front of the model, the retrieval behind the answer,<br>
the router that picks the model, the runtime that survives a crash, and the evaluation loop that says when quality dropped.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-lakshyakumar24-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lakshyakumar24/)
[![Website](https://img.shields.io/badge/Website-lakshyak.com-111111)](https://lakshyak.com/)
[![Projects](https://img.shields.io/badge/Enterprise%20AI%20Platform-10%20projects%20%C2%B7%20477%20tests-6e56cf)](https://github.com/kumarlakshya24/personal-projects)

</div>

## The Enterprise AI Platform

Ten projects in one repository, [**personal-projects**](https://github.com/kumarlakshya24/personal-projects). Each one tackles a hard part of putting language models in front of employees and agents. Each has an architecture document, decision records with the trade-offs, tests, and a demo that runs offline on synthetic data with no API key.

| | Project | What it does | Measured |
|:-:|:--|:--|:--|
| <img src="assets/dots/aegis.svg" width="10" height="10" alt=""> | [**Aegis**](https://github.com/kumarlakshya24/personal-projects/tree/main/secure-ai-gateway) | Security gateway: replaces personal data with placeholders before a prompt leaves, checks agent tool calls, keeps a tamper-evident audit log | 97.0% recall, 95.5% precision on an 84-case red-team suite |
| <img src="assets/dots/lumen.svg" width="10" height="10" alt=""> | [**Lumen**](https://github.com/kumarlakshya24/personal-projects/tree/main/rag-knowledge-assistant) | Knowledge assistant: cited answers from company documents, with access control inside the retrieval query | Answer accuracy 63% → 89%; restricted-document leaks 100% → 0% |
| <img src="assets/dots/switchboard.svg" width="10" height="10" alt=""> | [**Switchboard**](https://github.com/kumarlakshya24/personal-projects/tree/main/switchboard) | Model router: the cheapest model that is good enough, under a versioned policy | 65% cheaper than always using the premium model, on answered requests |
| <img src="assets/dots/forge.svg" width="10" height="10" alt=""> | [**Forge**](https://github.com/kumarlakshya24/personal-projects/tree/main/forge) | Sandbox for agent tool calls: refuses a dangerous call before a process exists | 55 / 55 eval cases; 41 protections locked by a regression gate |
| <img src="assets/dots/atlas.svg" width="10" height="10" alt=""> | [**Atlas**](https://github.com/kumarlakshya24/personal-projects/tree/main/atlas) | Durable multi-agent workflows: event log, idempotency keys, sagas | 16 / 16 workflows succeed against 3 / 16 for a naive agent; 0 duplicate charges after a crash |
| <img src="assets/dots/lens.svg" width="10" height="10" alt=""> | [**Lens**](https://github.com/kumarlakshya24/personal-projects/tree/main/lens) | Observability and evaluation: traces, a sampled judge, drift, error budgets, a CI quality gate | Judge agreement κ 0.76 with hand labels; a seeded regression is blocked |
| <img src="assets/dots/charter.svg" width="10" height="10" alt=""> | [**Charter**](https://github.com/kumarlakshya24/personal-projects/tree/main/charter) | Governance control plane: which model may run on whose data, in which region | 10 met, 4 partial, 3 gaps on the control matrix |
| <img src="assets/dots/arena.svg" width="10" height="10" alt=""> | [**Arena**](https://github.com/kumarlakshya24/personal-projects/tree/main/arena) | Fine-tune, RAG, or prompt: one labeled set, four ways to answer, and a memo that says which to ship | RAG 25 / 25 cited; the adapter is stale on 3 / 3 amended policies |
| <img src="assets/dots/conduit.svg" width="10" height="10" alt=""> | [**Conduit**](https://github.com/kumarlakshya24/personal-projects/tree/main/conduit) | Embedding pipeline: one model per index generation, a guarded swap, erasure by person | Recall@1 20 / 20 after the swap; 0 links after a rebuild |
| <img src="assets/dots/skyline.svg" width="10" height="10" alt=""> | [**Skyline**](https://github.com/kumarlakshya24/personal-projects/tree/main/skyline) | Cloud landing zone: private accounts, a key per tenant, a price per 1,000 requests | 20 / 20 invariants; $6.26 against $9.20 per 1,000 at 100,000 requests a day (projected) |

Every number comes from an evaluation report committed in that project. Start with the [platform overview](https://github.com/kumarlakshya24/personal-projects#readme), which shows how the ten fit together.

## What I work with

Python 3.12 · FastAPI · PostgreSQL and pgvector · Redis · SQLite · ONNX Runtime · OpenTelemetry-style tracing · Docker Compose · GitHub Actions · AWS (multi-account networking, KMS, Bedrock)
