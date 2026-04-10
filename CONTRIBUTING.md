# Contributing to openclaw-practical-skills

Thanks for contributing practical skills for OpenClaw agents.

## Contribution Principles

1. **One skill, one responsibility**
   - Keep each skill focused and composable.
2. **Evidence over narration**
   - Prefer commands, checks, and explicit output templates.
3. **Operationally safe by default**
   - Include guardrails for risky actions.
4. **Reusable in real projects**
   - Keep wording concrete and implementation-friendly.

## Skill Quality Checklist

A skill PR should include:

- `SKILL.md` frontmatter with:
  - `name`
  - `description`
- Clear **trigger conditions**
- Step-by-step workflow
- Standardized output template (YAML/text)
- Guardrails / boundary notes
- At least one practical example (if applicable)

## Recommended Structure

```text
skills/<skill-name>/SKILL.md
```

## Local Validation Before PR

- Ensure markdown renders correctly
- Keep language concise and deterministic
- Verify examples/commands are executable or clearly marked pseudocode

## Pull Request Guidelines

Please include:

1. Why this skill is needed
2. What scenario it targets
3. Expected output format
4. Risks and boundaries

Use this PR template section:

- Summary
- Motivation
- Skill design
- Output contract
- Risks / boundaries

## Scope Rules

- Avoid bundling unrelated skills in one PR.
- Prefer incremental PRs over massive drops.
- If updating existing skill behavior, mention backward-compatibility impact.

## Code of Conduct

Be respectful, practical, and evidence-driven.
