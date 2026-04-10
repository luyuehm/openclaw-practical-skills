# openclaw-practical-skills

A unified, practical skill pack for OpenClaw agents.

## What this repo provides

- `self-healing`: structured recovery from regressions and flaky behavior
- `release-readiness`: pre-release checks with evidence-based PASS/FAIL output
- `lesson-extractor`: capture repeatable lessons from incidents into reusable rules

## Layout

```text
skills/
  self-healing/
    SKILL.md
  release-readiness/
    SKILL.md
  lesson-extractor/
    SKILL.md
templates/
  pr-summary.md
README.md
README_CN.md
LICENSE
```

## Quick start

1. Copy skills into your agent workspace:
   - `skills/self-healing`
   - `skills/release-readiness`
   - `skills/lesson-extractor`
2. Run skill workflows with your project context.
3. Keep outputs short, auditable, and evidence-driven.

## Suggested workflow

1. Use **self-healing** to fix incidents.
2. Use **release-readiness** to gate releases.
3. Use **lesson-extractor** to persist hard-won insights.

## Contribution rules

- Keep one skill = one responsibility.
- Include explicit output templates.
- Prefer commands and objective checks over narrative claims.
- Add examples for edge cases.

## License

MIT
