# Component Polish

Use this as a reasoning checklist, not a mandate to add every behavior.

## Navigation
- current location is apparent;
- mobile behavior is designed, not squeezed;
- active/hover/focus states are distinct;
- menus close predictably and restore focus where relevant;
- back/forward/deep links preserve meaningful state.

## Buttons and actions
- visual hierarchy matches consequence/frequency;
- pending state prevents accidental duplicates;
- destructive actions are visually and behaviorally distinct;
- icon-only actions have accessible names/tooltips when meaning is not obvious;
- hover animations transition smoothly both into and out of hover rather than snapping back;
- success/error feedback appears near the action when useful.

## Search
- useful empty query state;
- loading/no-results/error are distinct;
- query/filter state should be URL-backed when sharing/back-navigation benefits;
- preserve query on recoverable errors;
- clear button and keyboard behavior should work naturally.

## Filters
- active filters are visible;
- reset is easy;
- result count/change is understandable;
- mobile filter UI remains usable;
- avoid hidden filter state users cannot discover.

## Tables/data lists
- alignment follows data type;
- numbers align consistently;
- sticky headers when they materially improve long tables;
- sorting communicates direction;
- loading/empty/error/permission states;
- overflow strategy on narrow screens;
- row actions do not become mystery icon soup;
- pagination/infinite loading preserves context.

## Tabs
- tabs represent peer views, not arbitrary navigation;
- active state is obvious;
- keyboard semantics work;
- changing tabs should not unexpectedly destroy unsaved work.

## Dialogs/drawers/popovers
- focus enters/restores correctly;
- Escape/outside-click behavior matches consequence;
- background interaction/scroll is controlled;
- destructive dialogs state the consequence;
- mobile viewport/keyboard does not hide controls.

## Settings
- group by mental model;
- show saved/pending/error state;
- avoid a Save button when changes are actually immediate;
- warn about unsaved changes only when there is truly something to lose;
- irreversible settings need clear consequence.

## Notifications/toasts
- use for transient confirmation, not essential instructions;
- do not hide actionable errors only in a disappearing toast;
- avoid toast spam for every routine interaction.

## Onboarding
- get users to meaningful value quickly;
- ask for setup information only when needed;
- allow skipping optional education;
- preserve progress where setup is substantial;
- empty states can teach better than a forced tour.

## Checkout
- price/recurrence/fees are clear before commitment;
- prevent duplicate purchase attempts;
- distinguish pending payment from success;
- handle declined/abandoned/retried payment;
- never claim success only from a client redirect when server/webhook truth matters.
