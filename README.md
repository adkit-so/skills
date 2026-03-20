# Ads Skills for AI Agents

Ads strategy skills for Claude Code, OpenAI Codex, Cursor, Copilot, Windsurf, and any agent that supports the [Agent Skills spec](https://agentskills.io).

Give your AI agent expert-level advertising knowledge. Instead of guessing at campaign structure, targeting, and budgets, your agent follows proven frameworks to plan and launch ads that work.

## Available Skills

| Skill | Platform | What it covers |
|---|---|---|
| [ad-brief](./skills/ad-brief/) | All platforms | Product research, audience profiling, market analysis, KPIs. Foundation for all campaigns. |
| [meta-ads](./skills/meta-ads/) | Meta (Facebook & Instagram) | Auction mechanics, creative strategy, campaign structure, targeting, budget management, performance analysis |

Coming soon: Google Ads, LinkedIn Ads, TikTok Ads.

## How Skills Work Together

The `ad-brief` skill is the foundation. Every platform skill reads it first to understand the product, audience, and goals before doing anything.

```
ad-brief (run first)
    |
    v
meta-ads ── fundamentals, creative, campaigns, analysis
google-ads   (coming soon)
linkedin-ads (coming soon)
```

## Install

```bash
npx skills add adkit-so/ads-skills --all -y -g
```

Works with Claude Code, OpenAI Codex, Cursor, GitHub Copilot, Windsurf, and 17+ other agents.

## What Are Skills?

Skills are markdown files that give AI agents specialized knowledge and workflows. When you install these skills, your agent can recognize when you're working on advertising and apply the right strategy and best practices.

| | Without skills | With ads skills |
|---|---|---|
| Campaign structure | Agent guesses | Agent follows proven frameworks |
| Targeting | Agent picks random interests | Agent uses broad targeting (lets Meta's ML optimize) |
| Budget | Agent sets arbitrary amounts | Agent starts at 2x max acquisition cost, scales 10-20% every 48h |
| Creative | Agent writes generic copy | Agent crafts hooks that compete with entertainment, not other ads |
| Analysis | Agent reads numbers | Agent diagnoses issues and recommends specific fixes |

## Why Skills, Not Tools

MCP servers give agents hands (API access). Skills give agents brains (strategy knowledge).

Use both together: skills for planning, tools for execution.

## Using with AdKit

These skills work standalone. But if you want your agent to execute campaigns (create ads, manage budgets, publish) without touching Business Manager, install the [AdKit CLI](https://adkit.so):

```bash
npx adkit-cli setup manage
```

## Contributing

Found something wrong or outdated? PRs welcome.

## License

MIT
