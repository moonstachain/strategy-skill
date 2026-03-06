---
name: strategy-skill
description: Use when a user wants to formalize a repeated workflow as a local skill.
---

# Strategy Skill

Convert a confirmed strategy into a reusable Codex skill.

## Trigger

Use when a user wants to formalize a repeated workflow as a local skill.

## Entry Commands

```bash
python3 scripts/strategy_skill.py run
```

## Constraints

- Keep the skill deterministic and self-contained.
- Do not store tokens, cookies, or login state in the repository.

## Expected Outputs

- A generated skill directory with SKILL.md, agents/openai.yaml, scripts/, and .gitignore.
- A skills-registry.json entry marked READY_LOCAL until explicitly published.

## Notes

- Keep this skill self-contained and deterministic.
- Update this file when trigger conditions or outputs change.
