# Proposal System

## Purpose

A formalized system for capturing, evaluating, and ranking product ideas. Anyone can contribute proposals. AI ranks them by MRR potential.

---

## Slash Commands

| Command | Description |
|---------|-------------|
| `/proposal-draft` | Create a new proposal |
| `/proposal-read <id>` | View a specific proposal |
| `/proposal-list` | List all proposals |
| `/proposal-search <query>` | Search proposals |
| `/proposal-rank` | AI ranks proposals by MRR potential |

---

## Proposal Structure

When drafting a proposal, include:

```markdown
# Proposal: [Name]

## One-Liner
[What is this in one sentence?]

## Problem
[What problem does this solve?]

## Target Customer
[Who pays for this?]

## Revenue Model
[How does this make MRR?]

## MVP Scope
[What's the minimum to ship in 2 weeks?]

## Competition
[What exists? Why is this different?]

## Gut Check
[Why do you think this will work?]
```

---

## AI Evaluation Criteria

When ranking proposals, AI considers:

1. **MRR Potential** — How much recurring revenue is realistic?
2. **Time to Revenue** — How fast can we get first dollar?
3. **Market Demand** — Is there proven demand? What's hot?
4. **Competition** — Crowded or underserved?
5. **Build Complexity** — Can we ship in 2 weeks?
6. **Team Fit** — Does this match our skills?

---

## Workflow

1. **Anyone drafts a proposal** via `/proposal-draft`
2. **Proposals accumulate** in the system
3. **Weekly (or as needed):** Run `/proposal-rank` for AI analysis
4. **Team reviews** top-ranked proposals
5. **Pick one** for the next 2-week cycle
6. **Ship it**

---

## Guiding Principle

**MRR is the ONLY objective.**

We don't prioritize what we want to build. We prioritize what makes money. AI helps us see past our biases.

---

*System design: January 6, 2026*
