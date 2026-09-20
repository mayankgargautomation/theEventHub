# Custom Agents for EventHub

This folder contains project-specific custom agents for QA, testing, and release work.

## Available agents

### create-scenarios
Use when you need functional scenarios and edge-case coverage based on business rules and user flows.

### generate-tests
Use when you need Playwright E2E tests created for a specific feature or flow.

### review-tests
Use when you want a structured review of an existing Playwright test file.

### test-strategy
Use when you need to assign scenarios or features to the right test layer: unit, API, component, or E2E.

### bug-triage
Use when investigating a defect, reproducing it, and narrowing to the root cause.

### api-validation
Use when validating backend behavior, contract correctness, authorization, and error handling.

### release-qa
Use when doing a release-focused QA pass or assessing app readiness before deployment.

### pr-review
Use when reviewing a pull request for correctness, risk, and test coverage.

## How to use
Run these agents from Copilot chat using the agent name, for example:

- /create-scenarios
- /generate-tests
- /review-tests
- /test-strategy
- /bug-triage
- /api-validation
- /release-qa
- /pr-review

## Principles
These agents are designed to follow the project rules:
- validate against EventHub business rules
- prefer real app behavior over assumptions
- check frontend and backend evidence before making a conclusion
- prioritize defect detection and regression prevention
