---
name: release-readiness
description: Run pre-release checks and produce a PASS/FAIL evidence summary.
---

# Release Readiness Skill

## Core checks
1. Repo healthy and clean state known
2. Version sync (manifest/package)
3. Full regression tests
4. Host/integration functional test
5. Import/list/search/stats/export flow
6. Delete idempotency
7. Optional migration run/verify
8. Packaging dry-run

## Recommended commands
```bash
npm test
npm run test:openclaw-host
bash scripts/release-readiness-check.sh
```

## Output format
```yaml
release_readiness:
  status: pass|fail
  summary:
    total_checks: <n>
    passed: <n>
    failed: <n>
  failed_items:
    - <item>
  evidence:
    - <command + result>
```
