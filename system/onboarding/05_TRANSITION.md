# Cycle Transition

**Goal:** Archive current cycle data, run modified onboarding for next cycle
**Prerequisites:** At least one month of entries must exist in `Entries/`
**Estimated time:** 20-30 minutes

---

## Instructions for Claude

**Important:** A cycle transition is a dedicated conversation — it is NOT a daily workflow chat. Do not combine with a morning inventory or brain dump. If the user tries to do both, complete the transition first, then tell them to start a fresh chat for their first daily entry in the new cycle.

### Pre-Check: Validate Readiness

Before starting, check `Entries/` for existing month folders and entry files.

- **No entries exist at all** → Tell the user: "You don't have any entries to archive yet. Transitions work best after at least a few weeks of journaling. Want to keep going with this cycle instead?" Do not proceed unless the user explicitly confirms.
- **Fewer than ~2 weeks of entries** → Warn: "You only have [X] entries so far. You can transition now, but there won't be much to synthesize for your journey context. Want to continue anyway?"
- **Entries exist** → Proceed normally.

### Phase 1: Assessment

Before starting, read `system/MY_CONTEXT.md` to understand current cycle state. If MY_CONTEXT.md doesn't have a `## Cycle Info` section (pre-v3.0 user), treat this as the first cycle.

Then assess what exists:
- List `Monthly_Summaries/` — how many summaries exist?
- List `Entries/` — how many month folders and entry files?
- If monthly summaries exist, read the last 2-3 for synthesis context
- **If no monthly summaries exist,** read a representative sample of entries directly (first entry, last entry, and 2-3 from the middle) to synthesize the cycle arc

Open with something like:
"Looks like you're ready for a new cycle. Before we start the next chapter, let me take stock of where this cycle brought you."

Present a brief synthesis of the cycle based on what you read (summaries if available, entries if not). Ask: "Does this capture the arc? Anything major I'm missing?"

### Phase 2: Archive (Automated)

Determine the cycle number. Check if any `Cycle_*` folders exist in the root:
- No cycle folders → this will be `Cycle_01`
- Existing cycle folders → increment (e.g., if `Cycle_01` exists, this is `Cycle_02`)

Determine the date range from the entries (earliest entry date → latest entry date). Format: `[MonthAbbr][Year]` (e.g., `Sep2025_Mar2026`).

Tell the user:

"I'm going to archive your current cycle into `Cycle_[XX]_[StartMonth][Year]_[EndMonth][Year]/`. This moves your entries, monthly summaries, and foundation docs into a dated folder so your history stays browsable while we start fresh. Ready?"

Wait for confirmation. Then:

1. Create `Cycle_[XX]_[StartMonth][Year]_[EndMonth][Year]/` folder
2. Create subfolders: `Entries/`, `Monthly_Summaries/`, `Foundation/`
3. Copy all files from `Entries/` into `Cycle_[XX]/Entries/` (preserving month folder structure)
4. Copy all files from `Monthly_Summaries/` into `Cycle_[XX]/Monthly_Summaries/`
5. Copy all files from `My_Foundation/` into `Cycle_[XX]/Foundation/`
6. Copy `system/MY_CONTEXT.md` into `Cycle_[XX]/Foundation/MY_CONTEXT.md` (preserves tracking config for historical reference)
7. Delete the original files from `Entries/`, `Monthly_Summaries/`, and `My_Foundation/`
8. Create fresh empty `Entries/`, `Monthly_Summaries/`, and `My_Foundation/` folders

Confirm to user: "Archive complete. Your [X] months of entries and [X] monthly summaries are preserved in `Cycle_[XX]_[dates]/`. Ready for the next chapter."

### Phase 3: Modified Onboarding

Now run a compressed version of the four onboarding steps. The key difference from first-time onboarding: you already have rich context from the previous cycle.

#### Step 1: Journey Context (Auto-Generated)

Read ALL monthly summaries from the archived cycle: `Cycle_[XX]_[dates]/Monthly_Summaries/`
If no monthly summaries exist in the archive, read all entries from `Cycle_[XX]_[dates]/Entries/` and synthesize directly.

Generate `My_Foundation/My_Journey_Context.md` using this structure:

```markdown
---
title: My Transformation Journey Context
date_created: [TODAY'S DATE]
tags:
  - journey
  - transformation
  - cycle-[XX]
---

# My Transformation Journey Context

## Previous Cycle Summary
[Synthesize the full arc of the previous cycle in 3-5 paragraphs. Include: what they started with, key breakthroughs, identity shifts demonstrated, resistor evolution, and where they ended up. Use evidence from monthly summaries.]

## Patterns Carried Forward
[Recurring patterns that persisted across the cycle — both productive and resistive. These are the user's operating patterns to track in the new cycle.]

## Key Relationships in This Journey
[People who matter, pulled from monthly summaries]

## Current Tools and Practices
[What's working — journaling approach, coping strategies, support systems, etc.]
```

Read this back to the user. Ask: "Does this capture your journey? Anything important to add or correct?"

#### Step 2: Baseline (Conversational — Fresh Assessment)

If the previous cycle's baseline exists at `Cycle_[XX]_[dates]/Foundation/My_Baseline.md`, read it for reference.

Open with: "Your last baseline was taken [X months ago]. A lot has changed. Let's take a fresh snapshot."

For each domain from the previous baseline:
- State their previous rating: "Last time you rated [Domain] at [X/10]. Where is it now?"
- Ask for brief explanation of what changed

Also ask:
- "Any new domains that matter now that didn't before?"
- "What's your most reliable form of self-sabotage NOW? Has the Resistor evolved?"
- "What are you avoiding right now?"

Generate `My_Foundation/My_Baseline.md` using the same format as `02_BASELINE.md` but including a "Previous → Current" comparison for each domain.

#### Step 3: Vision (Fully Fresh)

Open with: "New cycle, new vision. Same exercise as before — but from where you are now, not where you were."

Run the timeline selection and future-day exercise exactly as specified in `03_VISION.md`. This must be completely fresh — do not carry forward the old vision.

Generate `My_Foundation/My_Vision.md` and create monthly entry folders in `Entries/`.

**Folder naming rule:** Folders are numbered sequentially from `Month_01` based on the journey start date, labeled with the calendar month name. Example: if the cycle starts April 15 and runs 6 months, create `Month_01_April/`, `Month_02_May/`, `Month_03_June/`, `Month_04_July/`, `Month_05_August/`, `Month_06_September/`. If the start date is mid-month, the first and last folders may be partial months — that's fine.

#### Step 4: Customize (Quick Refresh)

Read the previous cycle's MY_CONTEXT.md from the archive: `Cycle_[XX]_[dates]/Foundation/MY_CONTEXT.md`. This was preserved during Phase 2. Use it to reference the user's previous Resistor/Builder patterns and special tracking configuration.

Open with: "Last step. Let's update how the system tracks your patterns. Your Resistor has probably evolved since last cycle."

Quick-fire through:
- "What does your Resistor do NOW? What are its current tactics?" (Reference previous tactics from archived MY_CONTEXT.md for comparison)
- "What does your Builder look like now?"
- "Is your special tracking area still the right focus, or has it shifted?" If the user wants to keep the same area, carry the trigger keywords and lens forward — don't make them re-specify everything. If they want to add a second tracking area, support up to two in MY_CONTEXT.md (use `## Special Tracking 1` and `## Special Tracking 2`).

Generate `system/MY_CONTEXT.md` using the same format as `04_CUSTOMIZE.md` output. Carry forward the `**Language:**` setting from the previous cycle's MY_CONTEXT.md (don't re-ask unless the user brings it up). Add:

```
## Cycle Info
**Current cycle:** [XX]
**Previous cycles:** [List with date ranges]
**Archive location:** Cycle_[XX]_[dates]/
```

### Phase 4: Confirmation

Tell the user:

"Your new cycle is set up. Here's what's ready:

**Archived:** [Previous cycle] — all entries and summaries preserved in `Cycle_[XX]_[dates]/`

**Fresh for this cycle:**
- Updated Journey Context (informed by [X] months of data)
- New Baseline (domain ratings refreshed)
- New Vision ([timeline])
- Updated MY_CONTEXT.md

**Your daily workflow is the same:** morning inventory + evening brain dump. Day 1 of Cycle [XX] starts now.

Want to do your first brain dump?"

---

## Constraints

- The transition should feel like graduation, not reset. Celebrate what was accomplished.
- Archive is automated but always confirmed by the user before proceeding ("Ready?" → wait for yes).
- Journey Context is auto-generated (efficiency) but confirmed by user (accuracy).
- Baseline must be conversational — self-assessment can't be automated.
- Vision must be completely fresh — don't carry forward old targets.
- Customize is a quick refresh, not a full redo.
- Total time: 20-30 minutes.
