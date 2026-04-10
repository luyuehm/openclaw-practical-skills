---
name: lesson-extractor
description: Distill incident/debug sessions into short reusable lessons and prevention rules.
---

# Lesson Extractor Skill

## Trigger
Use after a bug fix, regression recovery, release incident, or notable debugging session.

## Goal
Convert one-off troubleshooting into reusable team memory.

## Steps
1. Capture symptom in one sentence.
2. Capture root cause in one sentence.
3. Capture fix in one sentence.
4. Capture prevention rule as an actionable checklist item.
5. Verify lesson is specific, testable, and non-generic.

## Output template
```yaml
lesson:
  title: <short title>
  symptom: <what failed>
  root_cause: <why>
  fix: <what changed>
  prevention:
    - <rule 1>
    - <rule 2>
  evidence:
    - <test/command result>
```

## Quality bar
- Keep total under 12 lines.
- No vague advice like "be careful".
- Prevention must be enforceable in CI/checklist/workflow.
