# Project Context

**Project Name:** Share Your Thoughts  
**Tagline:** A social blogging platform.  
**Project Owner:** Markellos Markides  
**Repository:** `mmark76/Share_Your_Thoughts_Platform`  
**Repository Visibility:** Private  
**Document Version:** 1.1  
**Last Updated:** 2026-06-21  
**Status:** Active  

---

## 1. Purpose of This Document

This document preserves the essential context, decisions, current state and next steps of the project.

It must allow the project to continue correctly even when:

- a previous conversation is unavailable,
- work resumes after a long interruption,
- development moves between ChatGPT, GitHub, VS Code or Codex,
- a new development session begins without access to earlier discussions.

This document must be read together with:

```text
GENERAL_SOFTWARE_PROJECT_GUIDE.md
```

The general guide defines the common architectural and development principles for all software projects. This document records the specific context of this project.

---

## 2. Project Overview

“Share Your Thoughts” is an independent custom software project.

The complete long-term concept includes two distinct but connected products:

1. A platform for creating and hosting personal blogs.
2. A separate social platform for sharing, discovering, following and discussing published articles.

The social platform will not primarily host the complete articles. It will mainly operate as a network for article sharing and discovery.

---

## 3. Current Project Priority

The current priority is exclusively the first product:

> A custom application that allows users to create, manage and host a normal personal blog without requiring technical knowledge, separate hosting or installation of a CMS.

The separate social platform is deferred to a later project phase.

It must not influence or unnecessarily complicate the current implementation.

---

## 4. Current Development Phase

The project is currently in the visual design and frontend layout phase.

For the present phase, work focuses only on:

- visual identity,
- page structure,
- layout,
- responsive design,
- reusable visual components,
- typography,
- colours,
- spacing,
- navigation,
- article presentation,
- blog homepage appearance.

The following are not currently being implemented:

- backend,
- database,
- authentication,
- user registration,
- article publishing logic,
- administration system,
- APIs,
- comments,
- notifications,
- social platform functionality.

These will be designed and implemented in later controlled phases.

---

## 5. Current Core Product Flow

The future core user flow is expected to be:

```text
Register
→ Create Blog
→ Write Article
→ Publish
→ Manage Blog
```

This flow is contextual information only during the current layout phase. Its functional implementation has not yet begun.

---

## 6. Product Principles

The application will be:

- custom-built,
- independent,
- secure,
- maintainable,
- modular,
- extensible,
- suitable for long-term development.

The application will not be based on an existing CMS or social-networking platform such as:

- WordPress,
- BuddyPress,
- Flarum,
- Mastodon,
- another ready-made blogging or social platform.

Established programming languages, frameworks, libraries, databases, services and development tools may be used.

The distinction is:

> Established technical tools may be used, but the product itself must not depend on a ready-made CMS or social platform as its foundation.

---

## 7. Authentication Decision

The future primary authentication method will be:

```text
Email + Password
```

The email address will serve as:

- the login identifier,
- the communication address,
- a verification mechanism.

It will not constitute proof of a person's real-world identity.

The project currently does not require:

- identity documents,
- electronic identification,
- KYC,
- verification of a person's legal identity.

The platform must not falsely describe users as having verified real identities.

---

## 8. Content Model Decision

The blog application will focus on normal articles.

Short social-style “Thoughts” are not currently part of the Blog App.

The Blog App and the future Social Platform must remain conceptually separate:

### Blog App

Hosts and presents the complete articles.

### Social Platform

Shares links to articles and supports discovery and interaction.

---

## 9. Artificial Intelligence Boundaries

The application may provide:

- common formatting tools,
- basic editing support,
- spell-checking.

It must not automatically:

- rewrite the author's text,
- change the author's meaning,
- alter the author's writing style,
- replace titles,
- transform personal expression without explicit user action.

The author must retain control of the content.

---

## 10. Architecture Principles

The project must follow:

```text
GENERAL_SOFTWARE_PROJECT_GUIDE.md
```

The most important project-specific architectural requirements are:

- small files,
- one clear responsibility per file,
- modular structure,
- component-based frontend,
- feature-based organisation as functionality grows,
- low coupling,
- localised changes,
- no oversized HTML, CSS or JavaScript files,
- no accumulation of fixes and patches,
- no premature overengineering,
- gradual and controlled expansion.

The architecture must make it possible to modify a small part of the project without analysing or rewriting unrelated large files.

---

## 11. File Size and Responsibility

Files should generally remain small enough to be:

- easily understood,
- safely edited through ChatGPT or GitHub,
- reviewed through a clear diff,
- handled with limited Codex usage,
- changed without requiring full-repository context.

Approximately 100–200 lines may be used as an early warning for many component files, but this is not an absolute limit.

The real rule is:

> A file must be divided when it develops multiple responsibilities or becomes difficult to understand and modify safely.

---

## 12. Current Repository Strategy

The repository is:

```text
mmark76/Share_Your_Thoughts_Platform
```

It is currently private.

For the current phase, the repository should remain focused on the Blog App and its frontend layout.

The future Social Platform must not be added prematurely. A later decision will determine whether it belongs in:

- a separate repository,
- a larger workspace,
- or a carefully designed monorepo.

---

## 13. Development Tools

Currently available tools include:

- ChatGPT Plus,
- Codex through the available ChatGPT plan,
- GitHub,
- Visual Studio Code,
- GitHub Desktop,
- existing VS Code plugins,
- Hetzner infrastructure.

No other paid AI agent is assumed to be available.

The project architecture must therefore remain manageable without dependence on additional paid AI services.

---

## 14. Working Method

For the current phase, most planning, architecture and code preparation will take place inside ChatGPT conversations.

VS Code will be used when needed for:

- opening the local repository,
- editing real files,
- running the project,
- testing,
- debugging,
- previewing the layout.

GitHub Desktop will be used for:

- cloning repositories,
- creating and switching branches,
- viewing changes,
- committing,
- pulling,
- pushing,
- synchronising with GitHub.

ChatGPT may also work directly with the GitHub repository when access and the required operation are available.

---

## 15. Git Workflow

Important changes should normally follow this workflow:

```text
Create Branch
→ Make Focused Changes
→ Review Diff
→ Test
→ Commit
→ Pull Request
→ Review
→ Merge
```

Each change should have a limited and clearly defined scope.

Refactoring, new functionality, styling changes and bug fixes should not be mixed unnecessarily in the same commit or Pull Request.

---

## 16. Project Management Method

The project will follow a tailored hybrid approach:

- PMI-based governance and documentation,
- iterative and incremental software delivery,
- Agile principles where suitable,
- controlled decisions and documented changes.

Project roles are currently held by Markellos Markides:

- Project Sponsor,
- Project Owner,
- Project Manager.

The project is currently personal and does not have an external development team.

---

## 17. Stakeholders

The initial stakeholders are:

- Markellos Markides,
- his family,
- his friends,
- future blog creators,
- future readers,
- the future platform community.

---

## 18. Infrastructure Context

The project may use existing Hetzner infrastructure.

However, it must maintain:

- its own identity,
- its own domain,
- technical separation,
- configuration separation,
- deployment separation,
- appropriate security boundaries.

It must remain independent from the Markellos Ecosystem even when underlying physical infrastructure is shared.

---

## 19. Current Visual Direction

A visual mockup has already been created for a polished personal blog homepage.

The design direction includes:

- clean and modern layout,
- strong article presentation,
- header and navigation,
- hero content,
- latest article cards,
- author information,
- categories,
- sidebar content,
- footer,
- responsive behaviour.

The mockup is a design reference, not yet the final implementation specification.

---

## 20. Current Decisions

The following decisions are currently approved:

1. The current implementation concerns only the Blog App.
2. The current phase concerns only visual design and frontend layout.
3. The Social Platform is deferred.
4. The product will be custom-built.
5. The repository is private.
6. The architecture will be modular and component-based.
7. Files will remain small and focused.
8. Large central HTML, CSS and JavaScript files will be avoided.
9. ChatGPT Plus and Codex are the only assumed paid AI tools.
10. VS Code and GitHub Desktop are already installed.
11. Work will initially be conducted mainly through ChatGPT.
12. Important repository changes will use branches and Pull Requests where appropriate.
13. The general software project guide applies to this project.
14. The frontend technology is Next.js with React, TypeScript and the App Router.
15. The initial repository structure uses `src/app`, organised component folders, shared data, styles and types, `public/images`, and project documentation.
16. Components are initially organised into `layout`, `blog` and `ui` responsibilities.
17. Styling uses CSS Modules, limited global CSS and central design tokens, without Tailwind CSS in the initial phase.
18. Naming conventions use PascalCase for components, matching CSS Module names, camelCase for functions and variables, and clear lowercase folder names.
19. Each file has one clear responsibility; approximately 100–200 lines is an early warning rather than an absolute limit.
20. The homepage will be implemented incrementally, component by component, followed by responsive and architectural verification.

The detailed records of decisions 14–20 are maintained in `docs/decisions/`.

---

## 21. Decisions Not Yet Finalised

The following matters remain open and must not be assumed without explicit approval:

- package manager,
- testing framework,
- component library policy,
- exact design-token file format,
- detailed build and quality-tool configuration,
- backend technology,
- database,
- deployment architecture,
- final domain,
- social platform repository strategy.

---

## 22. Immediate Next Step

After the approved documentation and Architecture Decision Records are committed, create a focused frontend implementation branch and:

1. scaffold the Next.js project with React, TypeScript and the App Router,
2. apply the approved initial folder structure,
3. add the first shared layout components,
4. verify that the project runs before visual implementation continues.

The first implementation remains frontend-only. No backend, database, authentication or Social Platform functionality is included.

---

## 23. Continuity Instructions

At the beginning of a new development session:

1. Read `GENERAL_SOFTWARE_PROJECT_GUIDE.md`.
2. Read this `PROJECT_CONTEXT.md`.
3. Inspect the current repository state.
4. Confirm the active branch and latest commit.
5. Review recent decisions and open items.
6. Identify the exact next approved task.
7. Do not make unapproved architectural changes.
8. Do not silently reinterpret earlier decisions.
9. Update this document when an approved decision materially changes the project.

---

## 24. Source of Truth

The sources of truth, in order, are:

1. the current approved state of the real repository,
2. the latest approved `PROJECT_CONTEXT.md`,
3. the `GENERAL_SOFTWARE_PROJECT_GUIDE.md`,
4. approved Architecture Decision Records,
5. approved project-management documents,
6. explicit instructions from Markellos Markides.

When sources conflict, the conflict must be reported and resolved before implementation continues.
