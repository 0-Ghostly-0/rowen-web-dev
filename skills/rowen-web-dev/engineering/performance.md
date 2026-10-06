# Performance

Measure before optimizing.

Use real evidence such as browser performance tools, bundle analysis, field/lab Core Web Vitals, server timings or profiling.

Prioritize user-visible bottlenecks:
- LCP/media/font delivery;
- interaction latency and expensive main-thread work;
- layout instability;
- excessive JS/bundle size;
- avoidable waterfalls;
- unnecessary client rendering;
- inefficient queries/API fanout.

Do not add caching, memoization, lazy loading or complexity without a plausible measured reason.

Reserve media dimensions, optimize critical assets, and prefer server/platform capabilities when they reduce shipped client JavaScript without harming UX.
