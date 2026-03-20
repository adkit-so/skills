# AdKit Skills

Agent skills for advertising strategy across Meta Ads, Google Ads, LinkedIn Ads, and more.

> The ad strategist's brain, packaged as agent skills.

Works with Claude Code, OpenClaw, Cursor, GitHub Copilot, Windsurf, Codex, and any agent that supports the [Agent Skills](https://agentskills.io) standard.

## Skills

| Skill | Platform | What it teaches |
|---|---|---|
| [meta-ads](./meta-ads/) | Meta (Facebook & Instagram) | Auction mechanics, creative strategy, campaign structure, audience targeting, budget allocation, performance analysis |

More platforms coming (Google Ads, LinkedIn, TikTok).

## Install

**Universal** (works with 17+ agents):
```
npx skills add adkit/adkit-skills
```

**ClawHub** (OpenClaw):
```
clawhub install adkit/adkit-skills
```

**Manual** — clone this repo and copy the skill folder into your agent's skills directory (e.g., `.claude/skills/`).

## Why Skills, Not Tools

MCP servers give agents hands (API access). Skills give agents brains (strategy knowledge).

| | MCP servers | AdKit Skills |
|---|---|---|
| Create a campaign | Yes | - |
| Know *how* to structure a campaign | - | Yes |
| Read metrics | Yes | - |
| Know *what* metrics matter and *why* | - | Yes |
| Set a budget | Yes | - |
| Know *how much* to budget and *when* to scale | - | Yes |

Use both together for full autonomous ad management.

## How it works

Each skill contains:

- **SKILL.md** — entry point with core principles and a routing table. Your agent reads this first and loads detailed guides on demand.
- **Strategy guides** — deep dives on specific topics (creative, targeting, budgets, analytics). Only loaded when relevant — zero token cost until needed.

The guides teach advertising strategy — not tool documentation. They cover the "what" and "why" of running ads so your agent can advise, plan, and make informed decisions.

## Using with AdKit

These skills work standalone — no subscription required. But if you want to execute campaigns programmatically (create, manage, publish ads without touching Business Manager), install [AdKit](https://adkit.so):

```
npx @adkit.so/cli setup manage
```

## Contributing

Found something wrong or outdated? PRs welcome.

## License

MIT
