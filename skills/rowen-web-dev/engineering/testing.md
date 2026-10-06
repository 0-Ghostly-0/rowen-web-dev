# Testing Strategy

Testing should match risk.

Prioritize tests for:
- authentication/authorization;
- payments/webhooks;
- destructive admin operations;
- persistence and data transformations;
- uploads;
- important business rules;
- bug regressions;
- complex state transitions.

Prefer behavior-focused tests over implementation-detail tests.

For a bug fix, add a regression test when it is useful and proportionate.

Do not force strict TDD onto trivial styling, throwaway prototypes or low-risk mechanical edits. For important behavior, writing the failing test first is preferred when practical because it demonstrates the test can detect the defect.

A test suite is not a substitute for rendered browser QA.
