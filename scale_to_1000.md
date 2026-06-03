# Scaling to 1,000 Companies
## Operational Plan for Industrial-Scale Federer Company Identification

---

## Objective

This document outlines how the research process demonstrated on 25 Gujarat specialty chemical companies can be scaled to identify 1,000 qualified Federer Company candidates across India's specialty chemicals, custom synthesis, pharmaceutical intermediates, and adjacent sectors.

The plan is operationally realistic, not aspirational. It accounts for drop-off rates at each filter stage, evidence quality variation across listed vs. unlisted companies, and the time cost of manual verification.

---

## Core Assumptions

| Parameter | Value |
|---|---|
| Target output | 1,000 qualified PASS candidates |
| Expected PASS rate after full filtering | ~15–20% of screened universe |
| Required input universe | ~5,000–6,500 companies |
| Sectors covered | Specialty chemicals, custom synthesis, pharma intermediates, agrochemical intermediates, performance chemicals, fluorochemicals |
| Geographies | All major Indian chemical manufacturing states |
| Revenue ceiling | Rs. 500 Cr (adjustable per client definition) |
| Team structure | 1 research lead + 2–3 analysts + QA reviewer |

---

## Conversion Funnel

```
Raw Universe (5,000–6,500 companies)
           ↓  Remove obvious mismatches (sector, size, geography)
Pre-Screened Universe (~3,000 companies)
           ↓  E1 Producer Test
           ↓  E2 Geography Test
E1/E2 Eligible (~1,500–1,800 companies)
           ↓  Revenue ceiling verification
Revenue-Qualified (~900–1,100 companies)
           ↓  C3–C8 Federer Scoring
           ↓  Minimum score threshold
Qualified Federer Candidates (~1,000 companies)
           ↓  QA verification
           ↓  DM identification
Final Outreach-Ready List (~850–950 companies after QA attrition)
```

**Expected conversion rates at each stage:**
- Pre-screen drop-off: ~50% (sector mismatches, traders, obvious disqualifiers)
- E1/E2 drop-off: ~40% (traders, non-target-state, subsidiaries)
- Revenue filter drop-off: ~30% (above ceiling or below minimum)
- Federer scoring drop-off: ~35% (commodity businesses, low scores)
- QA attrition: ~10% (unresolvable uncertainty, DM not identifiable)

---

## 4-Week Execution Plan

### Week 1 — Universe Construction

**Goal:** Build a raw universe of 5,000–6,500 companies.

**Day 1–2: Geography and Sector Mapping**
- Define target states: Gujarat, Maharashtra, Telangana, Rajasthan, Tamil Nadu (primary chemical manufacturing clusters)
- Define NIC codes for target sectors: 201 (basic chemicals), 202 (pesticides), 203 (paints/coatings), 204 (soap/surfactants), 205 (other chemicals), 210 (pharma), 2011 (industrial gases)
- Map GIDC, MIDC, TSIIC, RIICO cluster directories to sector codes

**Day 3–5: Source Harvesting**
- Pull BSE and NSE listed chemical companies by sector code → ~800–1,000 listed companies
- Pull BSE SME chemical companies → ~300–500 additional
- Extract DSIR-recognised R&D companies (chemicals + pharma) → ~400–600
- Download CHEMEXCIL and Pharmexcil member directories → ~1,500–2,000
- Pull MCA NIC code searches for Gujarat, Maharashtra, Telangana → ~2,000–3,000 private companies
- Cross-deduplicate across sources

**Day 6–7: Triage and Pre-Screening**
- Remove companies below Rs. 10 Cr revenue (too small)
- Remove companies above Rs. 1,000 Cr revenue (too large — flag separately)
- Remove obvious traders (no manufacturing facility evidence)
- Remove known non-ICP sectors (bulk commodity, fertilizers, plastics)

**Deliverable:** Pre-screened universe of ~3,000 companies with name, website, state, sector, and revenue estimate.

---

### Week 2 — E1/E2 Filtering and Revenue Verification

**Goal:** Apply eligibility filters to the pre-screened universe.

**E1 Filter (Producer Test) — Batch Processing**
- For listed companies: extract manufacturing facility disclosures from latest annual report
- For unlisted companies: check company website for plant/facility pages; fall back to IndiaMART profile claims; fall back to MCA registration address
- Tag each company: CONFIRMED MANUFACTURER / LIKELY MANUFACTURER / TRADER / UNCLEAR
- Remove TRADER; send UNCLEAR to manual review queue

**E2 Filter (Geography Test) — Batch Processing**
- Confirm registered address or operational address in target state
- For listed companies: verify plant location from BSE filings
- Tag: CONFIRMED IN-STATE / POSSIBLE IN-STATE / OUT-OF-STATE
- Remove OUT-OF-STATE; send POSSIBLE to manual review queue

**Revenue Verification**
- Listed companies: pull FY25 revenue from screener.in or BSE annual report
- Unlisted companies: pull from MCA via Tofler (accept 1–2 year lag; flag as estimated)
- Apply Rs. 500 Cr ceiling; flag Rs. 400–500 Cr companies for QA (ceiling proximity risk)
- Flag companies with rapidly growing revenue for ceiling monitoring

**Deliverable:** Revenue-qualified, E1/E2-eligible list of ~900–1,100 companies with evidence tags.

---

### Week 3 — Federer Scoring

**Goal:** Score all revenue-qualified companies across C3–C8 dimensions.

**Scoring Approach by Company Type**

| Company Type | C3–C8 Approach | Approximate Time per Company |
|---|---|---|
| Listed (BSE/NSE/BSE SME) | Annual report + concall + screener.in | 25–35 minutes |
| Unlisted, DSIR-recognised | DSIR listing + website + MCA + export data | 35–50 minutes |
| Unlisted, no DSIR | Website + IndiaMART + MCA + LinkedIn DM | 45–60 minutes |

**AI-Assisted Scoring (Accelerated)**

AI tools can accelerate the process with the following workflow:

1. Feed the company's annual report or website content to AI
2. Request: "Identify evidence for each of these criteria: [C3 checklist / C4 checklist / etc.]"
3. AI produces a first-pass evidence summary
4. Analyst reviews and disputes or confirms each claim
5. Final score is set by the analyst, not the AI

This hybrid approach reduces per-company research time by approximately 40% while maintaining human accountability for all final scores.

**Scoring Rules**
- Score conservatively when evidence is ambiguous
- Do not assign maximum scores without strong, specific evidence
- Flag all company-specific uncertainties in the QA column at point of scoring

**Deliverable:** Fully scored database with C3–C8 scores, Federer Total, Score Band, Verdict, and QA flags.

---

### Week 4 — Manual QA and Outreach List Preparation

**Goal:** Validate flagged uncertainties, identify decision-makers, and produce outreach-ready records.

**QA Resolution**
- Assign each QA-flagged company to an analyst
- Resolve flags in priority order: Revenue Ceiling → DM Identity → ERP/Systems → Location
- Apply one of three outcomes: CONFIRMED (QA resolved, PASS stands), DOWNGRADED (evidence insufficient, move to BORDERLINE), REJECTED (disqualifying information found)

**Decision-Maker Identification**
- For all PASS companies: identify the primary decision-maker via LinkedIn, annual report, or company website
- Record: Full name, title, email format (if inferable), LinkedIn URL
- Score C4 post-DM identification if initial scoring used placeholder

**Personalisation Hook Generation**
- For top-tier PASS companies (Federer score ≥ 75): write a 1–2 sentence outreach hook using the most distinctive, verifiable fact about the company
- Good hooks reference: world/India rankings, specific technology advantages, recent growth milestones, regulatory achievements

**Final List Grading**
- Tier 1 (Score ≥ 80, no open QA): Priority outreach
- Tier 2 (Score 65–79, QA resolved): Standard outreach
- Tier 3 (Score 50–64, QA resolved): Second-wave outreach
- BORDERLINE (QA unresolved): Monitor and re-evaluate next cycle

**Deliverable:** Outreach-ready list of ~850–950 qualified Federer Company candidates with DM names, personalisation hooks, and QA status.

---

## Quality Controls at Scale

**Calibration companies:** Include 5–10 companies with known profiles (e.g., Aarti Industries — auto-disqualify on revenue; Tatva Chintan — PASS) as calibration anchors to test whether the scoring model is being applied consistently across analysts.

**Inter-analyst scoring checks:** For a random 10% sample, have a second analyst score the same company independently. Flag discrepancies above 10 points for review. Resolve by discussing the specific evidence, not averaging the scores.

**QA column as a forcing function:** Any company where the scorer has uncertainty must use the QA column. An empty QA column on an unlisted company with estimated revenue is a red flag, not a sign of confidence.

**Rejection documentation:** Every FAIL verdict must have a stated reason. A batch of companies with "Insufficient Evidence" as the only rejection reason signals the researcher is not digging deeply enough.

---

## Expected Outputs by Sector

Based on the Gujarat pilot (25 companies, ~9 PASS outcomes from the eligible pool):

| Sector | Expected Candidates in Rs. 50–500 Cr Band | Expected PASS Rate | Expected Qualified Companies |
|---|---|---|---|
| Specialty Chemicals — Gujarat | ~300–400 | 20–25% | 60–100 |
| Pharma Intermediates — Gujarat + Maharashtra | ~400–600 | 15–20% | 60–120 |
| Agrochemical Intermediates — All India | ~300–400 | 15–20% | 45–80 |
| Fluorochemicals | ~80–120 | 25–30% | 20–35 |
| Custom Synthesis (CRAM/CRO/CDMO) | ~150–200 | 25–30% | 35–60 |
| Performance Chemicals | ~200–300 | 15–20% | 30–60 |
| **Total** | **~1,430–2,020** | **~18–22%** | **~250–455** |

To reach 1,000 qualified companies, the geography must expand beyond Gujarat and Maharashtra to include Telangana, Rajasthan (RIICO clusters), Tamil Nadu (SIPCOT clusters), and Himachal Pradesh (pharma intermediates).

---

## Tools and Infrastructure Required

| Function | Tool | Notes |
|---|---|---|
| Company database | Screener.in + MCA/Tofler | Primary financial data |
| Export intelligence | Zauba.com or Volza | Shipment-level export data |
| Document analysis | AI (Claude) + human review | Annual report summarisation |
| DM identification | LinkedIn Sales Navigator | Essential for outreach preparation |
| Data storage | Google Sheets or Airtable | CRM-ready format |
| QA tracking | Dedicated QA column + review workflow | Mandatory |

---

## Timeline Summary

| Week | Activity | Output |
|---|---|---|
| Week 1 | Universe construction + pre-screening | ~3,000 pre-screened companies |
| Week 2 | E1/E2 filtering + revenue verification | ~900–1,100 eligible companies |
| Week 3 | C3–C8 Federer scoring | ~900–1,100 scored records |
| Week 4 | QA resolution + DM identification + grading | ~850–950 outreach-ready records |

**Total calendar time:** 4 weeks (team of 3–4 researchers)
**Estimated output:** 850–950 Tier 1–3 qualified Federer Company candidates
**Ongoing maintenance:** Quarterly re-evaluation of BORDERLINE companies; annual re-scoring of PASS companies to track revenue ceiling proximity

---

## What This Plan Does Not Promise

Reaching exactly 1,000 outreach-ready records in four weeks is achievable only if the sector table above holds — which requires expanding beyond Gujarat into Maharashtra, Telangana, and Tamil Nadu clusters. A Gujarat-only run, even well-executed, would yield approximately 250–350 qualified candidates. The 1,000-company target is a national exercise, not a single-state one.

The plan also does not promise zero false positives. It promises a documented, auditable process where every PASS can be traced back to specific evidence, and every FAIL has a stated reason. That discipline — not volume — is what makes the output usable for outreach.
