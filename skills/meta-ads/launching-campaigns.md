# Launching Campaigns

You are guiding a user through setting up and launching Meta ad campaigns. This document is your playbook — follow the decision tree, ask the right questions, and tailor your advice to the user's situation.

## Before You Start

Ask the user:
- What do you sell? (product type, price point)
- What's your daily budget?
- Do you have pixel data already? (conversions firing?)
- Have you run Meta ads before?

Use the answers to route through this guide:

| Situation | Recommended path |
|-----------|-----------------|
| No pixel data, no ad history | Leads objective, single ad set, low budget ($2-5/day). Jump to **Low budget setup**. |
| Has pixel data, budget under $10/day | Sales objective, single ad set with DCA. Optimize for the event with the most data. |
| Has pixel data, budget $25-50+/day | Sales objective, 2-3 ad sets (interest + broad + lookalike). Full **Default setup**. |
| Has pixel data, budget $100+/day | Consider Advantage+ Shopping in addition to manual campaigns. See **Other Setups**. |
| New ad account, any budget | Start at $2-5/day regardless of total budget. See **Ban Prevention** notes throughout. |

> **Ask:** "What's your main goal — sales, leads, or awareness?" Use the answer to select the campaign objective below.

## The Three-Level Hierarchy

Every Meta ad account is organized in three nested levels:

| Level | What you set here | Think of it as |
|-------|------------------|----------------|
| **Campaign** | Objective, overall budget (CBO), spending limits | The goal |
| **Ad set** | Audience, placements, schedule, optimization event, budget (ABO) | Who sees it, when, and how Meta optimizes |
| **Ad** | Images/videos, copy, headlines, CTA, destination URL | What people actually see |

One campaign contains multiple ad sets. Each ad set contains multiple ads. They are nested, not separate.

## Campaign Objectives

> **Ask:** "Do you want direct sales from your site, or are you collecting leads/signups first?"

Pick the objective that matches your actual business goal. Meta adjusts its algorithm and available optimizations based on this choice.

| Objective | When to use | When to skip |
|-----------|------------|--------------|
| **Sales** | You sell a product/subscription and want direct conversions. Default for most advertisers. | You have no pixel events firing yet. |
| **Leads** | You collect emails, signups, or contact info. Great for pre-launch, low budgets, or high-touch sales. | You can already sell directly from a landing page. |
| **Engagement** | You want video views or post interactions. Useful for building retargeting audiences. | You care about revenue, not vanity metrics. |
| **Traffic** | Almost never. You get clicks, not conversions. | Almost always. Optimize for actions, not clicks. |
| **Awareness** | Massive brand-building budgets (think Coca-Cola). | You need measurable ROI. 99% of advertisers skip this. |
| **App Promotion** | Mobile app installs. Requires separate tracking setup. | You run a web app or SaaS. |

**Most common choice:** Sales. If budget is tight or you lack pixel data, start with Leads.

> **If the user has no pixel data:** Recommend starting with the Leads objective. Explain that Sales optimization requires conversion events to learn from — without data, Meta has nothing to optimize toward, and the campaign will waste budget.

## Ad Set Configuration

### Optimization & Conversion Events

At the ad set level, you choose what Meta optimizes for. Set **Performance goal** to "Maximize number of conversions" and select your pixel event (purchase, subscribe, signup, etc.).

> **Walk the user through choosing the optimization goal based on their budget and product price.** A $5/month product optimizing for Purchase needs the same budget as a $50 product — if the product is cheap, leads + email nurture is almost always more cost-effective.

**The virtuous cycle:** Your pixel sends conversion data to Meta. Meta finds similar users and shows them your ad. Some convert, feeding more data back. The more data you have, the better Meta targets. This is why coupling ads with other traffic sources (SEO, email, organic) accelerates results — Meta learns from all site visitors, not just ad traffic.

If your chosen event has zero or very few fires, Meta has nothing to learn from. Options:
- Optimize for a lower-funnel event you do have data on (e.g., signup instead of purchase)
- Drive some organic conversions first, then switch to ads
- Use leads as a stepping stone

### Audiences

**Start broad.** Meta has become exceptionally good at finding buyers without interest targeting. Over-targeting from day one leaves the algorithm no room to optimize.

Three audience types for ad sets:

| Type | Setup | Best for |
|------|-------|----------|
| **Interest-based** | Add relevant interests. Use Meta's "Suggestions" button to expand. Aim for 50M+ audience size. | First ad sets when you have no pixel data. |
| **Broad** | No interests, no custom audiences. Just location + age. Let Meta figure it out. | Accounts with existing pixel data. Often outperforms interests. |
| **Lookalike** | Based on a custom audience (subscribers, purchasers). Meta finds the top 1% similar users. | You have 1,000+ people in a source audience. |

**Location:** Target all countries you sell to, not just the obvious ones (US, UK, CA). Include Western Europe, Japan, Korea, Australia — anywhere with purchasing power. Save location lists so you don't re-enter countries for every ad set.

**Age & gender:** Leave as broad as possible (18-65+, all genders). Meta already knows who is likely to convert. Restricting these limits the algorithm's reach — even for gendered products, Meta can find gift buyers.

### Placements

Use **Advantage+ placements** (Meta's default). Manual placement selection is almost never worth it. Meta will automatically stop showing your ad on placements where it underperforms.

### Budget & Schedule

Two modes:
- **CBO (Campaign Budget Optimization):** Set budget at campaign level. Meta distributes across ad sets automatically. Recommended for most setups.
- **ABO (Ad Set Budget Optimization):** Set budget per ad set. Use when you want explicit control over spend per audience.

**Schedule rule:** Never start ads mid-day. Meta will rush to spend the remaining daily budget in fewer hours, reaching less relevant people. Start between midnight and 6 AM. If you're new and Meta needs review time, add a 12-hour buffer — schedule for 6 AM the next day.

> **Ban prevention:** Never start ads mid-day — Meta rushes to spend remaining budget, reaching less relevant people and producing erratic spend patterns that can flag the account.

**End dates:** Don't set them unless you're running a time-limited promotion. You can always pause manually.

## Choosing the Right Optimization Goal

This is the most consequential decision in your campaign. It determines who Meta shows your ads to.

| Goal | Use when | Typical daily budget needed |
|------|----------|---------------------------|
| **Purchase / Subscribe** | Strong landing page, product with proven demand, enough budget for Meta to learn | $20-50+/day minimum |
| **Signup / Free Trial** | Product where users convert better after trying it. Test against direct purchase — free trials don't always win. | $10-25+/day |
| **Lead / Email** | Pre-launch, low budget, high-touch sales, lead magnets with email automation | As low as $2-5/day |

> **If budget is under $10/day:** Recommend the Lead/Email optimization. Explain that Purchase optimization needs enough budget to generate several conversions per week for Meta to learn — at $10/day, that's unlikely for most products.

**Key insight:** A cheap product ($5/month) costs nearly the same effort per acquisition as a $50 product. Don't waste ad spend on low-value conversions. If your product is cheap, collect leads and nurture with email automation instead.

**Lead magnets work:** A free PDF, industry report, or tool that collects emails, followed by an automated email sequence, is one of the most cost-effective funnels for Meta ads.

## Recommended Account Structure

> **Ask:** "How much can you spend per day on ads?" Then recommend the matching structure below.

**Default setup (works for $25-50+/day):**

```
Campaign (Sales, CBO, $25-50/day)
├── Ad Set: Interest-based (SEO, marketing, etc.)
│   └── DCA: 3 media + 2 texts + 1 headline
├── Ad Set: Broad (no targeting)
│   └── DCA: same assets
└── Ad Set: Lookalike (if you have 1k+ source audience)
    └── DCA: same assets
```

- 1 campaign, 1-3 ad sets, dynamic creative ads (DCA) in each
- Enable **Dynamic Creative** on each ad set — Meta mixes your media, copy, and headlines to find winning combinations
- DCA formula: **3 media files + 2 primary texts + 1 headline** (reduce to 2 media + 1 text if budget is under $10/day)
- Create the first ad set with its ad fully configured, then **duplicate** the ad set to create variations — saves time and preserves ad setup

**Low budget setup ($2-10/day):**
Same structure but optimize for Leads instead of Purchase. Use a single ad set with DCA. Consider using Meta's **Instant Forms** instead of a landing page — conversions happen inside Facebook, so tracking is 100% accurate and costs are lower.

> **If the user has a new ad account:** Regardless of their total budget, recommend starting at $2-5/day and scaling up over 1-2 weeks. Large initial spend on fresh accounts triggers Meta's fraud detection and can result in account restrictions or bans.

## Naming Conventions

Consistent naming makes analysis, collaboration, and external analytics possible at a glance.

| Level | Pattern | Example |
|-------|---------|---------|
| **Campaign** | `{project}_{goal}_{date}` | `talknotes_sales_2025-03` |
| **Ad set** | `{event}_{audienceType}_{audienceName}` | `purchase_interest_executives` or `purchase_broad` |
| **Ad** | `{creativeId}--{copyId}--{headlineId}` | `a3kx--b7mq--c2nf` |

For ads, generate short unique IDs for each creative, copy, and headline. This lets you identify winning combinations from the dashboard without opening individual ads. When using DCA, just name the ad `DCA` — Meta handles the combinations internally.

**UTM parameters** for external analytics (Plausible, GA, etc.):

| Parameter | Value |
|-----------|-------|
| `utm_source` | `facebook` |
| `utm_medium` | `{{placement}}` |
| `utm_campaign` | `{{campaign.name}}` |
| `utm_content` | `{{ad.name}}` |

Set these in the ad's URL Parameters field. They survive ad blockers that may block pixel events.

## Budget Management

### Setting Your Initial Budget

**Formula:** Maximum acquisition cost x 2 = daily budget. Run for at least 7 days.

| Optimization | Max cost per result | Daily budget | 7-day spend |
|-------------|--------------------|--------------|-----------  |
| Purchase | $30 | $60 | $420 |
| Subscription | $50 | $100 | $700 |
| Lead | $3 | $6 | $42 |

Why 7 days minimum: conversion costs vary by day of week. B2B products are cheaper on weekdays. Consumer products spike on weekends. A partial-week test gives unrepresentative data.

**Only spend what you can afford to lose.** Meta ads are a marketing experiment — you're buying data, not guaranteed sales.

> **Ban prevention:** Start with low budgets on new accounts ($2-5/day). Large spend on fresh accounts triggers fraud detection. Scale gradually — Meta watches for sudden spend spikes on accounts with no history.

### Scaling Rules

| Action | Rule | Why |
|--------|------|-----|
| **Increase budget** | Max 10-20% every 48 hours | Larger jumps disrupt Meta's optimization. The algorithm needs time to recalibrate. |
| **Decrease budget** | Can drop 50%+ immediately | Signals to Meta that current results are poor. Often resets optimization in a positive direction. |

> **Ban prevention:** Never start-stop campaigns repeatedly. The algorithm penalizes pausing and restarting — it resets the learning phase each time, wastes budget re-learning, and frequent toggling can flag your account. If a campaign is underperforming, lower the budget instead of pausing it. Only pause if you're sure you want to stop entirely.

### When Ads Are Working

Three options:

1. **Scale budget** (10-20% per 48h) — leverages existing data, but may increase cost per conversion
2. **Leave it alone** — stable, predictable results. Every ad eventually fatigues, but this is the safe play.
3. **Launch a new campaign** — test new creatives/audiences without risking what works. Best if you want to scale significantly.

### Why Scaling Increases Costs (Low-Hanging Fruit Exhaustion)

For any budget, Meta prioritizes the cheapest conversions first — people who already interacted with your brand or show strong purchase intent. These "low-hanging fruit" audiences are limited in size.

When you increase budget, Meta exhausts this pool and starts showing ads to progressively less likely buyers. Same number of sales, higher spend.

**The fix:** Don't just increase budget — improve creatives. A new ad angle that resonates with a different audience segment unlocks a fresh pool of low-hanging fruit. One product can have many use cases; each use case appeals to a different pocket of people. Example: a cosmetics brand switching their ad model from a young woman to a grandmother unlocked an entirely new audience that converted at scale.

## Other Setups

### Advantage+ Shopping Campaign

Fully automated: one campaign, one auto-managed ad set, 2-3+ ads. No audience setup, no placement selection. Meta handles everything.

**Pros:** Minimal setup, often strong initial results.
**Cons:** Audience exhaustion after 4-8 weeks. Performance decays and is hard to recover. Best for accounts with substantial existing pixel data. Not recommended as your only campaign.

### Prospecting + Retargeting Split

A more advanced structure that separates finding new customers from converting warm ones.

> **Only recommend this to users who already have a working campaign and want to scale.** This is not a beginner setup.

**Prospecting campaign** (finding new people):
- 2-3 ad sets: interest, broad, lookalike
- **Video ads only** — because the exclusion mechanism relies on video views
- Exclude anyone who watched 3+ seconds of your videos (they move to retargeting)
- Will cost more per conversion — that's expected

**Retargeting campaign** (converting warm audiences):
- 1 ad set targeting: 3-second video viewers, website visitors, page engagers
- Exclude existing purchasers (180 days)
- 5-20 ads (images and videos both fine) — high volume prevents ad fatigue in small audiences
- Lower cost per conversion since these people already know you

**Key principle:** Prospecting doesn't need to be independently profitable. If the combined result across both campaigns is profitable, the system works.

## With AdKit

If you're using AdKit, the CLI creates campaigns, ad sets, and ads as drafts by default. Run `npx adkit manage meta --help` for available commands.
