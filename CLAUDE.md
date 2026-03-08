# CLAUDE.md

This file provides guidance to AI assistants (Claude and others) working in this repository.

## Project Overview

**cambio** is a newly initialized repository. This CLAUDE.md will be updated as the project takes shape.

- **Repository:** `benjamincano/cambio`
- **Current state:** Initial scaffold — no source code, dependencies, or tooling yet configured.

---

## Repository Structure

```
cambio/
├── CLAUDE.md        # This file
└── README.md        # Project README (placeholder)
```

As the project grows, update this section to reflect the actual layout.

---

## Development Workflow

### Branching Strategy

- Feature/task branches follow the pattern: `claude/<description>-<session-id>`
- The default long-lived branch is `master`
- Always develop on the designated feature branch and push before opening a PR

### Git Commit Conventions

Write clear, imperative commit messages:

```
Add user authentication module
Fix off-by-one error in pagination logic
Update dependencies to resolve security advisory
```

- Keep the subject line under 72 characters
- Use the body to explain *why*, not *what*

### Push Workflow

```bash
git add <files>
git commit -m "your message"
git push -u origin <branch-name>
```

> Note: Branch names must start with `claude/` when working in AI-assisted sessions.

---

## Commands

> No build system or scripts are configured yet. Update this section once a tech stack is chosen.

Typical commands to document here:

| Command | Purpose |
|---------|---------|
| `npm install` / `pip install` / etc. | Install dependencies |
| `npm run dev` / `python main.py` | Start development server |
| `npm test` / `pytest` / `cargo test` | Run tests |
| `npm run lint` | Lint source code |
| `npm run build` | Produce production build |

---

## Code Conventions

Update this section when the tech stack is established. In the meantime, follow these general principles:

- **Simplicity first** — write the minimum code that satisfies the requirement
- **No premature abstractions** — avoid helper utilities for one-off operations
- **No speculative features** — only implement what is explicitly requested
- **No unnecessary comments** — only add comments where logic is non-obvious
- **Validate at boundaries** — user input and external API responses; trust internal code
- **Secure by default** — avoid command injection, SQL injection, XSS, and other OWASP Top 10 issues

---

## Testing

> No test framework configured yet. Update this section when tests are added.

Conventions to follow once a framework is chosen:

- Tests live alongside source files or in a dedicated `tests/` / `__tests__/` directory
- Every new feature or bug fix should be accompanied by a test
- All tests must pass before merging

---

## Environment Variables

> No `.env.example` exists yet. Add one when environment configuration is needed.

When environment variables are introduced:

1. Add a `.env.example` listing every required variable with placeholder values
2. Never commit actual secrets — add `.env` to `.gitignore`
3. Document the purpose of each variable in `.env.example`

---

## AI Assistant Guidelines

When working in this repository:

1. **Read before editing** — always read a file before modifying it
2. **Minimal changes** — only change what is necessary for the task at hand
3. **No unrequested improvements** — do not refactor, add docstrings, or clean up surrounding code unless asked
4. **Confirm destructive actions** — ask before force-pushing, dropping data, or deleting files
5. **Update CLAUDE.md** — when the project gains a tech stack, tests, or new conventions, update the relevant sections of this file to keep it accurate
6. **Branch discipline** — develop on the branch specified in the task; never push to `master` directly

---

*Last updated: 2026-03-08. Update this file whenever the project structure or conventions change.*
