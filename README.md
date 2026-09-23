# Bruno Rodrigues

**Senior Software Engineer** — Node.js · TypeScript · AWS · AI-assisted engineering
Florianópolis, Brazil (Remote) · [LinkedIn](https://www.linkedin.com/in/brnbruno/) · [brunorodrinasc@gmail.com](mailto:brunorodrinasc@gmail.com)

5+ years building, modernizing, and maintaining business-critical web applications and APIs — TypeScript, Node.js, React/Next.js, PHP, Go, AWS, Kafka, distributed systems. A lot of that work is untangling complex business rules inside legacy systems without breaking what already works. Day to day, I use Claude Code, Cursor, and ChatGPT deliberately — for codebase investigation, implementation, debugging, and documentation — not to skip engineering judgment, but to move faster while keeping it.

---

## Featured project — [COMIGO](https://github.com/BrunoRodriguesNasc/Comigo)

A cosmetics-compatibility PWA: scan a product, get a **personal, explainable compatibility score** for your skin — never a generic "toxic/safe" verdict. Built and documented as a portfolio-grade example of how I actually work:

- **Deterministic core, AI on the edges.** The scoring engine (`src/domain`) is pure TypeScript with zero LLM in the score/verdict path — tested with `Σ rule contributions === final score` as an enforced invariant. AI only explains a result the engine already computed, with a working non-AI fallback.
- **Uncertainty as a first-class output.** Unrecognized ingredients lower confidence instead of being silently ignored; below a coverage threshold the verdict shows "insufficient data" instead of a falsely confident badge — a rule born from a real bug I caught with real data.
- **Rules and weights are versioned data**, not code — editable from an admin panel, validated with Zod, with a schema that blocks an invalid ruleset before it ships.
- **AI agents work under a written brief.** A [`CLAUDE.md`](https://github.com/BrunoRodriguesNasc/Comigo/blob/main/CLAUDE.md) at the repo root governs how Claude Code operates in that codebase — module boundaries, when to bump the engine version, banned language, and "question it before implementing if it conflicts with the product principle."

→ [Full architecture, rules engine, and AI-assisted workflow write-up](https://github.com/BrunoRodriguesNasc/Comigo#readme)

---

## How I use AI in engineering

Not vibe-coding — governed AI usage. On real projects that means: docs and decisions written before implementation, explicit module boundaries an agent has to respect, and guardrails (like "no LLM in the scoring logic") written into the agent's instructions and checked in review, not just assumed. I've also prototyped agent-facing infrastructure beyond application code: a read-only **MCP server** exposing structured feature-flag and business-rule knowledge to AI assistants, to cut down on manually searching large enterprise codebases.

---

## Tech stack

**Languages** TypeScript · JavaScript · Go · PHP · Python · Java
**Backend** Node.js · NestJS · Express · REST APIs · Microservices
**Frontend** React · Next.js · Tailwind CSS
**Data** SQL · NoSQL · Prisma · TypeORM
**Infra** AWS · Docker · Kafka
**Observability & testing** Jest · Vitest · Kibana · New Relic
**AI-assisted engineering** Claude Code · Cursor · ChatGPT · MCP

---

## Currently

- **Senior Software Engineer @ TOTVS** (2024–present) — production reliability and legacy modernization on enterprise systems with complex business rules; cut a critical backlog from 30 items to 3 in one quarter.
- Previously **Senior Software Engineer @ Ahgora Sistemas** (2020–2024) — business-critical systems for large Brazilian clients (Via Varejo, Mercado Livre), sustaining a 90% SLA target.

Older personal portfolio (pre-AI-assisted-engineering era, kept for continuity): [brunorodridev.vercel.app](https://brunorodridev.vercel.app/)
