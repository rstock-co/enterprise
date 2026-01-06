# Task System

## Purpose

Fully automated task delegation using GitHub Issues + Claude Code. Humans define WHAT (completion criteria). AI figures out HOW (implementation).

---

## Core Principles

1. **GitHub Issues = Tasks** — Not markdown files, not Notion, not Jira
2. **Completion Criteria Only** — Issue description says what DONE looks like
3. **No Implementation Details** — Claude/AI figures out the HOW
4. **Any Co-Founder Can Claim** — See what others pushed, pick it up
5. **Claude Manages Completion** — AI tracks and closes when criteria met

---

## Issue Structure

### Title
Clear, action-oriented. What needs to exist when this is done?

### Description (Completion Criteria)
```markdown
## Done When

- [ ] [Criteria 1]
- [ ] [Criteria 2]
- [ ] [Criteria 3]

## Context

[Any relevant context, links, or constraints]
```

### What NOT to Include
- Step-by-step instructions
- Implementation approach
- Technology choices (unless required)
- Time estimates

---

## Slash Commands (Planned)

| Command | Description |
|---------|-------------|
| `/task-create` | Create a new GitHub Issue |
| `/task-list` | List open tasks |
| `/task-claim <id>` | Assign yourself to a task |
| `/task-complete <id>` | Mark task as done (checks criteria) |
| `/task-status` | Show your current tasks |

---

## Workflow

1. **Co-founder has a task** → Creates GitHub Issue with completion criteria
2. **Anyone can see open issues** → Claims one via `/task-claim`
3. **Claude Code executes** → AI figures out implementation
4. **Criteria checked** → When all boxes tick, issue closes
5. **Push to main** → Work is visible to all

---

## Why GitHub Issues?

- Native to our workflow (already on GitHub)
- Visible to all co-founders
- Integrates with PRs and commits
- API access for automation
- History and audit trail
- Slack integration possible

---

## AI-Native Task Management

The key insight: **Humans are bad at writing HOW. Humans are good at defining DONE.**

Traditional task systems: "Implement OAuth using NextAuth with Google provider..."

Our system: "Users can sign in with Google. Session persists across page refresh."

Claude figures out the rest.

---

*System design: January 6, 2026*
