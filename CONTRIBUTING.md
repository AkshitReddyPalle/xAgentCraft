# Contributing to xAgentCraft
 
Thanks for wanting to add an agent. Here's how to do it right.
 
## Agent Format
 
Every agent lives in a `Command.md` file. It must follow this structure:
 
**Frontmatter** — metadata at the top of the file wrapped in `---` delimiters:
 
```
---
name: "Your Agent Name"
description: "One sentence describing what this agent does."
color: "blue"
icon: "🔧"
model: "inherit"
---
```
 
| Field | Required | Description |
|-------|:--------:|-------------|
| `name` | Yes | The display name of the agent |
| `description` | Yes | One clear sentence explaining what it does |
| `color` | Yes | A color label for the agent |
| `icon` | Yes | A single emoji representing the agent |
| `model` | No | The model to use. Use `"inherit"` to use the default |
 
**Body** — after the frontmatter, the Command.md should include the following sections:
 
1. **Title** — `# Agent Name` matching the frontmatter name
2. **Role** — who the agent is and what it does, written as "You are a..." so it reads as a direct instruction
3. **Input** — what the agent expects to receive from the user
4. **Process** — the step-by-step workflow the agent follows
5. **Output** — the exact format the agent should respond in
6. **Rules** — specific constraints and behaviors the agent must follow
Not every agent needs every section. Some agents might need additional sections like "Severity Levels" or "Loop Termination." Use what makes sense — but Role, Output, and Rules are mandatory.
 
## Folder Structure
 
```
Agents/
├── Your-Agent-Name/
│   └── V1/
│       └── Command.md
```
 
- Agent folder name: **capitalized kebab-case** (e.g. `PR-Summarizer`, `Breaking-Code-Change-Reviewer`)
- Version folder: **uppercase** (e.g. `V1`, `V2`)
- Command file: **`Command.md`** — always capitalized
## Versioning
 
- Start with `v1`
- Create a new version folder (`v2`, `v3`) when there are major changes to the agent's behavior, output format, or scope
- Small fixes and wording improvements can be updated within the same version
## What Makes a Good Agent
 
- **Clear purpose** — it does one thing and does it well. No Swiss Army knife agents.
- **Specific rules** — tell the agent exactly what to do and what not to do. Vague instructions produce vague results.
- **Defined output** — the output format should be explicit so the response is consistent and predictable every time.
- **Honest about limitations** — if the agent can't do something, it should say so, not guess.
- **Readable** — written in plain language. If a developer can't understand the agent in 60 seconds, it's too complicated.
## What We Don't Accept
 
- Agents with no defined output format
- Agents that are too vague or generic (e.g. "helps with code")
- Duplicates of existing agents without meaningful differences
- Agents with no rules or constraints
- Agents that require API keys or external dependencies
## How to Submit
 
1. Create your agent following the format above
2. Add it to the `Agents/README.md` table
3. Open a PR
 
