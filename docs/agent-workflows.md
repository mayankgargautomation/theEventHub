# Agent Workflows for EventHub

This project includes a set of custom Copilot agents tailored for EventHub’s QA and validation workflows.

## Purpose
These agents help the team move faster across the product lifecycle by giving a consistent structure for:
- scenario design
- Playwright test creation
- test review
- test strategy selection
- defect triage
- API validation
- release QA
- PR review

## Agent map

### Functional test planning
- create-scenarios: Generate exhaustive scenarios from domain rules and user flows.

### Automation execution
- generate-tests: Create Playwright E2E tests for a feature or journey.
- review-tests: Check existing Playwright tests for quality and correctness.

### Test strategy
- test-strategy: Assign scenarios to the best test layer in the pyramid.

### Quality and risk
- bug-triage: Investigate failures and isolate root cause.
- api-validation: Validate backend contract, rules, and edge cases.
- release-qa: Run a release-focused QA pass for critical flows.
- pr-review: Review pull requests for risk, business rule alignment, and test gaps.

## Recommended usage by phase

### During feature discovery
Use create-scenarios to build the test inventory before implementation.

### During development
Use generate-tests and review-tests to create and validate the automation coverage.

### Before merging
Use test-strategy and pr-review to assess test layering and risk.

### When a defect is reported
Use bug-triage and api-validation to confirm root cause and affected behavior.

### Before release
Use release-qa to verify the product is production-ready.

## Team guidance
- Prefer real business rules over assumptions.
- Validate both happy paths and negative paths.
- Check both frontend and backend evidence when a bug is suspected.
- Treat booking integrity, access control, and capacity logic as high-risk behaviors.

## Related files
- [.github/agents](../.github/agents)
- [.claude/skills](../.claude/skills)
- [docs/test-scenarios.md](./test-scenarios.md)
- [docs/test-strategy.md](./test-strategy.md)
