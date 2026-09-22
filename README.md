# Global SaaS Compliance Skill

Open-source, agent-agnostic product compliance skill for SaaS, web, mobile, API, developer, and AI products.

## Purpose
Given product facts, data, features, users, and jurisdictions, help an AI/software agent determine applicable product-level requirements, engineering controls, and evidence.

Scope deliberately excludes company formation, tax, payroll, accounting, and founder registration.

## Structure
- `SKILL.md` — core agent workflow
- `references/` — methodology, domains, official sources
- `jurisdictions/` — jurisdiction starting points
- `schemas/` — machine-readable contracts
- `templates/` — reusable inputs/registers
- `examples/` — sample product profiles

## Agent usage
Expose `SKILL.md` through the agent's skill/instructions mechanism. For other agents, provide the file plus only the relevant jurisdiction/domain references.

Example request:
> Assess my SaaS operating from India with EU/US users. It stores resumes, uses an LLM, sends email, accepts subscriptions and integrates with GitHub. Identify applicable privacy, AI, security, marketing, payment, accessibility and IP requirements. Cite authoritative sources, distinguish law from standards, and map each item to engineering controls and evidence.

## Important
This is a compliance-engineering aid, not legal advice. Laws change. Verify current requirements against authoritative sources and qualified counsel where appropriate.

## License
Apache-2.0.
