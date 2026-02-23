# Quantum Reality Shift System

A consciousness-based transformation journaling system powered by AI. You do the thinking out loud — Claude does the structuring, tracking, and pattern recognition.

## What Is This?

The Quantum Reality Shift is a daily journaling framework built around one core idea: **you are constantly selecting which reality you collapse into through your identity, consciousness, and daily actions.** This system helps you document that process, spot your patterns, and track the shift from who you are now to who you're becoming.

It works through three layers:

- **Daily brain dumps** — unfiltered voice or text, morning and evening, processed by AI into structured entries
- **Pattern recognition** — tracking the two forces inside you: your Builder (the part creating your new reality) and your Resistor (the part keeping you anchored to the old one)
- **Monthly reviews** — synthesizing a month of data into clear evidence of identity shift, synchronicities, and progress toward your vision

## What You Need

- **[Obsidian](https://obsidian.md)** (free) — where your files live. You'll browse entries, foundation docs, and monthly summaries here.
- **[Cowork](https://cowork.com)** — the AI layer that runs the system. Open this folder in Cowork to start.
- **~60 minutes** for first-time setup (4 steps, can be spread across sessions). ~15 min/day after that.

## How It Works (Cowork)

This system runs entirely through **Cowork** — no technical setup needed. Everything lives as markdown files in this folder.

### First Time Setup

Open this folder in Cowork and say: **"Help me set up my Quantum Reality Shift system."**

Claude walks you through 4 steps. Each step is a guided conversation — you talk, Claude creates the file.

| Step | What happens | Time | Creates |
|------|-------------|------|---------|
| 1. Your Story | You share your backstory — what brought you here, what you're moving away from | ~15 min | `My_Foundation/My_Journey_Context.md` |
| 2. Your Baseline | An honest snapshot of where you are right now across life domains | ~15 min | `My_Foundation/My_Baseline.md` |
| 3. Your Vision | A vivid description of your life at the end of your timeline | ~15 min | `My_Foundation/My_Vision.md` + month folders |
| 4. Customize Tracking | Configure specific patterns, relationships, or areas for special attention | ~10 min | `system/MY_CONTEXT.md` |

You can pause between steps and pick up later — just say **"continue setup"** and Claude will detect where you left off.

### Daily Use

**One chat per day.** Morning and evening happen in the same conversation.

**Morning** — List your tasks for the day in whatever way feels natural:

> "Morning inventory" or "Starting my day"

Claude classifies each task as Signal (moves transformation forward) or Noise (necessary maintenance), then checks whether the Builder or Resistor force is driving your priorities. You get a prioritized list and a force check. No file is created yet — this lives in the conversation.

**Evening** — Come back to the same chat and talk freely:

> "Brain dump" or "Ending my day"

Just talk. About everything. What happened, how you felt, what worked, what didn't. Claude combines your morning inventory and evening dump into a single structured entry file with themes, patterns, emotional tracking, plan-vs-reality comparison, and action items.

**Edge cases:**
- Evening-only is fine — if you skip the morning, Claude creates an entry from just the brain dump.
- Morning-only doesn't create a file — the inventory stays in the chat until you do an evening dump.

### Monthly Review

At the end of each month, say:

> "Generate my monthly summary"

Claude reads all your entries and produces a comprehensive review: momentum tracking, Builder vs Resistor analysis, reality selection evidence, identity shift markers, and progress toward your vision.

## The Framework

### Two Forces Inside You

You have two operating forces:

- **The Builder** — your forward-moving self. Creates, ships, takes risks, connects, grows. It builds the new reality.
- **The Resistor** — your self-protective self. Delays, overthinks, avoids exposure, keeps you comfortable. Not evil — protective. But left unobserved, it runs your life by default.

Both are you. The system doesn't fight the Resistor — it makes it visible so you can choose consciously.

### Two Types of Action

- **Signal** — Directly moves your transformation forward (revenue, growth, creation, deep relationship work, health breakthroughs)
- **Noise** — Necessary maintenance that doesn't move the needle (admin, organization, errands)

There's no such thing as a "Resistor task." What actually happens is the Resistor *force* makes you do Noise when you should be doing Signal — or disguises avoidance as Signal work. You spend the day "preparing" instead of doing. It feels productive. Nothing moved.

### The 3-Question Filter

For any task you're unsure about:

1. **"Does this directly create growth, income, or transformation?"** — Yes = Signal. No = Noise.
2. **"Am I doing this because it moves me forward — or because it feels safe?"** — Forward = Builder. Safe = Resistor.
3. **"If I'm honest, what am I avoiding right now?"** — The Resistor's best trick isn't stopping you. It's keeping you busy with the wrong thing so you never face the real one.

### Reality Selection

Your internal state (consciousness, identity, emotional regulation) correlates with external results. The system tracks this relationship over time, documenting synchronicities and showing you evidence of how your inner shifts create outer changes.

## Folder Structure

```
Quantum_Reality_Shift/
├── README.md                    ← You are here
│
├── My_Foundation/               ← Your personal foundation (generated during onboarding)
│   ├── My_Journey_Context.md
│   ├── My_Baseline.md
│   └── My_Vision.md
│
├── Entries/                     ← Your daily entries
│   └── Month_XX_[Name]/
│       └── Entry_YYYY-MM-DD.md
│
└── Monthly_Summaries/           ← Your monthly reviews
```

## Your Data

All your personal files (`My_Foundation/`, `Entries/`, `Monthly_Summaries/`) stay local and are gitignored — they never leave your machine.

During setup, Step 4 generates `system/MY_CONTEXT.md` — a ~500 word summary of your situation, goals, and tracking preferences. This is the only file Claude reads at the start of each daily session, so it doesn't need to re-read your entire foundation every time. Your full foundation files (`My_Journey_Context.md`, `My_Baseline.md`, `My_Vision.md`) are written once during onboarding and referenced through MY_CONTEXT.md going forward.

## Support This Project

Quantum Reality Shift is free and open source. If it helps you, consider supporting its development:

☕ [Buy Me a Coffee](https://buymeacoffee.com/moontown)

## Disclaimer

Quantum Reality Shift is a self-reflection tool, not a substitute for therapy or professional mental health treatment. See [DISCLAIMER.md](DISCLAIMER.md) for full details.
