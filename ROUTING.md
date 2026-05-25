# ROUTING.md — @aikdna/code_review

## When this domain SHOULD be loaded

- Reviewing pull requests, code changes, or patches
- Evaluating whether code meets architectural standards
- Assessing security implications of dependency changes
- Judging whether a change is ready to merge
- Identifying patterns that indicate technical debt

## When this domain should NOT be loaded

- Writing new code from scratch (generation, not review)
- Debugging runtime errors (execution, not review)
- Explaining how existing code works (documentation, not review)
- Formatting or linting (mechanical, not judgment)

## Easily confused tasks (contamination risks)

| Task that looks relevant | Why it should NOT load this domain |
|--------------------------|-----------------------------------|
| "Write a function that does X" | Code generation; not review |
| "Why is this test failing?" | Debugging; not review |
| "Format this file with prettier" | Mechanical formatting |
| "Explain what this code does" | Documentation/explanation |

## Recommended test statements

**Should load:**
1. "Review this PR — is it safe to merge?"
2. "Does this change introduce architectural risk?"
3. "Is this dependency upgrade safe?"

**Should skip:**
1. "Write a React component for a login form"
2. "Why is this API returning 500?"
3. "Document this module"

## Confidence guidance

- Load without asking when: task is explicitly a code review or PR evaluation
- Always skip when: task is generation, debugging, or documentation
