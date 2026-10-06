# Verification Before Completion

Evidence must match the claim.

Before saying something is complete, fixed, passing or production-ready:
1. State what evidence would prove that specific claim.
2. Run/inspect that evidence freshly when tools are available.
3. Read the result rather than assuming success.
4. Report gaps honestly.

Examples:
- "Build passes" -> successful full build output.
- "Tests pass" -> relevant test command with no failures.
- "Bug fixed" -> original reproduction no longer fails, plus relevant regression check.
- "UI works" -> rendered interaction exercised.
- "Feature complete" -> requirements checked individually, not merely tests passing.
- "All routes fixed" -> verify the authoritative route set, not only edited files.

Never use one weak signal (for example HTTP 200 or a successful lint) to prove a stronger claim it does not establish.
