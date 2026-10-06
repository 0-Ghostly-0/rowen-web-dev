# Anti-Overengineering Gate

This skill contains many checks. They are conditional, not a requirement to build maximum infrastructure.

Before adding complexity, ask:
1. Is this relevant to the actual feature?
2. What concrete failure/user need does it solve?
3. Is there a simpler existing platform/repo solution?
4. Does the risk justify the implementation/maintenance cost?

Examples:
- a static portfolio does not need a database/admin panel merely because the skill knows how to build one;
- a tiny local state change does not need a global state library;
- a simple hover does not need a motion dependency;
- a low-risk marketing edit does not need enterprise-grade test scaffolding;
- an admin dashboard should exist only when there is meaningful operational data to manage.

Quality means appropriate completeness, not maximum machinery.
