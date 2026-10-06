# Async and Data States

Design the complete state model, not only success.

Consider:
- initial/loading;
- refreshing/stale;
- empty;
- filtered/no results;
- partial success;
- retryable error;
- permanent/validation error;
- offline/disconnected;
- pending mutation;
- success;
- permission/read-only.

Keep local updates local: updating one panel should not unnecessarily blank the whole page.

Use optimistic UI only when rollback is safe and understandable.
