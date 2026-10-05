# supremeai-studio — Public Studio UI

**Visibility:** 🟢 Public · **Roadmap phase:** Phase 2 (Week 2–3) · **Ref:** `docs/plans/architecture/SUPREMEAI_REPOSITORY_SEPARATION_AND_EVOLUTION_ROADMAP.md` §4.1, §14

> **চূড়ান্ত লক্ষ্য:** প্রতিটি repo তার boundary-এর ভেতরে থেকে SupremeAI কে আগের চেয়ে ভালো করে তুলবে।

## Responsibility

- User-facing React/Vite Studio UI
- Reusable UI components, UX state, presentation logic
- Public API client (against `supremeai-sdk` contracts)
- Non-sensitive configuration schema, public examples, a11y tests

## Extraction readiness (Phase 0 verified)

- **0 direct backend imports** in `frontend/src` — the boundary is already clean
- Extraction is low-risk; copy history-preserving, replace internal imports with SDK/API calls

## Keep out (roadmap §4.1)

- Private orchestration prompts, internal policy evaluation, production credentials,
  privileged MCP execution code, internal memory datasets

## Governance

AGENTS.md constitution applies. Public quality bar (roadmap §20): license, docs,
tests, security review, dependency scan.
