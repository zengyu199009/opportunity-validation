---
name: opportunity-validation
description: "Evaluate any business/product idea by checking competitor density FIRST — before you build. Outputs a decision-ready opportunity list with background, use cases, competitor analysis, and monetization path. Built for solo founders, indie hackers, and anyone evaluating AI/SaaS opportunities."
version: 1.3.0
author: zengyu199009
license: MIT
metadata:
  tags: [opportunity, validation, competitor, market-research, saas, ai]
  related_skills: [competitor-news-monitor, multi-search-engine]
  hermes:
    tags: [Opportunity, Validation, Competitor, Demand, Trend]
    related_skills: [competitor-news-monitor, multi-search-engine]
---

# Opportunity Validation (Direction Assessment)

Validate any product/business direction BEFORE you commit to building it. The core rule: **check competitor density first** — most failed solo products die from choosing a red ocean that looked like a blue ocean.

## When to Use

- Someone asks "is this a good idea?" / "which direction should I pursue?" / "what's worth building?"
- You are about to build an AI tool, SaaS, or micro-SaaS and want to avoid wasting months
- You need a quick, evidence-backed scan of niche opportunities
- You're comparing multiple candidate directions and need one decision-ready list

## Core Rule: Competitor Density Check First

**Never recommend a direction without checking competitor density first.** Listing opportunities while skipping the competitor check = recommending red oceans as blue oceans.

Why this matters (real example): in September 2026, three directions — AI visibility/GEO monitoring, local-business AI receptionists, and compliance auditing — all LOOKED like blue oceans but actually had 6-11 mature competitors each. Half of the initial opportunity list was invalidated by one competitor check.

**AI tool niches have a short life cycle: 3-6 months.** A tool that was "open" last month can be saturated this month (example: OtterlyAI was a new category in 2025; by 2026 it had 11+ competitors starting at $29/mo). "It was a gap last month" is NOT a reason to build this month.

## Process

### 0. Intake Checklist (ask first, v1.1)
Collect inputs before evaluating — ask if missing, avoid drift:
- One-line idea + target user + job-to-be-done (who, what it solves)
- Business model (B2B/B2C, SaaS/one-time/marketplace/services)
- Geography & constraints (language, compliance, data requirements)
- Target outcome (venture-scale / cash-flow business / practice)
- Existing evidence (interviews / landing page / pre-sales / users / competitor list)

### 0.5 Assessment discipline (pre-registered rules, v1.1)
**Set standards BEFORE evaluating; do not move the goalposts:**
- Density threshold: ≥5 mature competitors = NO-GO (unless clear differentiation); 3-4 = CONDITIONAL; ≤2 = GO
- Resource budget: ≤8-10 searches per direction, stop when exceeded
- Evidence discipline: weak evidence cannot support a high score/GO — tag each claim: **supported (linked) / inferred / missing** (v1.2)

### 1. Collect candidate directions
Gather demand signals from anywhere: complaint mining, Reddit, Hacker News, GitHub, marketplaces, your own experience. No filtering at this stage.

### 2. Check competitor density for EVERY direction (mandatory — even if nobody asked)

Run searches like:
- `web_search "<keyword> tool 2026"`
- `web_search "<keyword> competitors pricing"`

Find: number of mature products, head players, pricing, user counts / funding.

**Also check: has a giant already built this in?** This is the easiest competitor to miss. Example: employee offboarding knowledge transfer — Rippling/Deel/HiBob/Qualtrics/Culture Amp (9+ enterprise HR platforms) already ship this; independent products only survive in the Chinese-language market gap.

**Check in THREE tiers (v1.1, not just direct competitors):**
- Direct competitors: same problem, same solution
- Indirect competitors: same problem, different solution (easy to miss)
- Substitutes: manual processes / spreadsheets / "do nothing" — often the actual status quo for most people, easiest to miss

**Also check localized/Chinese versions (v1.3, real-world lesson):** many English SaaS products ship Chinese/localized pages — those are direct competitors too. Example: the Chinese idea-validation market has 5-7 tools, half of them Chinese versions of English SaaS; "English vacuum" nearly got misread as "Chinese vacuum". Search `"<keyword> 中文版"` / `"<keyword> 中文"`.

Grade density:
- 🔴 **Red ocean** (5+ mature competitors) → downgrade unless clear differentiation
- 🟡 **Medium** (3-4) → find the specific gap
- 🟢 **Blue ocean** (0-2) → note: blue ocean may also mean "no market" — still need payment evidence

### 2.5 Multi-model cross-check (v1.2)
For key/major directions: run the same direction through 2-3 different models and compare conclusion differences (reduces single-model hallucination). Large divergence → mark "uncertain", do not force-merge.

### 3. Find the remaining gap (not "is there competition" but "where is there NO competition")

- Language/geography gap (e.g., Chinese version, localization)
- Vertical industry gap (single-industry edition)
- Niche scenario gap (the narrower the safer: "audit worksheet structuring" not "Excel AI")
- Pricing model gap (outcome-based vs seat-based)

### 4. Output: 8 fields per direction

For each candidate direction, output:

- **Direction**: one sentence (who, in what situation, why they pay)
- **Background**: why NOW — market context, macro trends, scale data. Distinguish "seen" (has source) vs "estimated" (calculated); every number must be traceable with a link; if you can't find it, write "no data / unverified" — never invent.
- **Use cases**: 2-3 CONCRETE scenarios (who, in what situation, how they use it, what problem it solves) — concrete enough to imagine the user's real day. No vague "improve efficiency" fluff.
- **Payment evidence**: existing products / paying behavior (with links)
- **Competitor analysis**: density (🔴/🟡/🟢) + head players (names + pricing) + maturity + remaining gap + window (3-6 / 6-12 months / ongoing). Based on this round's live check, links traceable.
- **SaaS path**: how to turn it into a SaaS, pricing model
- **Agent feasibility**: ✅ suitable / 🟡 conditional / ❌ not suitable (can OpenClaw/Hermes build/run it)
- **Sources**: 📎 links/data/cases
- **Decision (v1.1)**: GO / CONDITIONAL / PIVOT / NO-GO + one-line next action
- **Validation experiments (v1.1)**: 2-3 cheap experiments — landing page + waitlist / cold outreach / fake door / concierge MVP, each with [cost-time-signal]
- **Target-user discovery (v1.2)**: search Reddit/HN/communities for people actively complaining about the problem; list contacts (username + post link + one-line pain point) for outreach

### 5. Compare existing projects vs new opportunities (when asked)

Put existing projects and new opportunities on the SAME ruler: demand reality × competitor density × window × lightweight-fit (can agents cover it). Give each a grade (🟢 bet on cash flow / 🟡 tight window or many issues / 🔴 red ocean or too long cycle), and honestly mark "information blind spots" (e.g., project code lives on another machine, or a project has no docs).

Conclusion usually lands on: **short-term cash flow = push the project that's already built and one sale away; medium-term validation = the direction with cleanest competitor check; red-ocean projects get downgraded to practice.**

### 6. Honest correction

- If the check overturns a previous judgment (including your own earlier report), **explicitly write "correction: previous judgment invalidated/downgraded"** — no hedging.
- Downgrade or remove red-ocean recommendations, name the competitors and head players.
- Confidence levels: 🟢 high (multi-source verified) / ⚠️ medium (single source + reasonable inference) / ❓ low (big gaps)

## What this skill is NOT (v1.1)

This skill does NOT do: replacement for customer interviews / real-user validation, investor-grade due diligence (DimeADozen-type), or financial model building. It does: fast, evidence-based direction screening + decision + next validation experiments. Real willingness-to-pay must ultimately be confirmed by landing pages / interviews / pre-sales.

## Pitfalls

- ❌ Listing opportunities without checking competitors (the classic failure)
- ❌ Counting only independent products, missing giants' built-in features (HR platforms' offboarding modules are invisible competitors)
- ❌ "No direct competitor" = blue ocean — it may also mean "no market"; you still need payment evidence
- ❌ Using last month's data to judge this month's opportunity (AI tools turn red ocean in 3-6 months)
- ❌ Treating "we can build it" as "people will buy it" (low-tech wrapper ≠ real demand)
- ❌ Skipping the competitor check when the user didn't ask — checking IS the default for any opportunity assessment

## Data Sources (tested)

- GitHub API (api.github.com/search/repositories) — new projects / ecosystem heat
- HN Algolia (hn.algolia.com/api/v1/search — do NOT add `order` param)
- Reddit fallback: `web_search site:reddit.com/r/SaaS`
- BetaList: use web_extract (curl only gets the shell)
- Hugging Face Spaces (6th signal source): `https://huggingface.co/spaces?sort=likes&category=financial-analysis` (also document-analysis / ocr categories + weekly new Spaces). MUST use web_extract (direct API/curl times out). Only look at commercial tool-type Spaces (cross-border payout calculators, vertical document structuring, industry OCR). ⚠️ HF is a model demo community with weak payment signals — Space popularity ≠ payment evidence, treat as a demand hint only.
- Competitor prices/user counts: official pricing pages + tracxn/otterly-type comparison articles + OMR/authoritative lists
- Mark data blind spots honestly: Product Hunt direct / X / V2EX / 36kr / huxiu are often blocked

## References

- `references/2026-09-24-niche-density-map.md` — real density map of 7 long-tail niches measured in Sept 2026 (with red-ocean correction cases), usable as a density baseline
