# Systematic Debugging

When a bug, failing test, build error, performance regression or unexpected behavior appears:

1. Reproduce the problem reliably when possible.
2. Read the actual error/output before changing code.
3. Trace the data/control path backward to the earliest incorrect assumption or state.
4. Compare against a nearby working pattern in the repo when one exists.
5. Form one concrete hypothesis.
6. Make the smallest change that tests the hypothesis.
7. Verify the original symptom.
8. Check likely regressions.

Do not stack speculative fixes. If multiple attempted fixes fail, stop and re-investigate rather than increasing patch size.

Fix the source when practical, not merely the place where the symptom becomes visible.

If the cause is genuinely external/environmental, document what was established and add appropriate handling such as timeout, retry, user-facing recovery or observability.
