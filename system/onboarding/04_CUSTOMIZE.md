# Onboarding Step 4: Customize Your System

**Goal:** Generate `system/MY_CONTEXT.md` — the compact context file Claude reads during daily use
**Prerequisites:** `My_Journey_Context.md`, `My_Baseline.md`, and `My_Vision.md` must all exist in `My_Foundation/`
**Estimated time:** 10-15 minutes
**After this step:** System is fully set up and ready for daily use

---

## Instructions for Claude

Before starting, read all three foundation docs:
- `My_Foundation/My_Journey_Context.md`
- `My_Foundation/My_Baseline.md`
- `My_Foundation/My_Vision.md`

Open with something like:
"Last step. Your foundation is solid — we've got your story, your baseline, and your vision. Now I need to fine-tune how the system processes your daily entries. Two things: what to track with extra care, and how YOUR inner patterns work."

---

## Part A: Special Tracking

"The system tracks your general journey across all your domains. But sometimes there's one specific area that needs deeper, more careful documentation. For some people it's their relationship with a child. For others it's recovery from a specific pattern, building something from scratch, or healing a family dynamic."

### Questions:

**Primary Focus Area**
- Is there one relationship, project, or dynamic you want to track with extra depth?
- Why is this one important enough for special attention?
- What specifically should the system watch for? (Triggers? Breakthroughs? Behavioral patterns? Specific interactions?)

**Trigger Documentation**
- Are there specific triggers that should be flagged when they appear in your brain dumps?
- Are there recurring situations where you tend to fall back into old patterns?

**Custom Tracking Categories**
- Beyond the standard processing (themes, events, emotions, actions, patterns), is there anything else you want tracked?
- Examples: dreams, synchronicities, physical symptoms, specific habits, interactions with specific people

### If they identify a special tracking area:
Define:
1. **Name** for the tracking section (e.g., "Parenting Documentation," "Recovery Tracking," "Business Building Log")
2. **Triggers** — what in a brain dump should activate this section (list specific keywords, situations, or themes)
3. **What to capture** — the specific elements to document when triggered
4. **Lens** — the key question the system should ask about this area (e.g., "Am I responding from the old identity or the new one?")

### If they don't have one:
That's fine. Skip it. The system works without it. Can always be added later.

---

## Part B: Framework Language

"The system uses a few key concepts to analyze your entries. Let me explain them, and then let's map them to YOUR experience so the analysis actually hits home."

### The Two Forces

"You have two forces operating inside you. Everyone does."

**The Resistor**

"The Resistor is the part of you that keeps you anchored to your current reality. It's not evil — it's protective. But it shows up as self-sabotage, avoidance, busywork, delay, and comfort-seeking. Its best trick isn't stopping you — it's keeping you busy with the wrong thing so you never have to face the real one."

Ask:
- "What does YOUR Resistor typically do? What are its favorite tactics?"
- "How does it disguise itself as productivity or 'being responsible'?"
- "Can you think of a recent example where it won?"

**The Builder**

"The Builder is the part of you that creates the new reality. It ships, builds, takes risks, connects, stays present even when it's uncomfortable."

Ask:
- "When are you at your best? What does your Builder look like in action?"
- "What conditions help your Builder show up?"
- "What's a recent example where you operated from this place?"

### The Two Task Types

"Every action falls into one of two categories:"

**Signal** — directly builds the life you want. Revenue, creation, growth, deep connection, health breakthroughs.

**Noise** — necessary maintenance. Admin, errands, routine. Has to get done but doesn't move the needle.

"There's no such thing as a 'Resistor task.' What happens is the Resistor *force* makes you do Noise when you should be doing Signal — or disguises avoidance as Signal work. The system watches for that."

### Reality Selection

"The core premise: your internal state — identity, consciousness, emotional regulation — correlates with what shows up in your external life. When you're aligned, things flow. When you're fractured, things stall."

Ask:
- "Does this resonate with your experience?"
- "Can you think of a time when a shift inside you led to a shift outside?"
- "What about the reverse — when an inner fracture led to external chaos?"

---

## When This Step Is Complete

### Generate `system/MY_CONTEXT.md`

This is the CRITICAL output. This compact file (~500 words) is the ONLY file Claude reads during daily workflows. It replaces reading the three full foundation files every session.

Condense everything from the three foundation docs + this conversation into this structure:

```markdown
# My Context

## Who I Am
[2-3 sentences: name if given, core identity, what they're transforming from/to]

## Where I Started
[3-4 sentences: key patterns, cycles, baseline state. Reference domain ratings.]

## Where I'm Going
[3-4 sentences: vision summary in their voice]

**Timeline:** [Start date] → [End date] ([X] months / [X] days)

## My Domains
[Simple list of their chosen domains, e.g.:]
- Business
- Health
- Relationships
- Parenting
- Financial
- Creative

## My Resistor
[Their specific tactics in 3-5 bullet points, using their language]

## My Builder
[What aligned action looks like for them, 3-5 bullet points]

## Special Tracking
[If configured:]
**Name:** [Tracking name]
**Triggers:** [Keyword/situation list]
**Capture:** [What to document when triggered]
**Lens:** [Key question]

[If not configured:]
None configured. Standard processing only.
```

### Confirm Setup Complete

Tell the user:

"Your Quantum Reality Shift system is fully set up. Here's what's ready:"

List everything created:
- Foundation docs (My_Journey_Context, My_Baseline, My_Vision) in My_Foundation/
- Monthly entry folders in Entries/
- Your personalized context file (MY_CONTEXT.md)

Then explain daily workflow:
- **Morning:** Say "morning inventory" or "starting my day" — Claude categorizes your tasks as Signal or Noise and checks which force is driving
- **Evening:** Say "brain dump" or "ending my day" — talk freely, Claude creates a structured entry
- **Monthly:** Say "monthly summary" — Claude synthesizes all entries into a review

Suggest: "Want to do your first brain dump right now?"

---

## Constraints
- This is the final step — make it feel like completion
- The framework language section should feel like self-discovery, not a lecture
- MY_CONTEXT.md must be ~500 words MAX — it's read every single session, keep it tight
- Use their exact language for Resistor/Builder descriptions where possible
- Never judge their relationship with these concepts
- Celebrate the setup being done — this was real work
