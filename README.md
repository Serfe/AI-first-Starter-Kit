# AI-first Starter Kit

A lightweight, open-source reference for exploring AI-first software development with shared agents, skills, rules, and project context.

## What’s included

- Canonical agent roles, rules, and reusable workflows in `.agents/`
- Project context, requirements, and architecture decisions in `.ai/`
- Small adapters for Codex, Claude Code, and OpenCode
- An intentionally empty application extension point in `app/`

## Getting started

1. Clone this repository.
2. Choose Codex, Claude Code, or OpenCode.
3. Read `AGENTS.md` and `.ai/README.md`.
4. Start with `.ai/requirements/r001-example.md` and use the implementation, verification, and review workflows as appropriate.

## Supported tools

| Tool | Integration |
| --- | --- |
| Codex | Reads `AGENTS.md`; shared workflows live in `.agents/skills/`. |
| Claude Code | `CLAUDE.md` imports `AGENTS.md`; `.claude/skills/` links to canonical workflows. |
| OpenCode | `opencode.json` loads the canonical agent prompts directly. |

## Repository structure

```text
.agents/   Shared roles, rules, and task workflows
.ai/       Product and technical context
.claude/   Claude Code adapter
.codex/    Optional local Codex configuration
.opencode/ Optional local OpenCode extensions
app/       Application extension point
tests/     Application tests
```

## Example workflow

1. Read a requirement and applicable context in `.ai/`.
2. Follow `implement-task` to make a focused change.
3. Follow `verify-change` to run relevant checks and report evidence.
4. Use `review-change` for an independent quality review.

## Start Your Project

Use this starter kit as a foundation, not as the identity of your final project. The steps below use a real estate application as a concrete example; adapt the project context and prompt to your own domain.

After cloning it, remove the remote that points to this repository and add the remote for your new project:

```bash
git remote remove origin
git remote add origin <your-project-repository-url>
git remote -v
```

If you downloaded a ZIP file instead, initialize a new Git repository before adding its remote.

Before writing application code, adapt the project context. For the real estate example, this means defining the following:

- `README.md`: project name, purpose, and setup instructions.
- `.ai/project-overview.md`: product scope and intended users.
- `.ai/business-rules.md`: rules for listings, properties, agents, visibility, and enquiries.
- `.ai/requirements/`: a first small, verifiable requirement.
- `app/README.md`: application stack, run command, and test command once those decisions exist.

For that example, you can start an AI-assisted session with this prompt:

> I am starting a real estate application from this starter kit. I have attached or linked real project context, such as screenshots, existing designs, and reference documents; use it to inform the initial project vision and documentation. First, read `AGENTS.md` and the relevant files in `.ai/`. Then update the project overview, business rules, README, and a first verifiable requirement for a minimal property listings feature. Do not implement application code yet. Summarize the proposed scope and assumptions for review.

After approving that context and requirement, use the implementation workflow to begin building the application.

## Scope and limitations

This repository is a lightweight, open-source reference for exploring AI-first software development using shared agents, skills, and project documentation. It is a practical starting point, not a complete production-ready development framework.

At Serfe, we use a more comprehensive internal approach based on years of software engineering and delivery experience. Its requirements management, project coordination, quality assurance, and delivery practices are intentionally outside the scope of this public starter kit.

The goal is to help developers understand the core concepts, experiment with supported AI coding tools, and adapt the structure to their own projects.

## Contributing

Keep shared guidance canonical in `.agents/`, avoid duplicating prompts across tool adapters, and do not contribute credentials, customer data, or internal URLs.

## License

MIT. See [LICENSE](LICENSE).
