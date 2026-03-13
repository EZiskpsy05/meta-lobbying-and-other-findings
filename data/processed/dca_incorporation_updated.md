# DCA & DCI Corporate Registration — Updated Analysis

**Research Date:** 2026-03-13
**Data Sources:** IRS Business Master File (eo1-eo4 extracts), OpenCorporates API, ProPublica, GuideStar, state corporate registries

---

## Executive Summary

The Digital Childhood Institute (DCI) was confirmed in the IRS Business Master File with **EIN 39-3684798**, incorporated in **Delaware** at a registered agent address (213 N Market St #1039, Wilmington). However, the **Digital Childhood Alliance (DCA) does NOT appear in the IRS BMF at all** — across all four regional extract files covering every tax-exempt organization in the United States. Neither entity appears in OpenCorporates (200M+ companies indexed), ProPublica Nonprofit Explorer, or GuideStar.

This finding raises significant questions about DCA's legal structure: it may operate as a self-declared 501(c)(4) without formal IRS determination, as a fiscal sponsorship under another entity, or under a different legal name.

---

## 1. Digital Childhood Institute (DCI) — IRS Record Found

**Source:** IRS Exempt Organizations Business Master File (eo2.csv, March 2026 extract)

| Field | Value |
|-------|-------|
| EIN | 39-3684798 |
| Name | DIGITAL CHILDHOOD INSTITUTE |
| Address | 213 N Market St #1039, Wilmington, DE 19801-2527 |
| Subsection | 03 — 501(c)(3) |
| Ruling Date | November 2025 (202511) |
| Deductibility | Yes (contributions tax-deductible) |
| Foundation Status | 15 — organization which is not a private foundation |
| Status | 01 — unconditional exemption |
| Filing Requirement | 990 required |

### Address Analysis

213 N Market St #1039, Wilmington, DE 19801 is a **registered agent service address** — a commercial mail-forwarding location commonly used by Delaware-incorporated entities. This is standard practice for Delaware incorporations and does not indicate physical operations at this location.

DCI's actual operations appear to be in **Utah** (McKay is in American Fork/Lehi area).

---

## 2. Digital Childhood Alliance (DCA) — NOT IN IRS RECORDS

**Search conducted:** All four IRS EO regional extract files (eo1.csv through eo4.csv), covering every tax-exempt organization registered with the IRS.

**Search terms:** "digital childhood" (case-insensitive)

**Result:** Only DCI (EIN 39-3684798) was found. **DCA does not appear under any variant of its name.**

### What This Means

501(c)(4) organizations are **not required to apply for IRS recognition** of tax-exempt status (unlike 501(c)(3)s which must file Form 1023/1024). A 501(c)(4) can:

1. **Self-declare** its tax-exempt status by simply filing a Form 990 annually
2. **Voluntarily apply** for IRS determination by filing Form 8976 (notice of intent) and Form 1024-A

The absence of DCA from the IRS BMF means one of:

| Scenario | Likelihood | Implication |
|----------|-----------|------------|
| DCA has not yet filed Form 990 | **High** — first filing not due until ~May 2026 | Organization exists but hasn't completed first IRS reporting cycle |
| DCA has not filed Form 8976 | **Possible** — 501(c)(4)s must notify IRS within 60 days of formation, but enforcement is limited | Would be a technical noncompliance |
| DCA operates as a fiscal sponsorship | **Possible** — would explain both the IRS absence and the inability to find incorporation records | DCA's funds would flow through the sponsoring entity's EIN |
| DCA is registered under a different legal name | **Less likely** — would be deceptive given its public branding | Would require further investigation |

### Implications for the Meta Funding Investigation

If DCA operates as a **fiscal sponsorship** under another 501(c)(4), this would:
- Explain the absence of any DCA EIN, incorporation record, or IRS filing
- Mean DCA's finances are embedded within the sponsor entity's 990
- Make DCA's funding even more opaque than a standalone 501(c)(4)
- Be consistent with the Arabella network model (which operates hundreds of "sponsored projects" within its entities)

---

## 3. Database Search Results — Neither Entity Found

| Database | DCA | DCI |
|----------|-----|-----|
| IRS Business Master File | **NOT FOUND** | Found (EIN 39-3684798) |
| OpenCorporates (200M+ companies) | Not found | Not found |
| ProPublica Nonprofit Explorer | Not found | Not found |
| GuideStar / Candid | Not found | Not found |
| Charity Navigator | Not found | Not found |
| DC DLCP (CorpOnline) | Requires interactive search | Requires interactive search |
| Delaware ICIS | Requires interactive search | Requires interactive search |
| Virginia SCC | Not found | Not found |
| Utah Business Entity Search | Requires interactive search | Requires interactive search |

---

## 4. DCA's Network for Good Connection

DCA processes donations through **Network for Good** (digitalchildhoodalliance.networkforgood.com), using Network for Good's EIN (68-0480736). This is consistent with either:
- A new organization that hasn't set up its own payment processing
- A fiscal sponsorship arrangement where Network for Good handles donations on DCA's behalf

---

## 5. Updated DCA/DCI Comparison

| Feature | DCA | DCI |
|---------|-----|-----|
| Tax Status | Claims 501(c)(4) | Confirmed 501(c)(3) |
| EIN | **Not found in IRS records** | 39-3684798 |
| IRS Determination | **None found** | November 2025, unconditional |
| Incorporation State | **Unknown** | Delaware |
| Registered Address | Unknown | 213 N Market St #1039, Wilmington, DE |
| Operational Location | Washington, DC | Utah (McKay) |
| Domain Registered | 2024-12-18 | 2025-06-13 |
| Registration Length | 4 years | 1 year |
| Donation Processing | Network for Good | Unknown |
| Coalition | 140+ (claimed) / 50+ (confirmed) | N/A |
| First 990 Due | ~May 2026 (if standalone) | ~May 2027 |

---

## Sources

- IRS Exempt Organizations BMF: https://www.irs.gov/charities-non-profits/exempt-organizations-business-master-file-extract-eo-bmf
- IRS EO Extract files: https://www.irs.gov/pub/irs-soi/eo1.csv through eo4.csv
- OpenCorporates API: https://api.opencorporates.com/v0.4/companies/search
- ProPublica Nonprofit Explorer: https://projects.propublica.org/nonprofits/
- DCA Idealist Profile: https://www.idealist.org/en/nonprofit/digital-childhood-alliance-washington
- DCA Network for Good: https://digitalchildhoodalliance.networkforgood.com/
