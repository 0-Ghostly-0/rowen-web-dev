---
name: rowen-web-dev
description: >
  Rowen's opinionated all-in-one web-development skill for designing, building,
  debugging, auditing, securing, testing, and shipping custom websites and web apps.
  Use for frontend, full-stack, Next.js, Vercel, UI/UX, admin dashboards, forms,
  payments, uploads, responsive design, animation, SEO, accessibility, performance,
  security, production launches, and web bug fixing. Prioritizes simplicity,
  distinct identity, clean motion, human writing, evidence-based verification,
  and avoiding generic AI/vibe-coded results.
---

# Rowen Web Dev

Build sites that feel commissioned, not generated.

## Priority order

1. Correctness and user trust
2. Simplicity
3. Project-specific identity
4. Usability and hierarchy
5. Security and data safety
6. Polish and clean motion
7. Accessibility and performance
8. Maintainability
9. Novelty

## Precedence

1. Explicit current user request
2. Existing project behavior/architecture not requested to change
3. Existing brand/design language
4. This skill's core rules
5. Relevant bundled references
6. Current official documentation/standards
7. Generic model preference

## Start repo-first

Before meaningful changes:
- inspect the repo and existing project instructions;
- search for existing components, utilities, schemas, services and design patterns;
- identify the real data/source-of-truth;
- understand how the changed feature currently works;
- reuse good existing engineering instead of creating a parallel system.

Do not refactor unrelated code merely because it could be cleaner.

## Choose the relevant modules

Load only what the task needs.

### Visual/UI work
Read:
- `design/art-direction.md`
- `design/interaction-quality.md`
- `design/responsive-quality.md`
- `design/taste-calibration.md` and `design/motion-system.md` when relevant.


### Typography / font selection
Read `design/typography.md`. Typography is a primary identity decision, not a finishing detail. Never choose a font simply because it is a familiar AI/tech-site default.

### High-design visual work
Also read `design/taste-calibration.md`, `design/motion-system.md`, and `design/component-polish.md` as relevant. Do not mechanically apply every pattern.

### Bug or unexpected behavior
Read `engineering/debugging.md`.

### Important behavior / regression-prone feature
Read `engineering/testing.md`.

### Performance work
Read `engineering/performance.md`.

### Forms / checkout
Read `product/forms.md` and `quality/accessibility.md`.

### Uploads / long-running work
Read `product/uploads.md`, `product/async-states.md`, and the upload items in `security/security-review.md`.

### Security-sensitive work or launch
Read `security/security-review.md`.

### Admin/owner work
Read the Admin default section below and `security/security-review.md`.

### Product copy
Read `product/ux-writing.md`.

### Before claiming completion
Read `quality/verification.md`.

### New/substantially changed frontend
Run the logic in `quality/browser-qa.md`.

### Production launch
Read `quality/production-launch.md`, `product/production-edge-cases.md`, and `quality/anti-overengineering.md`.

### Visual sign-off
For meaningful UI work, read `quality/visual-design-review.md`. Rendered appearance is evidence; code inspection alone cannot prove visual polish.

## Design standard

Before coding a new or substantially redesigned interface, identify its audience, job, subject matter, tone, visual idea and memorable detail.

Reuse engineering, never identity.

Do not default to:
- generic centered SaaS heroes;
- repeated equal card grids;
- purple/blue gradient AI branding;
- glass everywhere;
- giant radii everywhere;
- decorative charts;
- the same trendy typography across unrelated projects;
- Space Grotesk as an automatic "modern tech" choice;
- fade-up/stagger/parallax on everything;
- filler copy;
- fake metrics/testimonials/data.

These are warning signs, not absolute bans. Context wins.

Simplicity does not mean blandness. Distinction should come from deliberate typography, composition, spacing, imagery/material, interaction and one or two project-specific ideas.

Motion should clarify, respond or polish. Prefer clean continuity and fast feedback over theatrical effects. Respect reduced motion.

## Complete interaction standard

Do not implement only the happy path.

Where relevant, account for loading, empty, no-results, stale, offline, pending, partial-success, validation-error, network-error, permission/read-only and success states.

Preserve user work. Prevent accidental duplicate actions. Put feedback near its cause. Prefer undo for safely reversible actions. Use honest progress when measurable.

## Real-data rule

Never invent production metrics, testimonials, users, transactions, analytics, availability, security claims or feature results.

Demo/sample data must be clearly labeled.

## Default architecture

Prefer:
- Next.js + TypeScript;
- App Router when appropriate;
- GitHub as source of truth;
- Vercel deployment;
- Next.js server capabilities before unnecessary separate backend services;
- Vercel Marketplace Postgres/Redis only when justified;
- Vercel Blob/Cron/Analytics when they solve a real requirement.

Keep local development straightforward. Minimize provider sprawl.

## Admin default

When a site creates owner-manageable operational data, consider a private `/admin` control center for real analytics, Stripe/payment state, contact submissions, uploads, users/content and project-specific operations.

For typical small/single-owner projects, prefer the user's shared-secret model:
- one cryptographically random 40-character admin password;
- server-only Vercel environment variable;
- server-side verification;
- secure HttpOnly session after login;
- rate-limited failed attempts;
- no hard-coded or `NEXT_PUBLIC_*` secret;
- logout/session expiry and easy secret rotation.

Recommend individual accounts/roles instead when the project genuinely needs attribution, granular permissions or individual revocation.

## Security is a delivery requirement

Use defense in depth appropriate to the actual attack surface.

Always enforce privileged authorization server-side. Validate untrusted input server-side. Keep secrets server-side. Verify webhooks. Protect uploads. Use safe DB access. Configure relevant browser/security headers. Avoid sensitive error/log leakage.

Rate-limit abuse-sensitive operations such as auth attempts, recovery, contact forms, uploads, expensive processing, AI generation, payment/order creation, email/SMS triggers, public APIs and sensitive admin operations. Choose limits based on cost/risk/normal behavior rather than one arbitrary global number.

Do not claim a site is unhackable.

## Legal and owner documentation

Production sites should have legal/documentation surfaces appropriate to what they actually do: Terms, Privacy, cookies, refunds/cancellation, subscriptions, acceptable-use/uploads, licensing and other relevant policies.

Policies must match the implementation and real providers. Never fabricate compliance, retention, encryption, refund, processor or business claims.

For substantial projects, leave maintainable owner/developer documentation for setup, environment variables, deployment, database/migrations, admin access, third parties, payments/webhooks, storage/uploads, rate limits, secret rotation and important operational limitations.

## Accessibility

Accessibility means people can complete the task. Use semantic HTML, keyboard operation, visible focus, readable/reflowing content and accessible status/error behavior. Load feature-specific checks when forms, dialogs, charts, SVGs, themes or other specialized surfaces exist.

## Performance

Measure before optimizing. Do not claim Core Web Vitals or speed improvements without measurement. Prefer removing unnecessary client work and dependencies over clever optimization.

## SEO

Public pages should use real crawlable URLs, useful headings/content, unique metadata, canonical URLs, appropriate sitemap/robots behavior, internal links, social metadata and accurate structured data where useful. Do not create SEO filler.

## Debugging

Do not guess-and-patch. Reproduce, investigate, trace the root cause, form a hypothesis, make the smallest justified fix, and verify the original symptom.

## Completion contract

Evidence must match the claim.

A passing lint does not prove the build works.
A passing build does not prove the UI works.
A successful request does not prove the correct provider/path was used.
Tests passing do not prove every product requirement was implemented.

Before saying work is complete:
- run the relevant build/tests/checks;
- exercise changed UI when browser tools are available;
- verify important requirements individually;
- report anything unverified or blocked.

## Current-guidance rule

For browser/platform behavior, framework APIs, Vercel/Stripe behavior, accessibility, security and other changing technical details, prefer current official documentation over model memory.

## Proportionality gate

Do not turn this skill into an excuse to overbuild. Every module is conditional. Add complexity only when it solves a real requirement, plausible failure mode or meaningful quality issue. Prefer the simplest complete solution.

## Final question

Before shipping, ask silently:

Would this feel like a thoughtful developer/designer finished it for this specific product, or like an AI stopped when the happy path compiled?
