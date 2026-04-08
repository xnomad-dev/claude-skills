# Claude Skills

A collection of custom Claude skills built for solo creators, entrepreneurs, and content producers. Each skill teaches Claude how to perform a specific task in a repeatable, production-ready way — from writing ad copy to automating email summaries.

---

## Skills

### [gmail-daily-summarizer](gmail-daily-summarizer/)

Automates daily email summarization using Google Apps Script and Claude AI. Monitors Gmail for emails from specific senders over the last 24 hours, summarizes each one using Claude, and saves the results as individual Google Docs in a Google Drive folder. Optionally sends a notification email or Telegram message with links to the summaries. Runs on a daily trigger — no server required.

**Stack:** Google Apps Script · Claude API (Haiku) · Google Drive · Gmail  
**Requires:** Claude API key · Google account · Google Apps Script access  
**Delivers:** Per-sender Google Docs · Daily trigger · Optional Telegram notifications

---

### [video-script-writer](video-script-writer/)

Writes complete, ready-to-film video scripts for solo creators and content producers. Takes a topic, format, and key points and produces a full script with hooks, timed segment breakdowns, B-roll cues, text overlay notes, caption cues for muted viewers, and a shot list. Follows a gated 4-phase workflow — brief → structure → write → deliver — so nothing gets written until the brief and outline are approved.

**Formats:** YouTube long-form · TikTok · Instagram Reels · Tutorials · Talking head  
**Delivers:** Full script with production cues · Shot list · Text overlay list · Caption list · Pre-filming checklist  
**Timing validation:** Word count checked against speaking pace (130–160 WPM) per format

---

### [ad-copy-generator](ad-copy-generator/)

Writes high-converting paid ad copy across every major platform. Follows a 6-phase workflow — brief → primary ads → variations → funnel/retargeting → compliance → delivery. Enforces hard character limits for every platform, generates 3 A/B test variations per platform with a testing matrix, maps copy to cold/warm/hot funnel stages, runs policy compliance checks, and optionally designs ad graphics in Canva using brand kits.

**Platforms:** Meta (Facebook/Instagram) · Google Search (RSA) · Google Display · YouTube · LinkedIn · TikTok · X (Twitter)  
**Delivers:** Primary ads with character counts · 3 variations + A/B matrix · Retargeting sequence · Audience targeting recommendations · Compliance checklist · Optional Canva graphics  
**Formulas:** PAS · AIDA · Before/After · Social Proof · Urgency · FAB

---

## Installation

### Claude Code CLI
```bash
/plugin add /path/to/skill-directory
```

### Claude.ai
1. Go to **Settings > Capabilities**
2. Enable the Skills toggle
3. Upload the skill folder

---

## Structure

Each skill follows the standard Claude Skills format:

```
skill-name/
├── SKILL.md        # Skill instructions with YAML frontmatter
└── scripts/        # Optional executable scripts
```

---

## Author

**xnomad-dev** — [github.com/xnomad-dev](https://github.com/xnomad-dev)
