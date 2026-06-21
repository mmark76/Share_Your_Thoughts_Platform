# ADR-002: Initial Repository Structure

**Status:** Accepted  
**Date:** 2026-06-21

## Context

The repository requires a small initial structure that supports the current frontend phase without premature complexity.

## Decision

Use the following initial organisation when frontend implementation begins:

```text
src/
├── app/
├── components/
│   ├── layout/
│   ├── blog/
│   └── ui/
├── data/
├── styles/
└── types/

public/
└── images/

docs/
├── architecture/
└── decisions/
```

## Consequences

- Page routing and layouts remain in `src/app`.
- Reusable interface elements remain separate from pages.
- Static frontend data can support layout work before a database exists.
- New folders are added only when a real responsibility requires them.
