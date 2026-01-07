# CLAUDE.md

## Repository Overview

This is the **Core monorepo** for a 3-person AI-native startup (JP Boodhoo, Matt Kennedy, Richard Stock). It contains vision, systems design, and future product code. The company ships 24 products in 2026 using AI-driven development.

## Structure

```
/docs           # Vision, roadmap, team bios
/systems        # Proposal system, task system, tooling specs
/meeting-notes  # Meeting captures
/products       # Individual products (added as shipped)
```

## Philosophy

- **Throughput over quality** — Ship fast, iterate in days not weeks
- **MRR is the only metric** — Every decision ties to monthly recurring revenue
- **Shape Up methodology** — 2-week delivery cycles, full product per cycle
- **Completion criteria only** — Define WHAT done looks like, AI figures out HOW

## Systems Being Built

### Proposal System
Slash commands for capturing/ranking product ideas by MRR potential:
- `/proposal-draft`, `/proposal-read`, `/proposal-list`, `/proposal-search`, `/proposal-rank`

### Task System
GitHub Issues as tasks with completion criteria (not implementation details):
- `/task-create`, `/task-list`, `/task-claim`, `/task-complete`, `/task-status`

## When Writing Code in This Repo

- Products go in `/products/<product-name>/`
- Claude Code primitives/slash commands go in `/claude-code/` (to be created)
- Issue descriptions should specify completion criteria, not implementation steps
- Ship MVPs fast — good enough beats perfect
