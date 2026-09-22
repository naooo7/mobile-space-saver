# FastLearner mobile space optimization

## Scope
- Bring the existing FastLearner repository into this workspace unchanged as the starting point, preserving its routes, data, learning logic, analytics, themes, and Liquid Glass styling.
- Make mobile-only density improvements, with desktop spacing retained at existing breakpoints.

## Changes
- Compact the Drill screen’s title spacing, section gaps, surfaces, numbered headings, settings groups, summary, and start area on small screens only.
- Replace tall Choose Material rows on phones with a compact two-column selection grid where labels fit, falling back safely for narrow or long content.
- Keep every selection visibly distinct and maintain at least comfortable 44px interaction heights.
- Apply the same small-screen spacing treatment only to closely related Learn material and subtest lists where existing whitespace is excessive.
- Reuse the current `Surface`, `LinkRow`, buttons, checkboxes, switches, and Liquid Glass classes; create no duplicate components.

## Verification
- Check Drill and Choose Material at 360px, 390px, and 430px for reduced scrolling, clear selection states, touch comfort, clipping, and horizontal overflow.
- Check desktop remains comfortably spaced.
- Exercise Light, Dark, and System themes and inspect browser console/runtime diagnostics.
