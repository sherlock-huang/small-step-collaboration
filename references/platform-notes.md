# Platform Notes

## Codex

- Install path: `~/.codex/skills/small-step-collaboration`
- Codex discovers the skill from `SKILL.md`.
- `agents/openai.yaml` improves the UI label and default prompt.

## OpenClaw

- Install path: `~/.openclaw/skills/small-step-collaboration`
- OpenClaw also reads `SKILL.md` as the main skill definition.
- A root `_meta.json` can be added later if the skill is published to a marketplace feed.

## Hermes

- Install path: `~/.hermes/skills/small-step-collaboration`
- Hermes can load the skill directly from the folder that contains `SKILL.md`.
- If you later want category grouping, move it under a parent category directory without changing the inner skill folder.

## Claude Code

- Keep this as a compatibility note for later packaging.
- The same prompt body can be reused, but the final distribution shape may differ depending on the runtime.
