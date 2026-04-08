---
name: ad-copy
description: "Writes high-converting ad copy for Meta (Facebook/Instagram), Google (Search, Display, YouTube), LinkedIn, TikTok, and X with platform-native variations, funnel-stage targeting, policy compliance checks, and optional Canva graphics. Use when a user needs paid ad copy, is launching campaigns, needs A/B test variations, or is building retargeting sequences."
allowed-tools: Read, Write, WebFetch, mcp__claude_ai_Canva__generate-design, mcp__claude_ai_Canva__generate-design-structured, mcp__claude_ai_Canva__resize-design, mcp__claude_ai_Canva__export-design, mcp__claude_ai_Canva__get-export-formats, mcp__claude_ai_Canva__list-brand-kits, mcp__claude_ai_Canva__get-design-thumbnail
metadata:
  author: AI Black Magic
  version: "2.0"
  last_verified: "2026-04"
---

# Ad Copy Generator

EVERY AD MUST BE NATIVE TO ITS PLATFORM, FIT ITS FUNNEL STAGE, PASS POLICY REVIEW, AND HIT CHARACTER LIMITS EXACTLY.

## When to Use This Skill

- User needs paid ad copy for Meta, Google, LinkedIn, TikTok, X, or YouTube
- User is launching a campaign and needs platform-native variations
- User wants A/B test variations for existing ads
- User needs a cold → warm → hot retargeting sequence
- User needs ad graphics designed in Canva alongside copy
- User asks for audience targeting or policy compliance review

---

## Phase 1: Brief

Gather these inputs before writing a single word of copy. **Required** items gate Phase 2; the rest improve quality but can be inferred or deferred.

### Required (gate Phase 2)
1. **Product/Service** — Name, core value prop, key differentiator
2. **Target Audience** — Who the ideal customer is
3. **Platform(s)** — At least one
4. **Offer/CTA** — What action the viewer should take

### Recommended (ask if reasonable, default if not)
5. **Objective** — Awareness, Consideration, or Conversion (default: Conversion)
6. **Funnel Stage** — Cold, Warm, or Hot audience (default: Cold for new campaigns)
7. **Landing Page URL** — Fetch it to align messaging
8. **Brand Voice** — Default: professional-casual
9. **Regulated Industry?** — Health, finance, crypto, gambling, alcohol, political (triggers Phase 5 compliance checks)
10. **Canva Graphics** — Y/N

### Brief Template (Filled Example)

```
Product:       Taskflow — AI project management for solo founders
Audience:      Solopreneurs, 25–45, overwhelmed by tool sprawl
Platforms:     Meta, Google Search
Offer:         14-day free trial, no credit card
Objective:     Conversion
Funnel Stage:  Cold
Landing Page:  https://taskflow.app/start
Brand Voice:   Confident, direct, founder-friendly
Regulated:     No
Canva:         Yes — Meta feed image
```

**GATE: Do not proceed until product, audience, at least one platform, and CTA are confirmed. Ask directly for any missing required item. If the user requests ads for 3+ platforms at once, ask whether they want full variation sets for all, or primary platform first.**

---

## Phase 2: Write Primary Ads

Write one primary ad per platform using the specs below. **Count every character.** Choose the formula that fits the funnel stage and audience.

### Ad Copy Formulas

| Formula | Structure | Best For |
|---|---|---|
| PAS | Pain → Agitate → Solve | Conversion, problem-aware audiences |
| AIDA | Attention → Interest → Desire → Action | Awareness, cold audiences |
| Before/After | Old way vs. new way | Product launches, differentiators |
| Social Proof | Result + proof + CTA | High-trust offers, testimonials |
| Urgency | Time/scarcity pressure + CTA | Limited offers, launches |
| FAB | Features → Advantages → Benefits | B2B, complex products |

Defaults: **PAS** for conversion, **AIDA** for awareness, **Social Proof** for retargeting warm audiences.

### Platform Format Specs

All specs verified April 2026. Character limits are hard caps — over-limit copy is rejected at upload.

#### Meta (Facebook / Instagram)

| Element | Limit | Notes |
|---|---|---|
| Primary text | 125 chars above fold (up to 500 total) | Front-load the hook in the first 125 chars |
| Headline | 27 chars recommended (40 max) | 40 often truncates on mobile; 27 is the safe bar |
| Description | 27 chars recommended (30 max) | Optional, often hidden |
| CTA button | Preset only | Shop Now, Learn More, Sign Up, Book Now, Download, Get Offer |

**Primary Ad Example (Taskflow — Meta, PAS, Cold audience):**

```
Primary text (110 chars):
You're juggling 6 tools to manage one business. Taskflow replaces them all with AI that knows your priorities.

Headline (27 chars): Stop Managing. Start Doing.
Description (27 chars): Free 14-day trial. No card.
CTA Button: Sign Up
```

#### Google Responsive Search Ads (RSA)

Expanded Text Ads were sunset in 2022. RSAs are the only Search format now.

| Element | Per-asset limit | Count |
|---|---|---|
| Headlines | 30 chars each | Provide 10–15 (min 3, max 15) |
| Descriptions | 90 chars each | Provide 3–4 (min 2, max 4) |
| Display path | 15 chars each | 2 paths (cosmetic) |
| Business name | 25 chars | Optional |
| Final URL | 2,048 chars | — |

Google shows 2–3 headlines and 1–2 descriptions per impression. Each headline must make sense standalone and next to any other headline. Pin sparingly — pinning kills Google's combination testing.

**Primary Ad Example (Taskflow — Google RSA, Cold audience):**

```
Headlines (provide all):
1.  AI Project Management Tool      (26)
2.  Built for Solo Founders          (23)
3.  Start Free — No Credit Card      (27)
4.  Replace 6 Apps with Taskflow     (28)
5.  Manage Projects with AI          (23)
6.  14-Day Free Trial                (17)
7.  Ship Faster, Stress Less         (24)
8.  Your AI Project Manager          (23)
9.  Built by Founders, for Founders  (31)
10. Taskflow for Solopreneurs        (25)

Descriptions (provide all):
1. Stop juggling 6 apps. Taskflow uses AI to prioritize your tasks and ship projects. (82)
2. Trusted by solo founders worldwide. 14-day free trial with full features included. (82)
3. Replace your project stack with one AI tool. No credit card required. Start today. (82)
4. Built for solo operators. Smart priorities, automatic tracking, zero setup needed. (82)

Display path: /solo-founders/free-trial
```

#### Google Responsive Display

| Element | Limit | Count |
|---|---|---|
| Short headlines | 30 chars each | Up to 5 |
| Long headline | 90 chars | 1 |
| Descriptions | 90 chars each | Up to 5 |
| Business name | 25 chars | 1 |
| Marketing images | 600×314+ | Up to 15 |

Long headlines must stand alone — they sometimes display without the description.

**Primary Ad Example (Taskflow — Responsive Display):**

```
Short headlines:
1. Manage Less. Build More.       (24)
2. AI for Solo Founders           (20)
3. Replace 6 Apps with One        (23)
4. Start Free Today               (16)
5. 14-Day Free Trial              (17)

Long headline (62):
AI project management that replaces 6 tools for solo founders.

Descriptions:
1. Taskflow prioritizes your tasks automatically. 14-day free trial, no card. (74)
2. Built for operators running businesses alone. Start in under 2 minutes. (71)

Business name: Taskflow
```

#### LinkedIn Sponsored Content

| Element | Limit | Notes |
|---|---|---|
| Intro text | 150 chars above fold (up to 600 total) | Front-load the hook |
| Headline | 70 chars (under 150 for news feed compat) | Below image |
| Description | 100 chars | Below headline, often hidden |
| CTA button | Preset only | Learn More, Sign Up, Download, Register, Apply Now |

**Primary Ad Example (Taskflow — LinkedIn, Before/After):**

```
Intro text (132 chars):
Before Taskflow: spreadsheets, sticky notes, and 3pm panic. After Taskflow: one AI dashboard that runs your entire project pipeline.

Headline (39 chars): AI Project Management for Solo Founders
Description (42 chars): 14-day free trial. No card. Full features.
CTA Button: Sign Up
```

#### TikTok In-Feed Ads

| Element | Limit | Notes |
|---|---|---|
| Ad caption | 100 chars (Latin), 50 chars (Asian scripts) | 4 lines max visible |
| Brand/app name | 2–20 chars (brand), 4–40 chars (app) | Preset field |
| CTA button | Preset only | Shop Now, Learn More, Sign Up, Download, Book Now, Contact Us |

**Critical restrictions:**
- **No emojis** in the caption on non-Spark ads (automatic rejection)
- **No `#` or `{ }`** characters
- **No clickable links or hashtags** in non-Spark captions
- Spaces and punctuation count
- Vertical 9:16 video required; watermarks from other apps = rejection

**Primary Ad Example (Taskflow — TikTok, Hook-first):**

```
Caption (94 chars):
POV: your to-do list manages itself. Taskflow uses AI so solo founders can actually ship work.

Brand name: Taskflow
CTA Button: Sign Up
```

#### X (Twitter) Promoted Posts

| Element | Limit | Notes |
|---|---|---|
| Post copy | 280 chars (257 if link included) | URLs always count as 23 chars via t.co wrapping |
| Website card headline | 70 chars | Appears under image on Website Cards |
| Website card description | 200 chars | Often truncated at ~50 chars on mobile |

**Critical:**
- Emojis count as **2 characters each** (Unicode double-width)
- X Premium's 25,000-char limit does **not** apply to promoted posts — still 280
- 100–150 chars performs best for engagement

**Primary Ad Example (Taskflow — X Promoted Post with link):**

```
Post copy (201 chars + 23 link = 224 total):
Solo founders: you didn't start your business to babysit 6 project tools.

Taskflow is one AI dashboard that prioritizes, tracks, and ships your work. Free for 14 days, no card.

https://taskflow.app/start

Website card headline (36 chars): AI Project Manager for Solo Founders
Website card description (42 chars): 14-day free trial. No card. Full features.
```

#### YouTube (Skippable In-Stream & Shorts Ads)

Run through Google Ads. Text often hidden on TV and mobile app placements — **your video must carry the full message.**

| Element | Limit | Notes |
|---|---|---|
| Headline (in-stream) | 15 chars | Extremely tight |
| Long headline (in-stream) | 90 chars | Alternative |
| Description | 70 chars (two lines, ~35 each) | Often hidden on TV/desktop |
| CTA button | 10 chars | Shop Now, Learn More, Sign Up, Get App |
| Video length (skippable) | 12 sec – 6 min | Hook in first 5 sec before skip |
| Video length (bumper) | 6 sec max | Non-skippable |
| Video length (non-skippable) | 15–30 sec | Guaranteed view |

**Primary Ad Example (Taskflow — YouTube Skippable):**

```
Headline (11 chars): Ship Faster
Long headline (54): AI Project Management for Founders Who Do It All Alone
Description (61): Replace 6 tools with one AI dashboard. 14-day trial, no card.
CTA button (8): Try Free

Video direction: 5-sec hook showing tab overload → Taskflow dashboard
→ demo of AI prioritization → brand + CTA. Total: 15–20 seconds.
```

**GATE: Verify every character count before proceeding. Rewrite anything over limit. Do not present over-limit copy.**

---

## Phase 3: Creative Variations

Generate **3 variations per platform** using different hooks, formulas, or audience angles. For multi-platform requests with 3+ platforms, ask if the user wants full variations for every platform or just the primary.

### Variation Strategy

| Variation | What Changes | Why |
|---|---|---|
| V1 (Hook shift) | Opening line uses a different emotional trigger | Tests which pain point resonates |
| V2 (Angle shift) | Different formula (e.g., PAS → Social Proof) | Tests messaging framework |
| V3 (Audience shift) | Different audience segment or use case | Tests audience targeting |

### A/B Testing Matrix

Always include this table so the user knows what is being tested:

```
Platform: Meta
| Version | Hook                    | Formula       | Audience     | Key Difference      |
|---------|-------------------------|---------------|--------------|---------------------|
| Primary | Pain (tool overload)    | PAS           | Solopreneurs | Baseline            |
| V1      | Fear (missed deadlines) | PAS           | Solopreneurs | Different pain      |
| V2      | Proof (customer wins)   | Social Proof  | Solopreneurs | Formula change      |
| V3      | Ambition (scale faster) | AIDA          | Freelancers  | Audience shift      |
```

### Meta V1 Example (Hook shift — missed deadlines)

```
Primary text (124 chars):
Missed another deadline? When you're the whole team, one dropped ball costs you a client. Taskflow keeps every ball in play.

Headline (27 chars): Never Miss a Deadline Again
Description (27 chars): Free 14-day trial. No card.
CTA Button: Sign Up
```

### Meta V2 Example (Angle shift — Social Proof)

Only use real numbers the user confirmed. This example assumes the user confirmed "thousands of solo founders" — do not invent metrics.

```
Primary text (116 chars):
Solo founders keep switching to Taskflow to manage projects in half the time. Your free trial is ready when you are.

Headline (23 chars): Built for Solo Founders
Description (27 chars): Free 14-day trial. No card.
CTA Button: Sign Up
```

### Meta V3 Example (Audience shift — freelancers)

```
Primary text (119 chars):
Freelancers: you started this for freedom, not for 3 hours a day of project admin. Taskflow gives you those hours back.

Headline (25 chars): Freelance Hours, Returned
Description (27 chars): Free 14-day trial. No card.
CTA Button: Sign Up
```

### Optional: Canva Ad Graphics

If the user requests graphics:

1. Check for existing brand kits with `list-brand-kits` and apply if available
2. Generate at platform-native sizes:
   - Meta feed: 1200×628 or 1080×1080
   - Instagram Stories / TikTok / Shorts: 1080×1920
   - LinkedIn: 1200×627
   - X image: 1200×628 or 1200×1200
   - YouTube thumbnail / companion banner: 1280×720 or 300×60
   - Responsive Display: 1200×628 + 1200×1200
3. Include headline + CTA on graphic; keep key elements out of TikTok's right-side UI and bottom caption bar
4. Thumbnail preview for approval before exporting
5. Export PNG

**GATE: All variations must stay within platform limits. Re-count every variation before presenting.**

---

## Phase 4: Funnel Stage & Retargeting

Most skills treat ads as one-shots. Real campaigns are sequences. Ask which stage the user is writing for — or write a full sequence if they're running retargeting.

### Funnel Stage Mapping

| Stage | Audience | Goal | Best Formulas | Copy Shift |
|---|---|---|---|---|
| **Cold (TOFU)** | No brand awareness | Educate, capture attention | AIDA, PAS, Before/After | Lead with the problem, not the product. Hook must be curiosity or pain |
| **Warm (MOFU)** | Visited site, engaged, didn't buy | Move to consideration | Social Proof, FAB, PAS | Address objections. Show proof. Reduce perceived risk |
| **Hot (BOFU)** | Abandoned cart, high-intent, list members | Close | Urgency, direct offer, testimonials | Specific offer + deadline. No re-education. Remove friction |

### Retargeting Sequence Example (Taskflow, Meta)

**Cold (Day 0 — Interest targeting):**
```
Primary text (110 chars):
You're juggling 6 tools to manage one business. Taskflow replaces them all with AI that knows your priorities.
Headline: Stop Managing. Start Doing.
CTA: Learn More
```

**Warm (Day 1–7 — Website visitors, no signup):**
```
Primary text (117 chars):
Still weighing project management tools? Taskflow handles prioritization, tracking, and planning in one AI dashboard.
Headline: One Tool. Every Project.
CTA: Learn More
```

**Hot (Day 7–14 — Signup page visitors who didn't convert):**
```
Primary text (120 chars):
Your Taskflow trial is still open. 14 days free, no card, full features. Start in under 2 minutes — your workflow waits.
Headline: Your Free Trial Awaits
CTA: Sign Up
```

### Frequency & Rotation

- **Cold:** Rotate 3+ creatives every 5–7 days to fight ad fatigue
- **Warm:** 2–3 creatives, refresh every 10–14 days
- **Hot:** 1–2 direct-offer ads, refresh every 7 days (smaller audience, burns faster)
- **Exclude converters** from all stages to avoid wasted spend

---

## Phase 5: Compliance & Policy Checks

Run this checklist for every ad before delivery. Rejected ads waste budget and trip account-level strikes.

### Universal Policy Rules (All Platforms)

- [ ] **No unverified claims.** "Cure," "guaranteed results," "100% effective" — rejected or restricted on every platform
- [ ] **No superlatives without proof.** "Best" / "#1" / "world-leading" without citation is restricted on Meta and LinkedIn
- [ ] **No negative personal attributes.** "Are you overweight?" / "Struggling with debt?" — Meta rejects these as calling out assumed attributes; rephrase as aspirational ("Reach your fitness goals")
- [ ] **No before/after images** for weight loss, cosmetics, or health on Meta
- [ ] **No fake engagement bait.** "Click here," "Like if you agree" triggers demotion on Meta/TikTok
- [ ] **No all caps** in body copy (all platforms) — allowed on recognized abbreviations only (FAQ, USA). Google auto-rejects.
- [ ] **No deceptive clickbait.** Copy must match the landing page
- [ ] **No trademarked brand names** you don't own (competitor brand bidding is restricted)
- [ ] **No prohibited symbols** on specific platforms: TikTok rejects emojis in non-Spark captions; Google rejects emojis entirely; X allows emojis but they count as 2 chars

### Regulated Industry Flags

If the user's product falls in any of these categories, flag it and add the platform-specific warning:

| Category | Restrictions |
|---|---|
| **Health / supplements** | No disease claims. Meta requires "results not typical" disclaimers. Google restricts prescription terms. LinkedIn bans most consumer health. |
| **Finance / credit / crypto** | Required licensure in ad copy on Meta/Google. No guaranteed returns. Most platforms ban unregistered crypto ads. |
| **Alcohol** | Age-gated targeting mandatory. Cannot imply social/sexual success. Banned in some countries regardless. |
| **Gambling** | License pre-approval required on Meta, Google, TikTok. Geo-restrictions enforced. |
| **Political / social issues** | Advertiser verification required (Meta, Google, X, TikTok). Disclosure label mandatory. |
| **Dating** | Pre-approval on Meta. No suggestive imagery. LinkedIn bans entirely. |
| **Weight loss / body image** | Cannot show "ideal bodies" implied as comparison. Cannot target based on body attributes. |

### Landing Page Alignment Check

- [ ] Headline claim matches the H1 on the landing page
- [ ] Offer in the ad (price, discount, free trial terms) matches what the visitor sees on arrival
- [ ] CTA in the ad matches the first CTA on the page
- [ ] If the landing page requires payment info, the ad does not imply "free"

---

## Phase 6: Deliver

### Delivery Format

For each platform, present:

1. **Primary Ad** — Full copy with character counts per element
2. **Variations V1–V3** — Full copy with the A/B testing matrix
3. **Audience Targeting** — 2–3 recommendations
4. **Funnel Notes** — Which stage this ad serves and what comes next
5. **Compliance Flags** — Any Phase 5 items that need the user's attention
6. **Graphics** — Canva exports if requested

### Audience Targeting Cheat Sheet

**Meta:** Interest stacks (3–5 overlapping interests), Lookalike (1%, 3%, 5% tiers from email list), Custom audience (website visitors 30/60/90-day, video viewers 75%+, engagers).

**Google Search:** Exact match for brand, phrase match for primary intent, broad match for discovery. Negative keywords list (always include "free," "jobs," "download torrent" unless relevant).

**LinkedIn:** Job title + seniority + company size. Avoid interest-only targeting (too broad). Exclude current customers.

**TikTok:** Interest categories + behavior (video engagement in last 15 days). Age/gender restrictions for regulated categories. Use Creator Marketplace for Spark Ads.

**X:** Keyword targeting (what users tweet/search), follower lookalike (target accounts your audience follows), conversation topics.

**YouTube:** In-market audiences (active buyers), custom affinity, topic + placement targeting, remarketing lists from YouTube channel + website.

### Pre-Delivery Checklist

- [ ] Every element within platform character limit (recount from scratch, do not trust earlier counts)
- [ ] Character counts displayed next to each element
- [ ] Each platform has 1 primary + 3 variations (or user-agreed scope)
- [ ] A/B testing matrix included per platform
- [ ] Copy matches the confirmed offer and CTA
- [ ] Funnel stage is identified for each ad
- [ ] No pricing mentioned unless user confirmed it
- [ ] No statistics or testimonials fabricated — real numbers from the brief only
- [ ] Landing page messaging aligns (if URL provided and fetched)
- [ ] Targeting recommendations included
- [ ] Phase 5 compliance checks run and flagged
- [ ] Canva graphics exported if requested
- [ ] Brand voice consistent across ads and platforms

---

## Anti-Patterns

- **DO NOT exceed character limits** — count every character, every time, on every variation
- **DO NOT fabricate numbers, testimonials, or social proof** — if the user didn't give you a stat, you don't have one
- **DO NOT use clickbait that mismatches the landing page** — this is a policy violation, not just bad practice
- **DO NOT write identical copy across platforms** — Meta is visual-emotional, Google is intent-based, LinkedIn is professional, TikTok is native/casual, X is conversational, YouTube is video-first
- **DO NOT use ALL CAPS in body copy** — Google auto-rejects; Meta/LinkedIn demote
- **DO NOT include emojis in TikTok non-Spark captions or any Google Search ad** — automatic rejection
- **DO NOT include pricing or offer details the user didn't confirm** — assumed specifics break trust
- **DO NOT use generic CTAs like "Click Here"** — every CTA must be specific to the action
- **DO NOT stuff keywords in Google RSAs** — write 10+ distinct headlines, each standalone
- **DO NOT pin every Google RSA headline** — pinning kills Google's combination testing
- **DO NOT skip the funnel stage question for multi-ad requests** — a cold ad and a hot ad require different copy
- **DO NOT ignore Phase 5 compliance** — a rejected ad wastes more time than a careful check
- **DO NOT present variations without the A/B testing matrix**
- **DO NOT generate Canva graphics without checking brand kits first**

---

## Recovery

**No landing page URL provided:**
Write copy from the product description. Flag that reviewing the landing page would improve alignment, offer to revise once a URL is available.

**Landing page URL unfetchable (paywall, JS-heavy, auth required):**
Tell the user you couldn't read the page. Ask for the H1, primary offer, and first CTA text. Proceed with those.

**Unknown target audience:**
Ask for the best customer in one sentence. If the user can't describe it, default to the broadest reasonable segment and flag that narrower targeting improves performance.

**Budget or objective unclear:**
Default to conversion. Most small businesses need direct-response, not brand awareness. Mention the assumption and offer to adjust.

**Funnel stage not specified:**
Default to cold (TOFU). Note the assumption and offer a retargeting sequence if the user has existing traffic.

**Regulated industry:**
Do not refuse. Write the copy, run Phase 5 flags, and make the restrictions explicit so the user can adjust or add required disclosures. If a category is banned on a platform the user requested, say so and suggest an alternate platform.

**Platform not listed in specs:**
This skill covers Meta, Google (Search, Display, YouTube), LinkedIn, TikTok, and X. For Pinterest, Reddit, Snapchat, or others, write copy following the closest analog platform and note that character limits should be verified against the platform's current specs before upload.

**Three revision attempts fail:**
Stop revising. Ask for an example ad the user admires or a competitor they want to emulate. Use it as a style anchor and restart from Phase 2.

**Canva integration unavailable:**
Deliver copy with image specs (dimensions, recommended overlay text, visual direction) so the user can create graphics manually or elsewhere.
