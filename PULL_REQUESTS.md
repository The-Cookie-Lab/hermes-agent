# Hermes-agent Pull Request Overrides

These repo-local overrides target the global PR rule IDs for this private repository.

All activity must stay within my fork (origin). NEVER open PRs to upstream unless I explicitly request it.

Override PR.RULE.NEW_REMOTE_BRANCH_PUSH:
Allow first pushes that create non-default remote feature branches after required local or QA gates pass.

Override PR.RULE.DEFAULT_BRANCH_MUTATION:
Allow merging into `main` only through GitHub/`gh` PR after the PR is green and clean: required local gates pass, hosted CI is green, the exact-head final PR sweep is clean, no review conversations remain unresolved, and the monitored head still matches the branch head. Direct pushes to `main` remain disallowed unless the user explicitly requests that action.
