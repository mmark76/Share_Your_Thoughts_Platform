# ADR-006: File Responsibility and Size

**Status:** Accepted  
**Date:** 2026-06-21

## Context

Large files and mixed responsibilities increase the risk of uncontrolled changes and repeated patches.

## Decision

- Each file and component has one clear primary responsibility.
- Approximately 100–200 lines is an early warning for many component files, not an absolute limit.
- Split a file when it gains multiple responsibilities, duplication or unsafe complexity.
- `page.tsx` composes components rather than containing the entire page implementation.
- Each CSS Module concerns its associated component.
- Refactoring remains focused and separate from unrelated features where practical.

## Consequences

Changes can remain local, reviewable and easier to test.
