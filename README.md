# Fillipe Loose

**AI & Data Engineer** · I build production AI systems for legal and regulated documents that non-technical people actually use.

Currently the first and only in-house engineer at a 40-person law firm in Brazil, where I own the AI and automation stack end to end: LLM pipelines over court and tax documents, a deadline-control pipeline, an AI-assisted intake flow in production, and the data layer behind the firm's dashboards.

Before that: two years administering state-wide government databases and building the analytics over ~1,000 public schools and 500,000+ students.

🎓 BSc Computer Science, PUC Goiás (Dec 2026) · degree recognised in Germany (anabin H+)
🌍 Relocating to Europe in 2027 · open to roles with visa sponsorship
🔗 [LinkedIn](https://www.linkedin.com/in/fillipeml) · [RenavePro](https://renavepro.com), my own SaaS

### What I work with
`Python` `TypeScript` `SQL` `Next.js` `React` `PostgreSQL` `SQLite` `AWS` `Docker` `Claude API` `Microsoft Graph` `GitHub Actions`

### Featured work
| Project | What it is | Stack |
|---|---|---|
| [tax-settlement-analytics](https://github.com/fillipeml/tax-settlement-analytics) | Analytics on 1,134 public tax-settlement terms extracted with an LLM into a versioned dataset, plus a client-side simulator that checks a proposal against the law and against what the treasury has actually accepted. In production at a tax team. | Python · Next.js · Claude API (Files API, Batches) |
| [court-deadline-triage](https://github.com/fillipeml/court-deadline-triage) | Daily triage of court gazette publications: a model classifies the deadline type, a deterministic engine computes the due date over versioned court calendars, a lawyer confirms. Pilot; 161 tests with hand-computed golden cases. | Python · Claude API · SQLite |
| [court-notice-monitor](https://github.com/fillipeml/court-notice-monitor) | Read-only daily sweep of the electronic judicial domicile: lists, triages and alerts, and is built so it cannot acknowledge service. In production for a law firm. | Python · SQLite · Microsoft Graph |
| [eu-job-pipeline](https://github.com/fillipeml/eu-job-pipeline) | Multi-source European job ingestion with rule-based and LLM fit scoring, a golden-set evaluation and an offline demo mode. | Python · Claude API · SQLite |

Next up: a judgment-liquidation engine with golden cases, a settlement-reminder pipeline in production (194 tests) and a full-stack case-diagnostics app.

### How I work
- I run discovery with the people who will use the thing, then decide the architecture, then build it, then train them.
- I make trade-offs explicit: moved a document pipeline from an agentic loop to the Batches API (about half the cost) and cut token spend by roughly 90 % with prompt caching; each README says what a decision cost.
- Legal rules are code, not prompts: every deadline, discount cap and threshold is deterministic and has a hand-computed test.
- I use AI coding tools daily and treat their output like a junior's pull request: reviewed, tested and validated against a schema before it ships. Every repository documents what was generated and what I changed.

> Most of my production work is under employer or client agreements. The repositories here are rebranded, anonymised versions of those systems, running on fictional or public data in demo mode: the architecture and the decisions are real, the private data is not.
