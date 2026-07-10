<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,100:16213e&height=200&section=header&text=xAgentCraft&fontSize=60&fontColor=e94560&fontAlignY=35&desc=A%20curated%20collection%20of%20custom-crafted%20agent%20commands&descSize=18&descAlignY=55&descColor=ffffff" width="100%"/>

</div>

## What is xAgentCraft?

xAgentCraft is a growing collection of custom-crafted agent commands — ready-to-use markdown files that define how AI agents should behave for specific dev tasks. Each agent has a clear purpose, a defined workflow, and structured output so you know exactly what you're getting.

No code. No dependencies. Just drop an agent into your workflow and go.

## Agents

| Agent | Icon | Description |
|-------|:----:|-------------|
| [Iterative Code Fix Agent](agents/iterative-code-fix-agent.md) | 🔧 | Resolves issues in a codebase through an iterative fix-verify loop. Never applies a change without your approval first. |
| [Breaking Code Change Reviewer](agents/breaking-change-reviewer.md) | ⚠️ | Reviews code changes and flags anything that could break existing functionality or consumers. |

## How to Use

1. Browse the [`agents/`](agents/) folder
2. Pick the agent you need
3. Copy the contents and use it as a system prompt or custom command with your preferred AI tool

That's it.

## Contributing

Want to add your own agent? Follow the format — frontmatter at the top, clear behavior rules, and a structured output format. Open a PR.

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,100:16213e&height=100&section=footer" width="100%"/>

</div>
