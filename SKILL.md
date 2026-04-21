---
name: small-step-collaboration
description: Guide users through complex tasks one small step at a time instead of dumping long checklists. Use when the user is working through setup wizards, webmaster consoles, cloud dashboards, CLI debugging, deployment flows, or any unfamiliar multi-step task that benefits from tight back-and-forth confirmation. Break the work into the next smallest meaningful action, ask only for the result of that step, then adapt the next step.
---

# Small-Step Collaboration

Keep the user moving without overwhelming them.

## Core contract

- Default to one meaningful next step per turn.
- Give the exact click path, field name, command, or check the user needs right now.
- Ask for only one result artifact before continuing: a screenshot, pasted output, a yes/no confirmation, or the visible state of the current page.
- After the user replies, interpret the result and continue with the next smallest step.

Do not dump a long SOP unless the user explicitly asks for the full checklist.

## Response pattern

Start with a short orientation line, then the next action, then what success looks like.

Preferred structure:

1. Goal in one sentence.
2. Do this now.
3. Tell me what you see.

When a command is needed, provide one command block and one sentence explaining the expected output.

## Interaction rules

- Prefer one recommendation over a list of equal-weight options.
- If there are multiple branches, recommend the safest path first and mention the fallback in one short sentence.
- Use the exact labels the user should click when dealing with web consoles.
- Separate "do now" from "verify now".
- If the agent can do part of the work directly, do it first and only hand back the step that truly requires the user.
- If the user asks for status, give a short status line and then the next step.

## When working in dashboards or consoles

- Give a single click path at a time.
- Name the menu, tab, button, and field exactly.
- Ask for the state of the current screen before moving deeper.
- If the page is loading or processing, tell the user whether to wait, refresh, or inspect another field.

## When debugging

- Test one hypothesis at a time.
- Ask for one log snippet, one screenshot, or one command result at a time.
- Say what the current test is trying to confirm or rule out.
- Once a result comes back, explain what it means before giving the next action.

## When releasing or deploying

- Split the flow into prepare, execute, verify.
- Never mix pre-checks, deployment, and post-checks into one dense block.
- If the user needs to click a console button after deployment, wait until the deployment is confirmed complete.

## Avoid

- Long numbered lists when only the next step matters.
- Asking for multiple screenshots, logs, and URLs in the same turn.
- Repeating background context the user already knows.
- Giving three different ways to do the same thing unless the first one is blocked.

## Escalation

If the task has hidden risk, say so briefly and pause on the smallest safe checkpoint first.

Examples:

- "Before we touch production, first confirm the current environment variable value."
- "Before we request validation, first open the example URL and confirm it returns 200."

## References

- For platform-specific notes and install paths, read `references/platform-notes.md`.
- For response templates and examples, read `references/response-patterns.md`.
