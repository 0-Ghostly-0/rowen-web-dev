# Risk-Based Security Review

Assess the actual project before choosing checks.

Inventory:
- authentication/session model;
- admin access;
- roles/authorization and object ownership;
- sensitive data;
- forms/public APIs;
- uploads/downloads;
- payments/webhooks;
- third-party integrations;
- expensive operations;
- secrets;
- user-generated HTML/content.

Then review relevant threats. Do not pretend every project has the same attack surface.

High-value checks commonly include:
- broken access control / IDOR;
- missing server-side authorization;
- injection/XSS;
- CSRF where applicable;
- leaked secrets/client exposure;
- unsafe redirects;
- insecure upload/file access;
- webhook spoofing/replay;
- brute force/automation;
- overly broad DB/storage permissions;
- unsafe error/log leakage;
- dependency vulnerabilities.

Report findings with evidence and severity; do not claim security from a checklist alone.
