# Interaction Quality: The Details Users Miss Until They're Gone

## Every action answers back
Give immediate, proportional feedback for presses, selections, drag/drop, saves and mutations. Keep feedback near the action.

## Honest progress
Use determinate progress when meaningful progress is known. Percent, item count, stage, transfer rate, or defensible ETA can reduce uncertainty. Never invent progress.

## Retry and resume
Preserve completed work when technically feasible. Retry from safe checkpoints, expose recovery, distinguish retryable from permanent failures, and avoid duplicate mutations.

## Upload UX
Consider drag-over feedback, click-to-browse, type/size guidance, validation, preview, filename/type/size, per-file progress, per-file success/failure, retry/remove, cancellation, resumability for large files, duplicate behavior, network loss, and accessible status announcements. Multi-file uploads should not become one opaque all-or-nothing state unless the product truly requires that.

## Preserve work
Keep entered values after errors. For long work, consider autosave/drafts or unsaved-change handling. Prefer undo over confirmation when an action is safely reversible.

## Stable loading
Skeletons/placeholders should resemble final geometry. Reserve image/media dimensions. Avoid full-screen loading for local work and avoid flashing loaders for near-instant operations.

## Empty/error states
Distinguish first-use empty, true empty, no-results, filtered-empty and permission-empty. Errors should identify the affected thing, use human language, preserve work, and provide recovery when possible.

## Focus/keyboard/overlays
Keyboard access and visible focus are mandatory. Dialogs should manage entry/return focus, scrolling and Escape behavior appropriately. Sticky UI must not obscure focused controls.

## Mobile
Use semantic input types, autofill/password-manager support, comfortable targets, no hover dependency, and test software keyboard overlap, safe areas and overflow.

## Data/admin surfaces
Use scannable alignment, useful statuses/timestamps, persistent filters where helpful, clear bulk selection, and recoverable failures. Do not use charts when a number or table answers the owner's question better.

## Quiet polish
Consider, only when useful: stable scrollbar gutters, stable image aspect ratios, tooltips for unfamiliar icon-only controls, temporary copied confirmation, access to truncated full values, sticky table headers, URL-backed filters, scroll-position restoration, safe optimistic UI with rollback, and stale/offline indicators.

The goal is not more effects. It is fewer tiny moments of uncertainty, lost work and friction.
