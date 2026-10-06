# Production Launch Review

Before a meaningful production launch/relaunch, review what applies:

- production build/tests;
- rendered browser QA;
- environment variables and environment scoping;
- database migrations and backups/rollback considerations;
- admin authentication/access;
- rate limiting/WAF/abuse controls;
- secrets not exposed to client or repo;
- Stripe/webhook production configuration;
- upload/storage permissions and limits;
- analytics/monitoring/error visibility;
- canonical domain, redirects, sitemap/robots/metadata;
- legal/privacy/refund/subscription/upload terms matching actual behavior;
- accessibility;
- performance;
- 404/500/error states;
- owner documentation and routine admin workflows.

Do not call a site production-ready merely because Vercel deployed it successfully.
