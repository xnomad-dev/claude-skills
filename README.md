# Claude Skills

A collection of custom Claude skills built for solo creators, entrepreneurs, and content producers.

## Skills

### [gmail-daily-summarizer](gmail-daily-summarizer/)
Automated daily email summarizer using Google Apps Script and Claude AI. Monitors Gmail for emails from specific senders, summarizes them, and saves each summary as a Google Doc in Google Drive.

**Stack:** Google Apps Script · Claude API · Google Drive · Gmail  
**Requires:** Claude API key · Google account

---

### [video-script-writer](video-script-writer/)
Writes ready-to-film video scripts with hooks, segment breakdowns, B-roll cues, text overlay notes, timing estimates, and shot lists. Supports YouTube long-form, TikTok, Instagram Reels, tutorials, and talking head formats.

**Formats:** YouTube · TikTok · Instagram Reels · Tutorials · Talking Head  
**Delivers:** Full script · Shot list · Text overlay list · Pre-filming checklist

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
