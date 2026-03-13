# Arabella Advisors / New Venture Fund / Headwaters OSINT Findings
## Date: 2026-03-11
## Status: Active Investigation

---

## 1. THE EICHBERG CONNECTION (CONFIRMED)

**Adam Eichberg** simultaneously holds:
- **Board Chair, New Venture Fund** (Arabella Advisors' primary 501(c)(3) fiscal sponsor)
  - Source: https://newventurefund.org/who-we-are/board-of-directors/adam-eichberg-chair-of-the-board/
- **Co-founder, Headwaters Strategies** (Denver lobbying firm, founded 2009)
  - Source: Colorado SOS lobbying records, headwatersstrategies.com
- Former Deputy Legislative Director for Colorado Governor Bill Ritter
- Former Director of Policy, CO Dept of Public Health and Environment

## 2. META → HEADWATERS LOBBYING (CONFIRMED)

**Meta Platforms, Inc. is a registered lobbying client of Headwaters Strategies** in Colorado.

From Colorado Secretary of State Client Lobbyist Directory (Feb 2026):
```
META PLATFORMS, INC
1660 Lincoln Street, Suite 2910
Denver CO 80264
650-561-2558
Lobbyists:
  BURKHART, AMBER JANELLE (HEADWATERS STRATEGIES) - 503-333-7973
  COYNE, WILLIAM C (HEADWATERS STRATEGIES) - 303-834-7799
  HEADWATERS STRATEGIES - 303-834-7799
  SCHMIDT, ALYSON (HEADWATERS STRATEGIES) - 970-214-4231
```

Meta's registered Colorado address IS the Headwaters Strategies office: 1660 Lincoln St, Suite 2910, Denver CO 80264

Source: https://www.coloradosos.gov/pubs/lobby/downloadFiles/emplobrpt.pdf

**Also notable:** Apple Inc. is also a Headwaters Strategies client (same firm, both sides of ASAA debate)

## 3. ARABELLA NETWORK — SHARED ADDRESS (CONFIRMED)

All four Arabella-managed funds share 1828 L Street NW Suite 300, Washington DC:

| Entity | EIN | Suite | Revenue (2023) | Subsection |
|--------|-----|-------|-----------------|------------|
| New Venture Fund | 20-5806345 | 300-A | $669,088,461 | 501(c)(3) |
| Sixteen Thirty Fund | 26-4486735 | 300-B | $181,353,252 | 501(c)(4) |
| Windward Fund | 47-3522162 | 300-C | $212,371,954 | 501(c)(3) |
| Hopewell Fund | 47-3681860 | 300-D | $157,709,416 | 501(c)(3) |

Combined 2023 revenue: ~$1.22 BILLION

Other Arabella funds (from web research): North Fund, Telescope Fund, Impetus Fund
Former name: Arabella Legacy Fund (2006-2009) → renamed New Venture Fund

Source: ProPublica Nonprofit Explorer API

### NVF Financial History (2011-2023):
| Year | Revenue | Expenses | Assets |
|------|---------|----------|--------|
| 2023 | $669M | $895M | $768M |
| 2022 | $756M | $825M | $1.04B |
| 2021 | $964M | $553M | $1.24B |
| 2020 | $975M | $659M | $823M |
| 2019 | $461M | $421M | $491M |
| 2018 | $405M | $373M | $423M |
| 2017 | $359M | $330M | $383M |

NVF gave $592,958,696 in grants in 2023 (1,020 awards)
NVF gave 1,187 awards in 2022

## 4. DIGITAL CHILDHOOD ALLIANCE (DCA) FINDINGS

### Entity Status:
- **501(c)(4)** social welfare org — donor disclosure NOT required
- Registered as "Digital Childhood Alliance, Inc."
- Based in Washington, DC
- NOT found on ProPublica Nonprofit Explorer (no 990 on file yet — likely too new)
- NOT found on InfluenceWatch, OpenSecrets, or Ballotpedia

### Domain:
- **digitalchildhoodalliance.org**
- Registrar: GoDaddy.com, LLC
- **Created: 2024-12-18** (barely 3 months before testifying at state legislatures)
- Expires: 2028-12-18
- DNS: Cloudflare (leia.ns.cloudflare.com, mitch.ns.cloudflare.com)
- Privacy protection enabled — registrant info redacted
- Wayback Machine first snapshot: 2024-12-19 (one day after registration)

### Funding:
- Meta is "helping to fund" DCA — confirmed by Insurance Journal (3 anonymous sources)
- Casey Stefanski refused to name funders under oath at LA Senate Finance Committee
- Stefanski eventually acknowledged receiving tech company funding but "flatly refused to name which companies"
- Stefanski named "the founder's father as its largest donor" (founder = Melissa McKay)
- Meta confirmed it has "collaborated with Digital Childhood Alliance"
- Source: https://www.insurancejournal.com/news/national/2025/07/25/833246.htm
- Source: https://www.deseret.com/opinion/2025/12/07/child-safety-bill-backed-by-meta/

### Leadership:
- **Casey Stefanski** — Executive Director
  - Former Senior Director of Global Partnerships/Events at NCOSE (10 years)
  - U of Chicago, public policy + economics
  - Capitol Hill experience
- **Melissa McKay** — Founder (also founded Digital Childhood Institute)
  - Utah-based mother of five
  - "Personally funded the first draft of model legislation" (ASAA)
  - Also runs digitalchildhoodinstitute.org (501(c)(3) arm)
- **John Read** — Senior Policy Counsel
  - 30 years at US DOJ Antitrust Division
  - Investigated app stores and Big Tech

### Claims:
- 140+ (later 170+) member organizations
- Led passage of Utah App Store Accountability Act (2025)
- DCA "paid attorneys to draft the model legislation"
- Has filed FTC complaints against Apple and Google
- Has met with Google "several times"

## 5. CONNECTSAFELY INC (FOR REFERENCE)

- **EIN:** 47-3168168
- **Address:** 3481 Greer Rd, Palo Alto, CA 94303
- **Revenue (2023):** $653,869
- **Status:** 501(c)(3)
- Very small org ($400K-$950K/year range)
- Source: ProPublica Nonprofit Explorer

## 6. ICMEC (FOR REFERENCE)

- **Name:** The International Centre For Missing And Exploited Children
- **EIN:** 22-3630133
- **Location:** Alexandria, VA
- Full filing details: pending (API returned 400 on detail query)

---

## OPEN THREADS FOR FOLLOW-UP

1. **NVF 990 Schedule I grants** — need machine-readable XML to search 1,000+ recipients for DCA/ConnectSafely/ICMEC grants
2. **Colorado SOS business filings** — DCA incorporation documents, registered agent
3. **Headwaters Strategies lobbying expenditure reports** — how much has Meta paid through Headwaters?
4. **FOIA responses** due 03/13-03/14 — may show direct coordination
5. **CO General Assembly witness lists** for SB26-051, SB25-086, HB25-1287 — did DCA, Headwaters, and Meta all appear?
6. **FEC/TRACER** — any Headwaters/Eichberg/Coyne contributions to CO bill sponsors?
7. **LinkedIn deep dive** — Headwaters staff prior employment, DCA staff connections
8. **DCA's DCI 501(c)(3) arm** — digitalchildhoodinstitute.org — may have 990 with donor data
9. **WHOIS history** — historical WHOIS data may show pre-privacy registrant
10. **Sixteen Thirty Fund** as 501(c)(4) — could be funding DCA's political operations
