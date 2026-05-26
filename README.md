> 🧬 [aikdna.com](https://aikdna.com) — Official website

# @aikdna/code_review

[![KDNA Spec](https://img.shields.io/badge/KDNA-v1.0--rc-4c1)](https://github.com/aikdna/KDNA)

**Code review judgment** — behavior-first review, comment classification, and anti-rubber-stamp principles.

## What this KDNA changes

**Before loading this KDNA, an agent tends to:**
- Approve changes that "look correct"
- Leave vague or cosmetic review comments
- Rubber-stamp pull requests that pass tests

**After loading this KDNA, an agent will judge:**
- Does every review comment that requests a change cite a specific failure mode?
- Does a fix remove the symptom while preserving the failure condition?
- Do passed tests mean eliminated risk?
- Is "LGTM without verification" ever acceptable?

## This KDNA is for

- Reviewing code changes, pull requests, or patches
- Human-written code, automated refactoring proposals, and security patches

## This KDNA is not for

- Automated linting or formatting-only changes (no behavior to verify)
- Emergency hotfixes with post-deployment audit
- AI-generated code without human intent
- Non-code artifacts (documentation, config schemas without executable logic)

## Core judgment

Every review comment that requests a change must cite a specific failure mode. A fix that removes a symptom while preserving the failure condition is not complete. Silent approval without verification is not review.

## Self-checks

- Does every change request cite a specific failure mode?
- Does this fix actually resolve the failure condition?
- Am I verifying behavior, not just looking at code?
- Is this "LGTM" backed by actual verification?

## Install

```bash
kdna install @aikdna/code_review
kdna dev validate .
```

## Files

- `KDNA_Core.json` — Axioms, ontology, frameworks, causal structure, stances
- `KDNA_Patterns.json` — Terminology, banned terms, misunderstandings, self-checks
- `KDNA_Scenarios.json` — Scenario signals that shift strategy
- `KDNA_Cases.json` — Concrete cases showing judgment structure
- `KDNA_Reasoning.json` — Reasoning chains: conclusion → logic → action
- `KDNA_Evolution.json` — Capability stages, measurable indicators, growth paths
- `evals/` — Evaluation cases (quality: untested)
- `kdna.json` — Domain manifest

## License

CC BY 4.0
