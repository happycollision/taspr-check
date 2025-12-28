# taspr-check

<!-- taspr-test-repo:v1 -->

This repository is used for integration testing of [taspr](https://github.com/happycollision/taspr).

## Purpose

- Tests PR creation, updates, and merging workflows
- Tests branch protection rule interactions
- Provides deterministic CI pass/fail via commit message markers

## CI Behavior

The CI workflow in this repository:
- **PASSES** for commits without special markers
- **FAILS** for commits containing `[FAIL_CI]` in the subject line

## Do Not

- Do not create manual PRs or branches in this repository
- Do not modify the CI workflow without updating taspr's test expectations
- Do not add branch protection rules manually (tests manage this programmatically)

---
*This repository is automatically managed by taspr integration tests.*
