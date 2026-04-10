---
name: self-healing
description: Recover from regressions and unstable behavior with a strict evidence-driven workflow.
---

# Self-Healing Skill

## Trigger
Use when tests fail, behavior regresses, release confidence is low, or issues are intermittent.

## Workflow
1. Reproduce quickly (target test first, then full suite, then host/integration path).
2. Classify root cause:
   - logic gap / missing branch
   - time-window fragility
   - config or data schema mismatch
   - host integration failure
3. Apply minimal fix (avoid scope creep).
4. Validate in layers:
   - target test
   - full tests
   - host/CLI functional flow
   - release-readiness script/checklist
5. Ship with evidence (commands + passing signals).
6. Capture lessons into stable rules.

## Output template
- Symptom:
- Root cause:
- Fix:
- Validation evidence:
- Risks & boundary:
- Prevention:

## Guardrails
- Do not claim fixed without reproducible evidence.
- Avoid widening unrelated code surface.
- Time-sensitive tests should avoid stale hard-coded timestamps unless intentionally testing expiry.
