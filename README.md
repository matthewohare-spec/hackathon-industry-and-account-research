# Industry & Account Research Workflow
**Vic.ai Hackathon Project — Built by Matt O'Hare**

https://www.loom.com/share/7661d715210a4da0a8ff5f5f824bfefc

---

## The Problem

AEs and SDRs aren't experts across every industry — but they need to sound like they are. Building credibility with a CFO at a 3PL company requires very different knowledge than selling to a Controller at a construction firm. That research is time-consuming, scattered across multiple sites, and has to be manually translated into something a rep can actually use on a call or in an email.

On average, reps can spend **1–3 hours per week** gathering this context. New hires spend even more time trying to ramp on industries they've never sold into.

---

## The Solution

The **Industry & Account Research Workflow** is a Cowork-native AI agent that generates fresh, web-researched sales intelligence for any company or industry — in under 2 minutes.

Reps simply open Cowork and type a request. The agent searches the web for live data, compiles it into a polished Word document tailored for sales use, and automatically posts a summary to the team's `#territory-research` Slack channel.

### Four Output Types

| Prompt | What You Get |
|--------|-------------|
| `account brief: [company]` | Deep-dive on a specific account — financials, key decision makers, AP complexity, ERP stack, strategic signals, talking points, objection handling |
| `one pager: [company]` | Executive-ready business case — key stats, industry pressures, company-specific pain, Vic.ai value prop, and why now |
| `outreach: [company or industry]` | Tailored cold emails and LinkedIn messages for 4 personas: CFO, Controller, AP Director, and VP Finance — with company-specific hooks |
| `industry overview: [industry]` | Sector primer with AP complexity breakdown, industry-specific finance terms, tech landscape, discovery questions, and Vic.ai positioning |
| `run all 4 for [company]` | All four outputs in a single run |

---

## How It Works

1. **Rep opens Cowork** and types a request (e.g. `one pager: Metronet`)
2. **Agent runs live web research** — 5–8 targeted searches per output using company websites, press releases, LinkedIn, trade publications, and analyst reports
3. **Polished Word doc is generated** and saved to the team's Workflow folder — formatted with Vic.ai branding, real executive names, specific talking points, and researched content (no filler)
4. **Slack notification fires automatically** to `#territory-research` with key highlights and the filename

---

## Impact

- **Saves 1–3 hours per week** for active AEs depending on call volume
- **Accelerates new rep onboarding** — reps can quickly build industry fluency across any sector without manual research
- **Increases call quality** — reps walk in with specific company context, real executive names, and tailored messaging instead of generic pitches
- **Supports full cycle** — useful before first outreach, before discovery calls, before demos, and for mid-cycle re-engagement

---

## Demo Instructions

1. Log into [Cowork](https://claude.ai/claude-code) on desktop
2. Open the **AI Research Agent/Workflow** project
3. Type any of the following prompts in chat:

```
account brief: [company name]
one pager: [company name]
outreach: [company name or industry]
industry overview: [industry name]
run all 4 for [company name]
```

**Example prompts to try:**
- `one pager: Metronet`
- `account brief: AIT Worldwide Logistics`
- `industry overview: construction`
- `outreach: third party logistics`
- `run all 4 for Ferguson Enterprises`

Results are delivered as a formatted Word document in the Workflow folder and summarized in `#territory-research` on Slack.

---

## Repo Structure

```
sales-research/
├── SKILL.md                     # Agent instructions and workflow steps
└── references/
    ├── output-formats.md        # Word doc formatting specs for each output type
    └── research-queries.md      # Web search query templates by output type
```

---

## Sample Outputs

- **Metronet Executive One-Pager** — Fiber ISP with T-Mobile/KKR acquisition, 7 acquisitions in 7 years, CFO promoted from Controller
- **Graybar Account Brief** — $12.9B electrical distributor, SAP S/4HANA migration, Conexiom gap, 6+ acquisitions
- **AIT Worldwide Logistics Account Brief** — 3PL, $2.6B revenue, new PE owner Greenbriar, 11 acquisitions, no AP automation found
- **Construction Industry Overview** — Subcontractor AP complexity, lien waivers, job costing, retainage

---

*Built with Anthropic's Cowork and Claude Agent SDK. Powered by live web research and the `docx` npm package for document generation.*
