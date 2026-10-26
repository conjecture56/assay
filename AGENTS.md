# AGENTS.md

Instructions for AI agents working in this repository.

## Purpose

This repository defines the **Assay** project: a self-hosted, reproducible evaluation methodology and tool for AI agent workflows, owned by Conjecture 56. At this stage the repository contains definition documents only — no executable code yet.

## Content conventions

- User-facing documents (`README.md`, `docs/*.md`) are written in **Spanish**. Preserve this. Do not translate existing documents or switch their language when editing.
- Code, identifiers, configuration keys, and future source files use **English**.
- `AGENTS.md` (this file) is written in English because it is primarily agent-facing tooling.

## Editorial rules

- Claims about security, privacy, or compliance must be scoped. Never state that a system is "secure" or that data "never leaves" infrastructure unless the claim is bounded to a described control and verified in context.
- Self-hosted means data does not reach Conjecture 56. It does not mean data stays local when users configure external model or tool providers. Preserve this distinction in every document.
- Do not describe the product as an "independent audit" of customer systems. Without direct access to evidence, the correct terms are "guided self-assessment" or "verifiable self-managed evaluation".
- Do not add customer testimonials, simulated promotions, or marketing superlatives. This project communicates evidence, not advertising.
- When editing `docs/business-model.md` or `docs/roadmap.md`, keep the zero-custody constraint intact: Conjecture 56 must never operate a service that receives or processes third-party customer data.

## Commits

- Conventional Commits format, e.g. `docs: define measurement model`.
- One logical work unit per commit.
- Never add `Co-Authored-By` or any AI attribution lines.

## Reference material

- Project framework and research lines: <https://github.com/conjecture56/charter>
- Evidence scale used for Conjecture 56 outcomes: `conjecture56/charter` → `docs/conjecture56_escala_resultados_impacto.md`
