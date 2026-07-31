---
name: amazing-claude-skills
description: Turn a linked issue or repo reference into a minimal, validated implementation plan and patch.
---

# Amazing Claude Skills

A practical skill for taking a repository or issue reference and converting it into focused implementation work with minimal, surgical code changes.

## When to Use This Skill

- You need to implement a change from an issue link with limited context
- You want to keep edits minimal while still fully solving the request
- You need a repeatable workflow for inspect → change → verify

## What This Skill Does

1. **Extracts requirements**: Identifies concrete expectations from links and surrounding context.
2. **Plans minimal edits**: Chooses the smallest set of file changes needed for a complete fix.
3. **Validates outcomes**: Runs targeted checks and confirms behavior manually where needed.

## How to Use

### Basic Usage

```
Implement the issue described at <link> with the smallest possible complete change.
```

### Advanced Usage

```
Implement the issue at <link>.
Use a minimal-diff approach, add focused tests only if test infra exists, and report progress after each verified unit.
```

## Example

**User**: "Implement the requirements in this repository link and keep the changes surgical."

**Output**:
```
A scoped plan, minimal file edits, targeted verification, and a concise summary of what changed.
```

**Inspired by:** Real-world coding-agent workflows for issue-driven maintenance.

## Tips

- Start by reading existing files before proposing changes.
- Prefer targeted verification over full-suite runs early.
- Keep each commit focused on one meaningful unit of work.

## Common Use Cases

- Translating issue links into implementation tasks
- Applying small fixes safely in unfamiliar repositories
- Producing reviewable, low-noise pull requests
