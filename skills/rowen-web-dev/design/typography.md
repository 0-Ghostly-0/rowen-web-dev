# Typography as Project Identity

Typography is one of the strongest signals that a site was designed for a specific product rather than generated from a familiar template.

## Never choose by AI default

Do not repeatedly reach for the same fashionable sans-serif across unrelated projects.

Space Grotesk is a specific warning sign for this workflow because it is strongly associated by the user with generic "vibe-coded" modern-tech sites. It is not banned. Use it only when there is a concrete project-specific reason and it genuinely fits better than alternatives.

Apply the same skepticism to any font that becomes an automatic model habit.

## Choose from the product outward

Before selecting type, identify:
- brand personality;
- subject/industry;
- audience;
- amount and type of reading;
- interface density;
- editorial vs application feel;
- seriousness/playfulness;
- historical/cultural references when relevant;
- whether typography should be quiet infrastructure or a memorable visual feature.

Then deliberately choose the typography direction.

Possible directions include:
- grotesk / neo-grotesk;
- humanist sans;
- geometric sans;
- serif/editorial;
- slab;
- condensed/display;
- monospaced/technical;
- mixed serif + sans;
- custom/brand type when supplied.

These are categories to reason from, not a required menu.

## Avoid font monoculture

Across separate client/projects, vary typography when their identities differ.

Do not make every site:
- one geometric/grotesk sans;
- oversized bold hero text;
- tight tracking;
- tiny uppercase eyebrow;
- medium-weight body;
- identical button typography.

Those choices can be good individually. Repetition across unrelated work creates the recognizable AI/template fingerprint.

## Build a type system, not a font picker

Define roles:
- display/hero;
- heading;
- body;
- UI/control;
- label/meta;
- numeric/data;
- code/technical when needed.

One family can fill all roles if its range is strong. Multiple families should have a reason.

Tune:
- size;
- weight;
- line height;
- letter spacing;
- measure/line length;
- casing;
- optical size/features when supported;
- numeric styles where data matters.

Hierarchy should remain clear even if color and containers are removed.

## Font pairing

Pair by useful contrast and compatible purpose, not because a blog calls two fonts a "perfect pair."

Good contrast may come from:
- serif vs sans;
- wide vs narrow;
- expressive display vs quiet text;
- editorial headline vs utilitarian UI.

Avoid two families that compete for attention without creating hierarchy.

## Technical quality

- Use licensed/legitimate font sources.
- Prefer WOFF2 for self-hosted web fonts.
- Subset only when it will not remove needed language/glyph coverage.
- Avoid loading weights/styles that are never used.
- Use `font-display` behavior appropriate to the product.
- Define sensible fallback stacks with reasonably compatible metrics.
- Reserve layout and avoid typography-driven CLS where practical.
- Verify the font actually loaded; do not approve screenshots unknowingly rendered in fallback.
- Test punctuation, numbers, symbols, long names, lowercase/uppercase and real content.
- Test at mobile sizes and high zoom.
- Keep body text comfortably readable.

## Variable fonts

Use variable fonts when their flexibility/performance tradeoff benefits the project, not merely because they are modern.

When supported and useful, axes such as weight, width, slant or optical size can create a more custom system without adding many separate files.

## Product/data typography

For dashboards, pricing, financial data, timers or changing numeric values:
- consider tabular numerals when alignment matters;
- distinguish labels from values clearly;
- avoid display fonts that make dense data hard to scan.

## Distinctive does not mean obscure

Do not choose an unreadable or poorly supported font merely to avoid looking AI-generated.

A common font used with excellent art direction can be better than a rare font used badly.

The goal is intentionality and project fit.

## Typography review

Before shipping, ask:
1. Why does this font belong to this specific product?
2. Would I have chosen the same font automatically for an unrelated AI/SaaS project?
3. Does the type system still have hierarchy without card borders and color?
4. Does real content look good, not only the hero headline?
5. Did the intended web font actually load?
6. Is body copy comfortable on mobile?
7. Are numbers/data handled appropriately?
8. Does this typography make the project more identifiable?

If the only explanation is "it looks modern," reconsider the choice.
