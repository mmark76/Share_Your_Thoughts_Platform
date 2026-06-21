# ADR-001: Frontend Technology

**Status:** Accepted  
**Date:** 2026-06-21

## Context

The current phase concerns only the visual design and frontend layout of the Blog App. The frontend must remain modular and capable of connecting to future backend services without implementing them now.

## Decision

Use:

- Next.js,
- React,
- TypeScript,
- App Router.

The browser output remains standard HTML, CSS and JavaScript. React components are written with TSX, and TypeScript is compiled to JavaScript.

## Consequences

- Pages and layouts follow the Next.js App Router model.
- The interface can be divided into small reusable components.
- Type checking can identify many mistakes before runtime.
- No backend, database, authentication or Social Platform functionality is introduced by this decision.
