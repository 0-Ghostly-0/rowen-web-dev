# Motion System

Motion is behavior, not decoration.

## Priority
1. Immediate control feedback.
2. Spatial/state continuity.
3. Enter/exit clarity.
4. Meaningful emphasis.
5. Decorative delight only when it genuinely fits.

## Frequency
Frequently repeated interactions should generally be faster and quieter than rare/high-consequence moments.

Do not make common navigation wait for animation.

## Continuity
When an object changes state/location, prefer continuity that helps the user understand what happened over unrelated fade-outs/fade-ins.

Menus, popovers, drawers and dialogs should feel attached to their trigger/context when appropriate.

## Timing
Avoid one universal duration. Tiny feedback can be very fast; larger spatial transitions can take longer. Judge by perceived distance, frequency and importance.

Never copy timing numbers mechanically from another skill.

## Easing
Use easing that supports the physical/state change. Avoid bounce/elastic motion unless the brand specifically calls for playful physicality.

## Hover/press
Do not make every card lift, scale and shadow. Hover should communicate affordance or reveal something useful. Pressed states should feel immediate.

## Bidirectional hover transitions

Hover motion must have a polished exit as well as an entrance.

If an element smoothly changes on hover, it should normally transition smoothly back to its resting state when the pointer leaves. Do not let animated properties snap instantly back unless that abrupt reset is a deliberate interaction decision.

This applies to properties/effects such as:
- transform, scale, rotation and position;
- opacity;
- background/color;
- borders;
- shadows;
- blur/filter;
- icon movement;
- underline/accent movement.

Prefer defining the transition on the base/resting element rather than only on `:hover`, so both hover-in and hover-out are animated.

The return animation may be slightly faster or quieter than the entrance when that feels more responsive, but it should preserve continuity.

During QA, explicitly test both entering and leaving hover states.

## Loading
Do not animate merely to prove the page is alive. Prefer stable geometry and honest state changes.

## Reduced motion
Reduced-motion mode should preserve meaning while removing unnecessary movement, not simply break transitions.

## Performance
Prefer transform/opacity for frequent visual motion when practical. Avoid expensive continuous effects without a reason.

## Motion QA
Check:
- interruption/repeated clicking;
- rapid open/close;
- route changes;
- focus behavior;
- reduced motion;
- mobile/touch;
- whether animation delays the task;
- whether state is still understandable with motion removed.
