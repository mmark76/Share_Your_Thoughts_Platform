# ADR-005: Naming Conventions

**Status:** Accepted  
**Date:** 2026-06-21

## Context

Consistent naming reduces ambiguity and makes files easier to locate and maintain.

## Decision

- Components and component files use PascalCase, for example `ArticleCard.tsx`.
- CSS Modules use the matching component name, for example `ArticleCard.module.css`.
- Functions and variables use camelCase, for example `formatArticleDate`.
- Folders use clear lowercase names, for example `components/blog`.
- Names must describe responsibility.
- Avoid vague names such as `helpers`, `misc`, `stuff`, `temp`, `final`, `new`, `fix` and `updated`.

## Consequences

The repository remains predictable and searchable as it grows.
