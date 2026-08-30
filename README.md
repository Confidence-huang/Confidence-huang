# Confidence Huang

<p align="center">
  Evidence-first systems · Agent Skills · Practical workflow software
</p>

I build small, inspectable systems that turn messy work into clear next actions: tools that govern agent capabilities, workflows that validate research and Office artifacts, and software that keeps career-service work inside explicit boundaries.

## Start here

| If you want to… | Start with |
| --- | --- |
| Build and validate research or Office artifacts | [`academic-workstation`](https://github.com/Confidence-huang/academic-workstation) |
| Write a source-preserving paper in LaTeX or Word | [`academic-paper-workflow`](https://github.com/Confidence-huang/academic-paper-workflow) |
| Produce and validate an editable PowerPoint deck | [`academic-ppt-workflow`](https://github.com/Confidence-huang/academic-ppt-workflow) |
| Govern Skill and plugin lifecycles across Windows and Linux | [`skill-lifecycle-manager`](https://github.com/Confidence-huang/skill-lifecycle-manager) |
| Turn accessible videos into Chinese learning material | [`bilibili-douyin-video-learning`](https://github.com/Confidence-huang/bilibili-douyin-video-learning) |
| Explore a career-service product from story to service boundary | [`careerpathdesk-website`](https://github.com/Confidence-huang/careerpathdesk-website) → [`careerpathdesk-frontend`](https://github.com/Confidence-huang/careerpathdesk-frontend) → [`careerpathdesk-backend`](https://github.com/Confidence-huang/careerpathdesk-backend) |

## Public project map

### Academic artifact workflows

| Project | What it does |
| --- | --- |
| [`academic-workstation`](https://github.com/Confidence-huang/academic-workstation) | Shared routing, structural checks, native acceptance, PDF/visual QA, evidence and recovery contracts for research and Office artifacts. |
| [`academic-paper-workflow`](https://github.com/Confidence-huang/academic-paper-workflow) | Routes natural-language paper requests to source-preserving LaTeX or Word workflows, with citation, layout and visual-QA gates. |
| [`academic-ppt-workflow`](https://github.com/Confidence-huang/academic-ppt-workflow) | Routes presentation requests to editable PowerPoint workflows, followed by native round-trip and PDF/visual acceptance. |

Their shared shape is:

```text
request → route → build → structural QA → native roundtrip → PDF/visual QA → evidence
```

### Tools and learning workflows

| Project | What it does |
| --- | --- |
| [`skill-lifecycle-manager`](https://github.com/Confidence-huang/skill-lifecycle-manager) | Governs Skill and plugin inventory, verification, installation, updates, backups and evidence across Windows and Linux. |
| [`bilibili-douyin-video-learning`](https://github.com/Confidence-huang/bilibili-douyin-video-learning) | Turns accessible Bilibili and Douyin sources into structured Chinese notes, review material, action lists and Anki material while preserving platform and privacy boundaries. |

### CareerPathDesk

CareerPathDesk is split into clear public-facing, user-facing and service-facing boundaries:

```text
website  →  frontend  →  backend
介绍与演示    角色工作台     权限、事务与审计证据
```

| Repository | Responsibility |
| --- | --- |
| [`careerpathdesk-website`](https://github.com/Confidence-huang/careerpathdesk-website) | Product story and first-party demonstration entry point. |
| [`careerpathdesk-frontend`](https://github.com/Confidence-huang/careerpathdesk-frontend) | Vue 3 / TypeScript role-based workspaces for owners, staff and students. |
| [`careerpathdesk-backend`](https://github.com/Confidence-huang/careerpathdesk-backend) | Go / PostgreSQL service boundary for authorization, transactions and minimal audit evidence. |

## Common thread

- Evidence before claims: a status label should point to a reproducible check.
- Explicit boundaries: credentials, private data and production actions stay outside public examples.
- Source ownership: repair the authoritative source, then repeat the relevant validation gates.
- Human-readable workflows: the shortest useful path should be visible before implementation detail.

## Tools and languages

Python · Go · TypeScript · Vue · SQLite · PostgreSQL · LaTeX

This page highlights public repositories only; private work and private acceptance outputs are intentionally not listed here.
