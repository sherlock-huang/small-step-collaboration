# small-step-collaboration

Make an agent guide a human one small step at a time instead of dumping a long SOP.

This repository contains a cross-runtime skill bundle designed for:

- Codex
- OpenClaw
- Hermes

It is especially useful for:

- Google Search Console
- Bing Webmaster Tools
- Baidu Search Resource Platform
- Cloudflare / Vercel / GitHub / database consoles
- setup, deployment, debugging, and verification flows

## What problem this solves

Many agents are capable, but not collaborative enough.

They often overwhelm users with:

- long numbered checklists
- multiple branches at once
- too many requests for screenshots, logs, and outputs in the same turn

This skill changes the default interaction style to:

1. give one smallest useful next action
2. ask for one result artifact
3. interpret the result
4. continue with the next step

## Repository contents

- `SKILL.md` - core trigger description and behavior rules
- `agents/openai.yaml` - Codex UI metadata
- `references/platform-notes.md` - runtime install notes
- `references/response-patterns.md` - reusable response patterns
- `_meta.json` - lightweight metadata for marketplace packaging
- `docs/RELEASE_PACK.md` - technical release sheet for publishing

## Install

### Codex

Copy this folder into:

```text
~/.codex/skills/small-step-collaboration
```

### OpenClaw

Copy this folder into:

```text
~/.openclaw/skills/small-step-collaboration
```

### Hermes

Copy this folder into:

```text
~/.hermes/skills/small-step-collaboration
```

## Example invocation

Use language like:

```text
Use small-step collaboration mode for this task. Give me only the next smallest useful step, wait for my result, then guide the next step.
```

Or more directly:

```text
Use $small-step-collaboration and take me through this console one step at a time.
```

## Public references

- Skill landing page: https://kunpeng-ai.com/skills/small-step-collaboration/
- Download bundle: https://kunpeng-ai.com/downloads/small-step-collaboration-skill.zip
- Technical guide: https://kunpeng-ai.com/blog/small-step-collaboration-skill-guide/
- Why this matters: https://kunpeng-ai.com/blog/why-agents-should-guide-users-one-step-at-a-time/

## License

MIT
