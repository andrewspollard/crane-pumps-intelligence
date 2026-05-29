# Crane Pumps & Systems - Account Intelligence Platform

> Living operational intelligence for account management, expansion, and retention.

## Architecture

```
┌─────────────────────────────────────────────────────────┐
│                   PRESENTATION LAYER                      │
│   docs/index.html - Interactive intelligence surface      │
│   Sections render conditionally based on data density     │
└─────────────────────────┬───────────────────────────────┘
                          │
┌─────────────────────────┴───────────────────────────────┐
│                   SYNTHESIS ENGINE                        │
│   Draws from all modules, ranks actions, detects         │
│   signals, generates prescriptive recommendations        │
└─────────────────────────┬───────────────────────────────┘
                          │
┌─────────────┬───────────┼───────────┬───────────────────┐
│  MODULE 1   │  MODULE 2 │  MODULE 3 │  MODULE 4         │
│  CRM/SFDC   │  Chorus   │  ZoomInfo │  Email/Calendar   │
│  ✅ LIVE    │  ✅ LIVE  │  ✅ LIVE  │  ✅ LIVE          │
│             │           │           │                   │
│  MODULE 5   │  MODULE 6 │  MODULE 7 │  MODULE 8         │
│  Usage/     │  Support  │  Roadmap/ │  Market/          │
│  Adoption   │  Tickets  │  Product  │  News             │
│  ⏳ PENDING │  ⏳ PENDING│  ⏳ PENDING│  ⏳ PENDING       │
└─────────────┴───────────┴───────────┴───────────────────┘
```

## Directory Structure

```
├── README.md
├── docs/
│   └── index.html              # Interactive intelligence dashboard
├── data/
│   ├── account.json            # Core account profile
│   ├── contacts.json           # Stakeholder map
│   ├── opportunities.json      # Pipeline and closed business
│   ├── interactions.json       # Meeting/call timeline
│   └── schemas/
│       ├── module-schema.json  # Standard module interface
│       ├── usage-module.json   # Placeholder: adoption telemetry
│       ├── support-module.json # Placeholder: ticket history
│       ├── roadmap-module.json # Placeholder: product roadmap
│       └── market-module.json  # Placeholder: market intelligence
├── meeting-notes/              # Structured post-call recaps
├── artifacts/                  # One-pagers, proposals, QBR decks
└── .github/
    └── CODEOWNERS
```

## Usage

This repo is maintained by Amazon Quick. To refresh:
- **Refresh Crane Pumps** - Full data pull from all live modules + synthesis
- **Update Crane Pumps with today's call** - Append meeting notes + update signals
- **Prep me for Crane Pumps** - Generate pre-call brief from latest state

## Module Status

| Module | Source | Status | Last Refreshed |
|--------|--------|--------|----------------|
| CRM/SFDC | Salesforce API | ✅ Live | 2026-05-29 |
| Call Intelligence | Chorus MCP | ✅ Live | 2026-05-29 |
| Company Intel | ZoomInfo (via SFDC) | ✅ Live | 2026-05-29 |
| Email/Calendar | Outlook | ✅ Live | 2026-05-29 |
| Usage/Adoption | TBD | ⏳ Awaiting | - |
| Support Tickets | TBD | ⏳ Awaiting | - |
| Product Roadmap | TBD | ⏳ Awaiting | - |
| Market Intelligence | TBD | ⏳ Awaiting | - |

## Synthesis: Current Signals

### Expansion Signals
- Interest in Candidate Experience Portal (new product area)
- Workflow opportunity in active pipeline ($18.5K, close 6/30/2026)
- Onboarding new users (Chelsea, Olivia) = org expanding usage footprint

### Risk Signals
- 37 days since last customer interaction (gap widening)
- Candidate import bug unresolved (creates daily friction)
- Hannah McKee struggling with search (unfavorable LinkedIn Recruiter comparison)
- No executive sponsor interaction logged

### Recommended Actions (Priority Order)
1. Reach out to Katy - Re-establish cadence, progress Workflow opp
2. Resolve candidate import bug - Follow up with tech on ticket status
3. Schedule Hannah enablement - Dedicated session on early-career search
4. Training for Chelsea and Olivia - Katy requested 5/23, needs scheduling
5. Candidate Experience Portal demo - Promised in March, not delivered