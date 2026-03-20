# Ads Skills for AI Agents

Advertising strategy for AI coding agents. Install once, and your agent plans and runs Meta ad campaigns using real frameworks instead of hallucinating campaign settings.

Works with Claude Code, Cursor, Copilot, Windsurf, OpenAI Codex, and any agent that supports the [Agent Skills spec](https://agentskills.io).

## Available AI Agent Advertising Skills

| Skill | Platform | What it covers |
| --- | --- | --- |
| [ad-brief](./skills/ad-brief/) | All platforms | Product research, audience profiling, market analysis, KPIs. Foundation for all campaigns. |
| [meta-ads](./skills/meta-ads/) | Meta (Facebook & Instagram) | Auction mechanics, creative strategy, campaign structure, targeting, budget management, performance analysis |

Coming soon: Google Ads, LinkedIn Ads, TikTok Ads.

## How to Install Ads Skills for Claude Code (and Other Agents)

```bash
npx skills add adkit-so/ads-skills --all -y -g
```

Works with Claude Code, OpenAI Codex, Cursor, GitHub Copilot, Windsurf, and 17+ other agents.

## What's Inside

650+ lines of advertising strategy across two skills, covering the full lifecycle from research to optimization:

- **Meta ads auction mechanics**: how Ad Rank works (Bid x Estimated Action Rate x Ad Quality) and how to work with the algorithm
- **Campaign structure**: three-level hierarchy (Campaign > Ad Set > Ad), objective selection, optimization events
- **Audience targeting**: when to go broad vs. interest-based vs. lookalike, and why most beginners over-target
- **Budget management**: start at 2x target acquisition cost, scale rules, when to kill underperformers
- **Ad creative**: hook frameworks, safe zones for 9:16 video, the 1-second rule, format selection (static vs. video vs. hybrid)
- **Performance diagnostics**: symptom-cause-action framework for reading CPM, CTR, CPC, ROAS, and frequency
- **Ad brief methodology**: product research, ICP profiling, market positioning, KPI selection before any money is spent
- **Account setup and compliance**: ban prevention rules, Pixel configuration, payment method strategy

## How Skills Work Together

The `ad-brief` skill is the foundation. Every platform skill reads it first to understand the product, audience, and goals before doing anything platform-specific.

```
ad-brief (run first)
    |
    v
meta-ads -- fundamentals, creative, campaigns, analysis
google-ads   (coming soon)
linkedin-ads (coming soon)
```

## What Are AI Agent Skills?

Skills are markdown files that give AI agents specialized knowledge and decision-making frameworks. The agent reads them at runtime and applies the right strategy for the task at hand.

The key distinction: MCP servers give agents **hands** (API access to run ads). Skills give agents **brains** (strategy knowledge to run them well). Use both together.

|  | Without ads skills | With ads skills |
| --- | --- | --- |
| Campaign structure | Agent guesses | Agent follows proven frameworks |
| Targeting | Agent picks random interests | Agent uses broad targeting (lets Meta's ML optimize) |
| Budget | Agent sets arbitrary amounts | Agent starts at 2x max acquisition cost, scales progressively |
| Creative | Agent writes generic copy | Agent crafts hooks that compete with entertainment, not other ads |
| Analysis | Agent reads numbers | Agent diagnoses issues and recommends specific fixes |

## How to Run Meta Ads with AI Agents

1. Install the skills with the command above
2. Open your agent (Claude Code, Cursor, etc.)
3. Ask it to run `ad-brief` first: builds your product brief, audience profile, and KPIs
4. Then run `meta-ads` for campaign planning, creative, and launch
5. Optionally, connect [AdKit](https://adkit.so) so your agent can execute campaigns directly (no manual Business Manager)

```bash
# For full execution (planning + publishing):
npx adkit-cli setup manage
```

## FAQ

**What agents are supported?**
Any agent that supports the [Agent Skills spec](https://agentskills.io): Claude Code, Cursor, Copilot, Windsurf, OpenAI Codex, and 17+ others.

**Do I need an AdKit account to use these skills?**
No. The skills work standalone for strategy and planning. AdKit is only needed if you want your agent to create and publish campaigns without logging into Business Manager.

**Can I add my own skills or modify these?**
Yes. Fork the repo, edit the markdown files, and install your fork with `npx skills add your-username/your-repo --all -y -g`. PRs with improvements are welcome.

## Author

Built by [Nico Jeannen](https://jeannen.com) ([@nico_jeannen](https://x.com/nico_jeannen)). 10 years in digital advertising, managed $1M+ in ad spend across Meta, Google, and LinkedIn. Built and sold three apps ($290k combined), two of them grown primarily through paid acquisition. Now building [AdKit](https://adkit.so), the advertising toolbox for SaaS founders.

The frameworks in these skills come from running real campaigns, not from reading blog posts about running campaigns.

## Contributing

Found something wrong or outdated? PRs welcome. If you've built skills for other ad platforms (Google Ads, TikTok, LinkedIn), open an issue first so we can coordinate.

## License

[MIT](./LICENSE)
