# Strategy Skill Template

## What it is
Strategy Skill Template is a lightweight Codex skill for turning a confirmed strategy into a reusable local skill scaffold.

## Who it's for
This repo is for operators who already know the workflow they want to formalize and need a fast way to produce a deterministic local skill skeleton before deciding whether to publish it.

## Quick start
```bash
python3 scripts/strategy_skill.py run
```

## Inputs
- A confirmed strategy or workflow definition.
- Any required prompt or configuration expected by `scripts/strategy_skill.py`.

## Outputs
- A generated skill directory with `SKILL.md`, `agents/openai.yaml`, `scripts/`, and `.gitignore`.
- A `skills-registry.json` entry marked `READY_LOCAL` until publication is requested.

## Constraints
- The generated skill must stay deterministic and self-contained.
- Tokens, cookies, and login state should never be stored in the repository.
- This repo is intended for local skill generation first, not automatic remote publication.

## Example
Use this skill when a workflow has already been validated in practice and you want a local Codex skill scaffold that can later be refined or handed to a publisher pipeline.

## Project structure
- `scripts/`: local skill generation entrypoint.
- `references/`: supporting notes for the strategy-to-skill workflow.
- `agents/`: Codex interface metadata.
