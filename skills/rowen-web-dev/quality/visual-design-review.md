# Visual Design Review

Rendered output is the product. Static code inspection is not enough to judge visual quality.

For meaningful UI changes, inspect real rendered pages when browser/screenshot tooling is available.

## Pass 1: hierarchy
Use a squint/thumbnail-level view:
- what is noticed first?
- is that correct?
- are sections grouped clearly?
- does everything compete equally?

## Pass 2: typography
Check:
- intended fonts actually loaded;
- hierarchy;
- measure/line breaks;
- awkward wrapping;
- body readability;
- numeric/data typography.

## Pass 3: geometry
Check:
- alignment;
- spacing rhythm;
- container widths;
- inconsistent control heights;
- accidental one-off radii/borders/shadows;
- image cropping/aspect ratio.

## Pass 4: identity
Ask:
- does this look specific to this product?
- what would remain identifiable if the logo disappeared?
- is there a generic AI/SaaS pattern dominating the page?
- did implementation dilute the original direction?

## Pass 5: states and responsiveness
Inspect narrow, tablet-like and wide layouts plus relevant hover/focus/loading/error/empty/disabled states.

## Pass 6: restraint
Identify anything that can be removed without losing clarity or identity.

## Reporting
Prioritize by visual impact:
- high: broken/unprofessional or hierarchy failure;
- medium: noticeably generic/inconsistent/unpolished;
- low: true finishing details.

Also identify what is working and should be preserved. Do not redesign merely to produce findings.
