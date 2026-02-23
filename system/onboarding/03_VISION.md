# Onboarding Step 3: Your Vision

**Goal:** Generate `My_Foundation/My_Vision.md` + create monthly entry folders
**Prerequisites:** `My_Journey_Context.md` and `My_Baseline.md` must exist
**Estimated time:** 15-20 minutes
**Next step:** Step 4 — Customize Your System (say "continue setup" or "next step")

---

## Instructions for Claude

Before starting, read both:
- `My_Foundation/My_Journey_Context.md`
- `My_Foundation/My_Baseline.md`

Open with:
"You've mapped where you've been and where you are. Now the most important part — where you're going. This isn't a goal list. I'm going to ask you to describe a day in your future life as if you're already living it."

## Timeline Selection

"First — how long do you want this journey to be?"

- **3 months** (90 days) — intense sprint
- **6 months** (180 days) — standard journey, enough for real identity shift
- **9 months** (270 days) — deeper work, more gradual
- **1 year** (365 days) — full transformation cycle

Record their choice. Calculate start date (today), end date, total days, number of months.

## The Future Day Exercise

"Close your eyes for a second if you want. It's [end date]. You wake up. Walk me through this day — not what you hope for, but what you SEE. First person, present tense, like you're living it."

Guide with prompts:
- "Where are you when you wake up?"
- "What's the first thing you do?"
- "Who do you interact with? How do those conversations feel?"
- "What are you working on? How does work feel?"
- "How does your body feel?"
- "What does your evening look like?"

**Critical:** Capture in THEIR voice. First person. Present tense. Rich with sensory and emotional detail. If they default to bullet points, redirect: "Don't tell me what you want. Tell me what you see."

## Key Domains

Based on all conversations, identify 4-8 key life domains. Suggest common ones, let them add/remove:
- Business / Career
- Financial
- Health / Body
- Relationships / Intimacy
- Family / Parenting
- Social / Community
- Creative / Expression
- Legal (if applicable)
- Spiritual / Consciousness

## When Complete

1. Read the vision narrative back. Ask: "Does this feel real? Does it pull you forward?"

2. Once confirmed, generate `My_Foundation/My_Vision.md`:

```markdown
---
title: "[END DATE] Reality"
date_created: [TODAY'S DATE]
tags:
  - vision
  - future-reality
---

# [END DATE] Reality

[Full first-person vision narrative — their future day, in their voice]

## Key Domains
- [Domain 1]
- [Domain 2]
- [etc.]

## Timeline
- **Start date:** [DATE]
- **End date:** [DATE]
- **Duration:** [X] months / [X] days
```

3. **Create monthly entry folders** in `Entries/`:
   One folder per calendar month: `Month_01_[MonthName]/`, `Month_02_[MonthName]/`, etc.

4. **Create the `Monthly_Summaries/` folder** if it doesn't already exist.

4. Tell the user: "Step 3 is done — your vision is saved and your monthly folders are created. One more step: customizing the system. Say 'continue setup' or 'next step' whenever you're ready."

## Constraints
- The future day exercise is the emotional core — invest time here.
- Capture their words, their metaphors, their language.
- Never judge the scale of their vision.
