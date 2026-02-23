# Contributing to Quantum Reality Shift

Thanks for your interest in contributing! QRS is open source under CC BY 4.0.

## How to Contribute

### Report Issues
- Use GitHub Issues for bugs, suggestions, or questions
- Include which file(s) are affected and what you expected vs what happened

### Suggest Improvements
- Open an issue first to discuss before submitting changes
- Describe the problem you're solving and your proposed approach

### Submit Changes
1. Fork the repository
2. Create a branch for your change
3. Make your edits
4. Submit a pull request with a clear description

## Project Structure
```
Quantum_Reality_Shift/
├── CLAUDE.md                    ← Main instructions (auto-loaded by Cowork)
├── README.md                    ← Public-facing overview
├── LICENSE.md                   ← CC BY 4.0
├── DISCLAIMER.md                ← Liability and scope
├── CONTRIBUTING.md              ← You are here
├── FUNDING.yml                  ← Donation links
│
├── system/                      ← Claude's reference files
│   ├── onboarding/              ← Setup steps (read once)
│   │   ├── 01_STORY.md
│   │   ├── 02_BASELINE.md
│   │   ├── 03_VISION.md
│   │   └── 04_CUSTOMIZE.md
│   └── templates/
│       └── Monthly_Summary_Template.md
│
├── My_Foundation/               ← Generated during onboarding (gitignored)
├── Entries/                     ← Daily entries (gitignored)
└── Monthly_Summaries/           ← Monthly reviews (gitignored)
```

## Key Files

- **CLAUDE.md** — Contains all prompts, templates, and workflow logic. This is the brain of the system. Changes here affect every user's daily experience.
- **system/onboarding/** — The four-step setup flow. Each file is self-contained with instructions for Claude.
- **system/templates/Monthly_Summary_Template.md** — Structure for monthly reviews.
- **system/MY_CONTEXT.md** — Generated per-user (gitignored). ~500 words, read every session.

## Guidelines

- Keep CLAUDE.md under reasonable token limits — it's loaded every session
- Preserve the Builder/Resistor + Signal/Noise framework language
- Test onboarding changes end-to-end
- Don't commit personal data (My_Foundation/, Entries/, etc.)

## Questions?
Open an issue or reach out to Adrian Muntean.
