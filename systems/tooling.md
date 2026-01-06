# Tooling Stack

## Overview

| Tool | Role | Status |
|------|------|--------|
| **Slack** | Communication nucleus | TODO: Set up |
| **GitHub Org** | Code + task management | TODO: Create org |
| **Claude Code** | AI automation layer | All have installed |
| **Core Repo** | Monorepo for everything | This repo (rename pending) |

---

## Slack (Nucleus)

### Purpose
- Primary communication hub
- Automated bots and integrations
- Async coordination between co-founders

### Setup TODO
- [ ] Create workspace
- [ ] Add all three co-founders
- [ ] Research: Paid vs free tier?
- [ ] Set up channels structure
- [ ] Integrate GitHub notifications
- [ ] Build custom slash commands

### JP's Expertise
JP is proficient at building Slack integrations. He'll lead the technical setup.

---

## GitHub Organization

### Purpose
- All code in one place
- All three co-founders as org members
- GitHub Issues for task management
- Single source of truth

### Setup TODO
- [ ] Create organization (name TBD)
- [ ] Add Richard, JP, Matt as members
- [ ] Rename this repo to "Core"
- [ ] Transfer repo to org
- [ ] Set up branch protection
- [ ] Configure GitHub Actions (if needed)

### Monorepo Structure (Core)

JP's preference: **One repo, not multi-repo.**

```
/core
├── /docs           # Vision, roadmap, team bios
├── /systems        # Proposal system, task system, tooling
├── /meeting-notes  # Meeting captures
├── /claude-code    # Slash commands, prompts, primitives
├── /products       # Individual product folders (as we ship)
└── README.md
```

---

## Claude Code (Automation Layer)

### Purpose
- AI agent runs on each co-founder's machine
- Manages task execution
- Automates proposal ranking
- Tracks MRR and course corrects

### Everyone Has
- [x] Richard — Claude Code installed
- [x] JP — Claude Code installed (heavy user, $3K+/mo)
- [x] Matt — Claude Code installed

### Primitives to Build
- [ ] Proposal system slash commands
- [ ] Task system slash commands
- [ ] MRR tracking automation
- [ ] Shape Up cycle management

---

## Integration Map

```
┌─────────────────────────────────────────────────────┐
│                      SLACK                          │
│                   (Communication)                   │
│                        │                            │
│    ┌──────────────────┼──────────────────┐         │
│    │                  │                  │         │
│    ▼                  ▼                  ▼         │
│ Richard's          JP's              Matt's        │
│ Claude Code     Claude Code       Claude Code      │
│    │                  │                  │         │
│    └──────────────────┼──────────────────┘         │
│                       │                            │
│                       ▼                            │
│              GitHub (Core Repo)                    │
│              - Code                                │
│              - Issues (Tasks)                      │
│              - Proposals                           │
│              - Documentation                       │
└─────────────────────────────────────────────────────┘
```

---

*Tooling design: January 6, 2026*
