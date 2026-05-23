> 🧬 [aikdna.com](https://aikdna.com) — Official website

# kdna-code_review

[![KDNA Spec](https://img.shields.io/badge/KDNA-v1.0--rc-4c1)](https://github.com/knowledge-dna/KDNA)

**Code Review** — Reference domain for code review judgment — behavior-first review, comment classification, and anti-rubber-stamp principles.

## Four Questions

### 1. What does this domain judge?

Define the core judgment principles for code review: what to check first, what counts as a real issue, and what self-checks prevent rubber-stamp reviews.

### 2. Where does it apply?

Always load when reviewing code changes, pull requests, or patches. Applies to human-written code, automated refactoring proposals, and security patches.

### 3. Where does it NOT apply?

- Automated linting or formatting-only changes (no behavior to verify)
- Emergency hotfixes with post-deployment audit
- Code generation by AI without human intent (the domain judges review quality, not generation quality)
- Non-code artifacts (documentation, configuration schemas without executable logic)

### 4. How do I use it?

```bash
kdna install github:knowledge-dna/kdna-code_review
kdna validate .
```

## Files

| File | Purpose |
|------|---------|
| KDNA_Core.json | Axioms, ontology, frameworks, core causal structure, stances |
| KDNA_Patterns.json | Terminology, banned terms, misunderstandings, self-checks |
| KDNA_Scenarios.json | Scenario signals that should shift strategy |
| KDNA_Cases.json | Concrete cases showing structure rather than scripts |
| KDNA_Reasoning.json | Reasoning chains: conclusion → logic → so_what |
| KDNA_Evolution.json | Capability stages, measurable indicators, growth paths |
| kdna.json | Domain manifest |
| evals/ | Evaluation cases (quality: untested) |

## License

CC BY 4.0
