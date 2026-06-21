# ADR-003: Component Organisation

**Status:** Accepted  
**Date:** 2026-06-21

## Context

The homepage must not become one large file. Visual elements require clear responsibilities and predictable locations.

## Decision

Begin with three component groups:

```text
components/
├── layout/
│   ├── Header.tsx
│   ├── Navigation.tsx
│   ├── Sidebar.tsx
│   └── Footer.tsx
├── blog/
│   ├── HeroArticle.tsx
│   ├── ArticleCard.tsx
│   ├── ArticleGrid.tsx
│   ├── AuthorProfile.tsx
│   └── CategoryList.tsx
└── ui/
    ├── Button.tsx
    └── Tag.tsx
```

These filenames describe the initial plan rather than a requirement to create every component immediately.

## Consequences

- Layout, blog-specific and general UI responsibilities remain separated.
- Components are created incrementally when required.
- Code used by only one feature is not moved prematurely into shared areas.
