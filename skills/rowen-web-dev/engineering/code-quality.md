# Code Quality and Simplicity

Prefer the smallest architecture that cleanly supports the product.

Before adding:
- a dependency, check whether the platform/repo already solves it;
- an abstraction, confirm there is real repetition or volatility;
- global state, confirm state must actually be global;
- a new service, confirm existing infrastructure is insufficient.

Follow established repo patterns unless they are the problem.

After implementation, remove dead code, duplicate logic, debugging leftovers, fake data and unnecessary indirection introduced by the change.

Do not refactor unrelated areas merely because they could be cleaner.
