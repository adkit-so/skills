---
name: google-ads-strategy
displayName: "Google Ads Strategy: Search Campaigns, Keywords, Ad Copy, Negative Keywords, Quality Score"
description: >
    Run Google Search Ads end-to-end: keyword mining, account structure, ad copy,
    negative keyword architecture, and performance analysis. Covers the full loop
    from setup to ongoing optimization for B2B SaaS and app makers. Use when the
    user wants to plan, launch, or optimize Google Search campaigns, or understand
    how the platform works before spending. Not for Meta Ads, TikTok Ads, LinkedIn
    Ads, or Google Display/YouTube campaigns.
version: 0.1.0
metadata:
    openclaw:
        homepage: https://adkit.so
triggers:
    - google ads
    - search ads
    - google search campaign
    - ppc
    - keyword research
    - negative keywords
    - quality score
    - ad copy google
    - roas google
    - cpc
    - ad group structure
    - search term report
    - google ads not working
    - optimize google ads
    - scale google ads
    - responsive search ads
    - rsa
    - smart bidding
    - target cpa
    - conversion tracking google
---

# Google Ads Strategy

Guide Google Search Ads strategy decisions. Ask before advising, tailor every recommendation to the user's situation. Reply in the same language as the user.

## First: check context

<!-- ad-process.md and ad-brief.md are looked up by filename, not path. Users can store them anywhere in their project. Do not rename these files. -->

1. Search the project for a file named `ad-process.md`. If found, read it and apply the user's preferences (naming, structure, budgets, etc.) to all recommendations. Read the `## General` and `## Google` sections. If the user shares preferences but no file exists, offer to create one. Save only specific preferences and conventions, not general strategy advice.
2. Search the project for a file named `ad-brief.md`. If found, use it. If not found, ask the user for the key inputs needed: product, audience, main offer, target CPA or ROAS goal, monthly budget.
3. Proceed to the routing table below.

## Core Principles (always apply these)

1. **Relevance wins auctions. Ad Strength does not.** Google rewards keyword → ad → landing page relevance with lower CPCs and higher positions. Ad Strength is a diagnostic metric, not the goal.
2. **Mine real query language.** Keywords should come from verbatim customer language — interviews, reviews, search term reports — not Keyword Planner fantasy. Keyword Planner is for sizing, not discovery.
3. **Campaigns by intent, ad groups by theme.** Split campaigns only when they need different budget, bidding, geo, or reporting. Each ad group maps to one landing page — one story, one page.
4. **Negatives are the other half of relevance.** Without a negative architecture, broad and phrase match leak budget to searchers who can't buy what you sell. Build the negative list before launching.
5. **Launch is not set-and-forget.** The Search Term Report is your primary feedback signal. Review it weekly for 60 days, then monthly. Each unexpected term is a decision: promote, demote, or ignore.
6. **Build modular ads, not score bait.** Write ad assets as a modular system — each headline earns its slot. Pin for learning speed early on; unpin after convergence.
7. **Conversion tracking first, always.** Smart bidding (Target CPA, Target ROAS) is only as good as the conversion data feeding it. Never run a campaign without verified conversion tracking.

## Routing table

Read the user's situation, then address the relevant phase:

| User says...                                                        | Address this                      |
| ------------------------------------------------------------------- | --------------------------------- |
| "I've never run Google Ads" / "How does it work?"                   | Fundamentals + Core Principles    |
| "Help me find keywords" / "What should I bid on?"                   | Keyword Mining (§1)               |
| "How do I structure my account?" / "Campaigns vs ad groups?"        | Account Structure (§2)            |
| "Help me write ad copy" / "How many headlines?"                     | Ad Copy (§3)                      |
| "What negatives do I need?" / "Budget leaking"                      | Negative Keywords (§4)            |
| "My ads aren't working" / "CPC is too high" / "Low CTR"             | Analyze Loop (§5) + diagnostics   |
| "I'm ready to scale" / "CPA came down, what next?"                  | Scale guidance in §5              |

**Address only the relevant section.** Don't dump all phases at once. Start where the user is.

---

## §1 — Keyword Mining: Gather Language, Not Planner Fantasy

Real queries come from real people. Mine verbatim language from sources your customers already own.

**Best sources (ranked by authority):**
- Customer interviews and sales calls — exact objections and vocabulary
- G2, Capterra, App Store reviews — how buyers describe the problem
- Competitor brand terms + "[competitor] alternative" patterns
- Google Autosuggest and related searches
- Search Console queries (if the site has organic traffic)
- Existing Search Term Reports (if the account has history)

**Intent classification — prioritize by paid ROI:**
- **Transactional** (buy, pricing, trial, demo) → highest priority, bid first
- **Commercial** (best, top, compare, alternative) → second priority
- **Informational** (how to, what is) → generally avoid for search spend; use for content
- **Navigational** (brand name, competitor brand) → brand campaign + competitor conquest

**Keep filters:**
- Clear 2-month intent-to-buy signal (someone searching this is in market)
- Long-tail preferred over head terms (less competition, higher intent signal)
- Retargeting potential if they don't convert

**Keyword Planner's role:** volume estimates and CPC ranges only. Never use it as the primary discovery source — it recycles popular vocabulary, not buyer language.

---

## §2 — Account Structure: Campaigns by Intent, Ad Groups by Theme

**Decision rule:** split into separate campaigns only when they need different budget, bidding strategy, geo, language, or reporting. Everything else stays in the same campaign.

**Ad group rule:** one ad group = one landing page. Each ad group tells one story. If the landing page would need to change, that's a new ad group.

**Target size:** 5–15 keywords per ad group. More dilutes relevance. Fewer limits match coverage.

**Typical B2B SaaS campaign structure (days 0–60):**
- Brand (protect your name, low budget, high ROAS)
- Competitor conquest (alternative/vs terms, separate budget, different bidding)
- Solution-aware (problem + category terms, largest budget)
- Problem-aware (pain-point queries, lower intent, lower bids)

**Match type by maturity:**
- New account, low volume → start with phrase match. Broad match needs conversion data to work.
- 30–50 conversions/month per campaign → test broad match with Target CPA. Never broad match without smart bidding.
- Brand campaign → always exact match.

---

## §3 — Ad Copy: Modular Relevance System

Write ads as a modular relevance system. Each asset earns its place.

**RSA structure — three headline pools:**
- **H1 (attention):** keyword echo or pain point — pin to position 1 during learning
- **H2 (interest):** key differentiator or proof point — pin to position 2 during learning
- **H3 (friction reduction):** objection handler, social proof, or offer — rotate from pool

**Sizing:**
- 8–10 headlines total (3 pinned + 5–7 pool)
- 2–3 descriptions (1 pinned for brand consistency, 1–2 rotating)

**Pinning strategy:**
- Pin H1 and H2 during the first 4–6 weeks so Google reports meaningful asset performance data
- Unpin H3 pool immediately to let Google optimize
- After convergence (4–6 weeks), unpin H1/H2 and let it run

**Supporting assets (add all of these before launching):**
- Sitelinks (4–6): send to specific pages, not homepage
- Callouts: facts, not features ("No setup fees", "SOC 2 certified")
- Structured snippets: category lists (features, integrations, platforms)
- Image extensions if visual proof exists

**What to avoid:**
- Keyword stuffing — Google rewards natural language now
- Disabling ACA (Automatically Created Assets) carelessly — review first, then disable if quality is low
- Writing for Ad Strength score — write for the human, let the score follow

---

## §4 — Negative Keyword Architecture

Negatives are the other half of relevance. Build three lists:

**List 1: Global Exclusions (apply to all campaigns)**
Intent categories to block everywhere:
- Educational / research: "what is", "definition", "meaning", "explained", "course", "learn"
- Jobs / hiring: "jobs", "careers", "salary", "hiring", "internship", "resume"
- Free / open-source: "free", "open source", "github", "freeware", "crack", "torrent"
- Wrong product collision: terms that share your product's name but mean something else

**List 2: Non-Commercial (apply to solution + problem campaigns)**
- Review and list sites: "reddit", "quora", "forum", "community"
- Comparison bait without intent: "vs", "compare" (keep in competitor campaign, remove from solution)
- DIY signals: "how to build", "diy", "template", "tutorial"

**List 3: Campaign-Specific**
- Keep competitor terms out of brand campaign
- Keep brand terms out of competitor campaign (usually — check search volume)
- Suppress geo terms irrelevant to your targeting

**Review cadence:**
- Weekly for the first 60 days: every new search term is a signal
- Monthly after 60 days: drift is slower once the account matures

**The three-way decision for every unexpected search term:**
1. On-intent, enough volume → add as a keyword in the right ad group
2. Off-intent → add as a negative at the appropriate scope
3. One-off noise → ignore for now, flag if it recurs

---

## §5 — The Analyze Loop

Launch feeds the loop. The loop tightens the system. There is no "done."

**Weekly review (first 60 days):**
1. Open Search Terms Report → three-way decision on every new term
2. Check Asset Report → unpin headlines that are "Low", add new variants
3. Check ad group CVR vs account median → ad groups below median need a dedicated landing page

**Monthly review (after 60 days):**
1. Search Terms Report (same as above, lighter cadence)
2. Quality Score by keyword → Low QS = relevance gap (keyword, ad, or page)
3. Budget utilization → underspend = bid/relevance problem, not budget problem
4. Auction Insights → new competitors or share shifts signal market changes

**Scaling signals (do all three before scaling budget):**
- CPA at or below target for 2+ consecutive weeks
- Conversion volume ≥ 30/month per campaign (enough data for smart bidding)
- Search Impression Share < 60% (room to grow before hitting ceiling)

**Scaling method:**
- Increase budget 20–30% at a time, wait 7 days before next increase
- Don't change bids and budget simultaneously — can't diagnose what moved CPA
- New ad groups beat higher bids for sustainable scale

---

## Execution: manual vs AdKit

When the user reaches an execution step (keyword uploads, campaign creation, ad publishing), check if AdKit CLI is installed by running `adkit status`.

- **AdKit is installed:** use the CLI by default. The user is already a customer — this is the faster path.
- **AdKit is not installed:** walk them through Google Ads Manager UI step by step. You can mention that [AdKit](https://adkit.so?utm_source=skills) has a CLI that automates campaign operations, but default to the manual path. Don't push it — the strategy above works entirely through the Google Ads interface.
