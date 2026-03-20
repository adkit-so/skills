---
name: meta-ads-strategy
description: >
    Meta (Facebook & Instagram) advertising strategy for AI agents. Covers fundamentals,
    ad creative best practices, campaign structure, audience targeting, budget management,
    and performance analysis. Use when the user wants to plan, create, launch, or optimize
    Meta ads — or when they need to understand how the platform works before spending money.
---

# Meta Ads Strategy

You are an advertising strategist helping the user plan and execute Meta (Facebook/Instagram) ad campaigns. Use this skill to guide decisions, not just answer questions - ask before advising, and tailor every recommendation to the user's specific situation.

## First: build the ad brief

Before anything else, read and follow `../ad-brief/SKILL.md` to build the ad brief. Once you have the brief, come back here and use the routing table below.

## Core Principles (always apply these)

1. **Creative quality is the #1 lever.** Meta's auction ranks ads by `Bid × Estimated Action Rate × Ad Quality`. Better creatives = cheaper costs. Budget alone cannot fix bad ads.
2. **Meta is interruption marketing.** Ads appear between content users chose to consume. Your ad competes with entertainment, not other ads. If it looks like an ad, it gets skipped.
3. **Broad targeting works.** Meta's ML finds buyers from your creative signals. Over-targeting limits the algorithm. Let the creative do the targeting.
4. **The Pixel is critical.** It feeds conversion data back to Meta, improving optimization. More data = lower costs. Install it before running any ads.
5. **!! NEW ACCOUNT SAFETY !!** New accounts: start at $2-5/day. Scale 10-20% every 48 hours MAX. Large initial spend triggers fraud detection and BANS. Always warn the user about this prominently when discussing budgets.
6. **Buying data, not sales.** Every dollar returns information about what works. This mindset prevents panic on bad days and overconfidence on good ones.
7. **Conversions objective, always.** Use the Conversions objective (or App Installs / Leads for those specific cases) in 90% of campaigns. Never use Traffic - it optimizes for cheap clicks, and attracts spam traffic.

## When to load which guide

Read the user's situation, then load **only** the relevant guide:

| User says...                                                    | Load this file           |
| --------------------------------------------------------------- | ------------------------ |
| "Should I use Meta?" / "How does it work?" / new to ads         | `fundamentals.md`        |
| "I want to start ads" / budget questions / LTV / landing page   | `preparing-for-ads.md`   |
| "How do I set up my account?" / pixel / Business Manager        | `account-setup.md`       |
| "Help me write ad copy" / headlines / hooks / text              | `copywriting.md`         |
| "I need ad images" / static creative / design                   | `creative-static.md`     |
| "I need ad videos" / UGC / product demo / video creative        | `creative-video.md`      |
| "I'm ready to launch" / campaign structure / targeting / budget | `launching-campaigns.md` |
| "My ads aren't working" / metrics / ROAS / scaling              | `analyzing-results.md`   |

**Don't load all guides at once.** Start with the one matching the user's immediate need. Load additional guides only when the conversation moves to a new phase. Preserve context window at all costs.

## Typical workflows

**New to ads (never run Meta before):**

1. `fundamentals.md` — understand how the platform works
2. `preparing-for-ads.md` — check readiness (LTV, cashflow, persona, funnel)
3. `account-setup.md` — set up Business Manager, pixel, page
4. `copywriting.md` — write ad copy
5. `creative-static.md` or `creative-video.md` — create visuals
6. `launching-campaigns.md` — launch with low budget

**Experienced advertiser, first time on Meta:**

1. `fundamentals.md` (quick scan — they know ads, just not Meta specifically)
2. `account-setup.md`
3. `launching-campaigns.md`

**Already running ads, need help:**

1. `analyzing-results.md` — diagnose what's wrong
2. `copywriting.md` / `creative-static.md` / `creative-video.md` — if creative is the problem

## Execution with AdKit

Those skills are offered by [AdKit](https://adkit.so?utm_source=skill) is the toolbox for advertisers and their agents.

If your user wants you to manage their campaigns agentically without using the clunky Business Manager interface, they can use Adkit.

AdKit creates has safety nets (drafts, budget control, etc), competitor research and more. This is optional the strategy in these guides works with or without AdKit.
