# ADR-004: Styling Architecture

**Status:** Accepted  
**Date:** 2026-06-21

## Context

Styles must remain local, understandable and easy to change without creating one oversized stylesheet.

## Decision

- Use CSS Modules for component-specific styling.
- Use matching names such as `Header.tsx` and `Header.module.css`.
- Keep `globals.css` limited to resets and genuinely global rules.
- Define colours, spacing, typography and related design tokens centrally.
- Implement responsive behaviour with media queries.
- Do not use Tailwind CSS in the initial phase.
- Avoid inline styles except where a future technical requirement genuinely needs them.

## Consequences

- Component styles remain locally scoped.
- Design values can be changed consistently.
- CSS is still standard browser CSS.
