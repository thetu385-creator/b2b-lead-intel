# B2B Lead Intelligence Analyst (Generic Edition / b2b-lead-intel)

A reusable **sales-intelligence skill** for **Chinese manufacturers / brands going global (B2B)**. It turns one raw lead — a website, a company name, public materials, or an inquiry BOQ — into a **decision-ready report** that actually guides selling: risk screening (spot shells / fake trading sites) + decision-chain mapping (reach the right person) + a 5-dimension 100-point priority score + a 7-day first-touch action list.

> This is an **industry-agnostic framework**. All industry-, brand-, and client-specific private data has been stripped out. Before use, fill in the **"Product Library"** and **"Certification Supplement"** for your own industry.

## What it does

- **8-stage workflow**: global search & risk screening → client-type classification → business baseline profiling → decision-chain / KP mapping → product-line fit → market-access certification → 5-dimension 100-point scoring → 7-day action list.
- **⚡ Client Snapshot card**: one table at the very top of the report — grasp the essentials in 10 seconds (company history / core products / main business / key channels / service regions / client tier + a one-line verdict).
- **5-dimension 100-point scoring**: Purchasing Power & Potential (25) / Market & Product Fit (25) / Company Credibility & Risk (20) / Partnership Depth & Intent (20) / Execution & Fulfillment (10), with a detailed score sheet and A/B/C/D grades.
- **Decision-chain mapping**: break "a company" into "a group of people" (decision-maker / influencer / gatekeeper / user), give a contact sequence by channel type, and flag "missing KP" risks.

## Who it's for

- Teams doing overseas B2B sales who need background checks and development strategies on foreign buyers / distributors / engineering purchasers.
- Any Chinese supplier, regardless of industry (machinery, electronics, building materials, consumer goods, food-contact, medical, etc.) — just swap in your product library and certifications.

## Install (WorkBuddy)

Place the entire `b2b-lead-intel/` folder into WorkBuddy's skills directory:

- Windows: `%USERPROFILE%\.workbuddy\skills\b2b-lead-intel\`
- macOS / Linux: `~/.workbuddy/skills/b2b-lead-intel\`

After restarting or refreshing WorkBuddy, trigger it by saying "analyze [client website URL / company name + country]", "client background check", etc.

> You can also `git clone` this repo directly into the path above.

## Required setup before first use

The `references/` folder ships as **fill-in templates** with no embedded industry data:

1. **`references/product_competitors.md`** — fill in your **[product library / technical specs / competitor map]**. Stage 5 (product-line fit) depends on it.
2. **`references/cert_matrix.md`** — fill the **[mandatory / high-attention certifications]** for your industry in the "Industry-specific certification zone" (building materials, electronics, food-contact, etc. each have their own). Stage 6 (market-access gate) depends on it.

Until these two are filled, Stage 5/6 judgments will be empty — by design, so no industry data is leaked or fabricated.

## Directory structure

```
b2b-lead-intel/
├── SKILL.md                      # Main skill file (8-stage workflow + snapshot + 5-dim scoring + output templates)
├── references/
│   ├── product_competitors.md    # Product library / specs / competitor map (template, fill in)
│   ├── cert_matrix.md            # Country market-access cert matrix + industry supplement (template, fill in)
│   ├── action_playbook.md        # Typed confirmation question bank & 7-day talk-track hooks
│   └── decision_chain.md         # KP role definitions / typed chain models / search patterns / risk warnings
├── README.md                     # Chinese README
├── README_EN.md                  # English README
└── LICENSE
```

## How to trigger

- Just say: analyze [client website URL / company name + country], client background check, lead development strategy, map the decision chain / KP, competitor analysis.
- The skill auto-searches the web + reasons, then outputs a structured report with a snapshot card.

## License

MIT — free to use, modify, and redistribute. Just keep the attribution.

---

*Generated with WorkBuddy. The structure and methodology are reusable across industries; specific product and certification data must be supplied by the user.*
