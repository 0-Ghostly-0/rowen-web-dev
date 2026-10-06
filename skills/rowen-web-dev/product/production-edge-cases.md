# Production Edge Cases

Do not build every edge case preemptively. Identify the ones plausible for the feature's cost, risk and data model.

## Persistence
Consider:
- duplicate requests;
- stale writes/concurrent edits;
- partial failure;
- retries after timeout;
- refresh/navigation mid-operation;
- idempotency for important mutations.

## Payments
Where applicable:
- client success vs authoritative webhook/server state;
- duplicate webhook delivery;
- out-of-order events;
- payment pending/failed/refunded/disputed/canceled;
- duplicate checkout/order creation;
- currency/minor units;
- subscription renewal/cancellation timing.

## Sessions/auth
Consider:
- expired session during a form/action;
- revoked/rotated admin secret;
- multi-tab logout;
- permission changed while page is open;
- redirect-back after login when safe.

## Uploads/files
Consider:
- invalid/misleading MIME;
- oversized file;
- same-name files;
- network interruption;
- partial multi-file failure;
- retry/resume support;
- abandoned/orphaned uploads;
- deleted/missing underlying object;
- private file authorization.

## Time/data formatting
Use explicit timezone/currency/locale semantics when the product depends on them. Avoid silently assuming the developer's local timezone.

## Lists
Consider zero, one, many and very-many records; pagination; deleted records; stale filters; long names; missing values.

## External services
Handle plausible timeout, rate limit, malformed response, temporary outage and webhook/API retry without pretending the external service is perfectly reliable.
