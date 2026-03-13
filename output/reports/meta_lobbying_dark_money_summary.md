# Meta Platforms: Lobbying, Funding, and Dark Money Networks
## Comprehensive Research Summary

**Compiled:** 2026-03-12
**Status:** Active investigation — multiple threads remain open
**Classification:** OSINT research product — all sources are public records

---

## I. EXECUTIVE SUMMARY

Meta Platforms has built a multi-layered influence operation to advance age verification legislation that shifts compliance burdens from social media platforms (its own products) to app store operators (Apple and Google). This operation spans direct lobbying ($26.3M federal in 2025, lobbyists in 45 states), covert funding of a nominally independent advocacy group (Digital Childhood Alliance), and personnel connections to one of the largest dark money networks in the United States (Arabella Advisors). The investigation has established five confirmed funding and influence channels, one structurally possible but unproven dark money pipeline, and a pattern of deliberate opacity designed to obscure Meta's role.

### Key Numbers

| Metric | Value |
|--------|-------|
| Meta federal lobbying (2025) | **$26.29 million** (all-time record) |
| Meta registered lobbyists | **86+** across **45 states** |
| Meta → Headwaters Strategies (CO) | **$338,500** (2019-2026) |
| Meta California super PACs | **$65 million** |
| NVF → Sixteen Thirty Fund transfers | **$121.3 million** (2022-2024) |
| All 5 Arabella entities grants analyzed | **4,433 grants (~$2.0 billion)** — ZERO to child safety |
| Arabella network combined revenue | **>$1 billion/year** |
| States with ASAA bills introduced | **~20** |
| States with ASAA signed into law | **3** (UT, LA, TX) |
| DCA coalition member organizations | **50+** |

---

## II. THE FIVE CONFIRMED CHANNELS

### Channel 1: Direct State Lobbying

Meta retains lobbying firms and individual lobbyists in at least 45 states. Confirmed operations:

**Colorado — Headwaters Strategies**
- Firm: Headwaters Strategies (est. 2009)
- Principals: Adam Eichberg (co-founder), Will Coyne (co-founder), Alyson Schmidt, Amber Burkhart
- Total Meta payments: **$338,500** (2019-2026, per CO SOS SODA API)
- Payment escalation: $5K/month (2019) → $30K single month (Jul 2023) → $8.5K/month (2025)
- Bills lobbied: SB26-051 (Age Attestation), SB25-086 (Social Media Protections), HB25-1287 (Social Media Tools for Minors) — position: "Monitoring" and "Amending"
- Additional CO Meta lobbyists: Ana Martinez (~$102K, 2021-2026), Dan Sachs (~$11K, 2021-2026)
- **Total disclosed CO lobbying payments to Meta lobbyists: ~$451,441**

**Louisiana — Pelican State Partners LLC + 8 Additional Firms**
- **12 lobbyists across 9 firms**, at least **$324,992** total ("very conservative estimate")
- Confirmed firms: **Pelican State Partners** (Koch, Rhodes, Kirkpatrick, Satpathi, Albrecht), **Adams and Reese LLP** (Wilkerson, Brooks — #1 ranked LA gov affairs firm), **State Capitol Solutions** (Borill)
- Meta NOT on Koch's 2023 registration — retained **2024-2025** specifically for ASAA campaign
- Also represents: **Roblox Corporation** (another ASAA beneficiary), Uber, AT&T, BP America
- **A Meta lobbyist "brought legislative language" directly to sponsor Rep. Kim Carver** — confirmed by Carver publicly
- **Nicole Lopez** (Meta Director of Global Litigation Strategy for Youth) testified at House Commerce Committee
- **HB-570 signed by Gov. Landry, June 30, 2025** — effective July 1, 2026
- **Key amendment battle:** Sen. Jay Morris expanded bill to include app developers alongside app stores; conference committee compromise maintained dual responsibility

**California — Record-Breaking Spend**
- Direct CA lobbying: **$1,036,728** (Q1-Q3 2025), Q2 alone was $518,605 (single-quarter record)
- Super PAC: **META California** ($20M), led by Brian Rice (Meta VP Public Policy) and Greg Maurer
- Super PAC: **ATEP** ($45M), bipartisan PAC run by Republican Brian Baker and Democratic Hilltop Public Solutions
- CA Chamber of Commerce payments: **$3.1 million**
- Trade association lobbying: TechNet (~$200K), Chamber of Progress (~$200K)
- Supported **AB-1043** (Digital Age Assurance Act, signed Oct 2025) — shifts age verification to OS providers

**Federal — 86+ Lobbyists**
- 2025 spend: **$26.29 million** (all-time record, up from $24.4M in 2024)
- 40+ lobbying firms retained, 87 lobbyists (85% "revolving door"), ~1 per 6 members of Congress
- **LD-2 filings explicitly list H.R. 3149/S. 1586, App Store Accountability Act** as a lobbied bill (CPI issue code)
- LD-2 narrative includes: "protecting children, bullying prevention and online safety; youth safety and federal parental approval; youth restrictions on social media"
- Also lobbies on KOSA (S. 1748) and COPPA 2.0 (S. 836) — likely opposing/amending bills that regulate Meta directly
- 12 in-house lobbyists include 3 former senior Senate committee counsel (Commerce, Judiciary)
- App Store Accountability Act introduced federally by Rep. John James (R-MI, H.R. 3149) and Sen. Mike Lee (R-UT, S. 1586), May 2025

### Channel 2: Digital Childhood Alliance (DCA) — Astroturf Advocacy

Meta covertly funds DCA, a 501(c)(4) advocacy group that presents itself as a grassroots coalition of conservative child safety organizations.

**Organizational Profile:**
- Tax status: 501(c)(4) — **no legal obligation to disclose donors**
- Location: Washington, DC
- Domain registered: **2024-12-18** (GoDaddy, privacy-protected, 4-year registration through 2028)
- Website live: **2024-12-19** (fully formed, professionally designed)
- Public launch: **~February 28, 2025**
- EIN: **Not found in IRS Business Master File** — searched all 4 regional extracts (eo1-eo4.csv) covering every tax-exempt organization in the US
- No incorporation record found in CO, DC, DE, VA, OpenCorporates (200M+ companies), ProPublica, GuideStar, or Charity Navigator
- Processes donations through **Network for Good / For Good** (EIN 68-0480736) — a **Donor Advised Fund** (not a payment processor). DCA is classified as a "Project" (ID 258136) in the NFG/Bonterra system. For Good explicitly limits grants to 501(c)(3) organizations, raising compliance questions about DCA's c4 status.
- **NCOSEAction** (EIN 88-1180705), NCOSE's confirmed 501(c)(4) affiliate, is a potential fiscal sponsor — same leadership (Marcel van der Watt), IRS ruling May 2025

**Leadership — NCOSE and DOJ Antitrust Origins:**

| Name | Title | Background |
|------|-------|------------|
| Casey Stefanski | Executive Director | 10 years at NCOSE (Senior Dir. Global Partnerships) |
| Dawn Hawkins | Chair | CEO, National Center on Sexual Exploitation (dual role) |
| Melissa McKay | Chair/Board President | Utah mother of five, DCI founder, #FixAppRatings activist since 2019 |
| John Read | Senior Policy Advisor | **30 years at DOJ Antitrust Division** — investigated app stores and Big Tech |

**Funding Exposure:**
1. **April 2025**: LA Sen. Jay Morris directly questioned Stefanski about tech funding at Senate Finance Committee hearing
2. Stefanski "squirmed, deflected and claimed she 'didn't feel comfortable' answering"
3. When pressed for yes/no, admitted receiving tech company funding but **refused to name companies**
4. **July 2025**: Bloomberg reporters exposed Meta as DCA funder
5. **December 2025**: Brian Lenney op-ed in Deseret News detailed Meta's manipulation

**Coalition Members (confirmed):**
- National Center on Sexual Exploitation (NCOSE)
- The Heritage Foundation
- Institute for Family Studies
- Ethics and Public Policy Center
- Moms for Liberty
- Protect Young Eyes
- 45+ additional organizations

**Strategic Function:**
DCA exclusively targets **Apple and Google app stores** — never Meta, Facebook, or Instagram. Every blog post, testimony, and press release frames app stores as the problem. This perfectly serves Meta's interest: if ASAA becomes law, age verification responsibility falls on Apple/Google, not on social media platforms.

### Channel 3: Digital Childhood Institute (DCI) — Research Arm

**Related entity to DCA:**

| Field | DCI | DCA |
|-------|-----|-----|
| Tax status | 501(c)(3) | 501(c)(4) |
| EIN | 39-3684798 | **Not in IRS BMF** |
| IRS ruling | November 2025 | None found |
| Incorporation | Delaware (213 N Market St #1039, Wilmington) | **Unknown — not in any registry** |
| President | Melissa McKay | Casey Stefanski (ED) |
| Claimed funding | "Does not accept major tech platform funding" | Admits tech funding, won't name companies |

**Shared Infrastructure (DCA ↔ DCI):**
- Same registrar: GoDaddy
- Same CDN: Cloudflare
- Same email: Microsoft 365
- Same email marketing: **Elastic Email** (distinctive shared platform)
- Same Google verification

DCA registered 6 months before DCI — unusual, as typically the research/education arm (c)(3) precedes the lobbying arm (c)(4). This reverse order suggests DCA was the primary objective.

### Channel 4: Super PACs and Trade Associations

**Total documented political spending: $70+ million**

| Entity | Meta $ | Type | Key Personnel |
|--------|--------|------|--------------|
| ATEP | $45,000,000 | 527 PAC, bipartisan | Brian Baker (R) + **Hilltop Public Solutions** (D) |
| META California | $20,000,000 | State PAC | Brian Rice (Meta VP Public Policy) |
| California Leads | $5,000,000 | State PAC | — |
| Forge the Future | (from ATEP) | State PAC (TX), Republican | Registered Fremont, CA Jan 2026 |
| Making Our Tomorrow | (from ATEP) | State PAC (IL), Democrat | Brian Rice (Meta VP Public Policy) |
| California Chamber of Commerce | $3,100,000 | CA lobbying | — |
| TechNet | Member | Trade association | — |
| Chamber of Progress | Member | Trade association | — |

**Critical:** All super PACs are **state-level entities**, not FEC-registered — filings scattered across state ethics commissions rather than searchable federal database. This is deliberate transparency avoidance.

**Forge the Future policy priorities** include: "Empowering parents with oversight of children's online activities across devices and digital environments" — **functionally identical to ASAA framing.**

**Hilltop Public Solutions** co-leads ATEP AND was previously identified in DCA's messaging coordination — the first firm connected to both Meta's super PAC operation and the DCA astroturf campaign.

**Notable:** Meta's own trade associations (TechNet, Chamber of Progress) **opposed** AB-1043, while Meta itself **supported** it — breaking ranks with its own industry groups.

### Channel 5: State Legislative Campaigns

**Enacted ASAA Laws:**

| State | Bill | Signed | Effective | Key Details |
|-------|------|--------|-----------|-------------|
| Utah | SB-142 | Mar 26, 2025 | Immediate | First in nation; McKay provided key testimony |
| Texas | SB 2420 | May 2025 | Jan 1, 2026 | **Paused by federal judge, Dec 2025** |
| Louisiana | HB-570 | Jun 30, 2025 | Jul 1, 2026 | 12 Meta lobbyists; Morris/Stefanski confrontation |

**Pending/Target States:** Kansas (Mar 2026), South Carolina, Ohio, Georgia, Florida, ~15 others

**Federal:** App Store Accountability Act (Lee/Lankford, May 2025) — DCA claims 100+ advocate endorsements

---

## III. THE ARABELLA ADVISORS DARK MONEY NETWORK

### The Nexus: Adam Eichberg

Adam Eichberg occupies the single most significant position connecting Meta's lobbying operation to the largest dark money network in the United States:

| Role | Entity | Significance |
|------|--------|-------------|
| **Co-founder & Principal** | Headwaters Strategies | Meta's Colorado lobbying firm ($338,500 received) |
| **Board Chair** | New Venture Fund (NVF) | Arabella's primary 501(c)(3), $669M revenue (2023) |
| **Founding Board Member** | Windward Fund | Arabella's $311M 501(c)(3) |

### The Arabella Network

Four entities sharing **1828 L Street NW, Washington, DC 20036**, all managed by Arabella Advisors (now Sunflower Services):

| Entity | Suite | Type | Revenue (2023-2024) | Assets |
|--------|-------|------|---------------------|--------|
| New Venture Fund | 300-A | 501(c)(3) | $669M | $768M |
| Sixteen Thirty Fund | 300-B | 501(c)(4) | $282M | $107M |
| Windward Fund | 300-C | 501(c)(3) | $311M | $433M |
| Hopewell Fund | 300-D | 501(c)(3) | $114M (grants) | $173M |
| **Combined** | — | — | **>$1.3 billion** | **>$1.4 billion** |

### NVF Schedule I Analysis — Definitive Negative Finding

Analysis of **2,669 grant recipients** across NVF's 2022-2024 Schedule I filings found:

- **ZERO grants** to ConnectSafely, ICMEC, NCMEC, FOSI, Thorn, Common Sense Media, DCA, DCI, NCOSE, 5Rights, FairPlay, CDT, NetChoice, Chamber of Progress, TechNet, EFF, or FOSI
- **ZERO grants** matching digital safety, online protection, or age verification keywords
- **$121.3 million** transferred to Sixteen Thirty Fund (c)(4)
- **$20.9 million** transferred to North Fund
- **$8.8 million** transferred to Hopewell Fund
- **$150.9 million total** in internal Arabella network transfers

NVF's grant portfolio is overwhelmingly progressive civic engagement, voting rights, environmental programs, and international development — not technology policy.

### Sixteen Thirty Fund Schedule I Analysis — Definitive Negative Finding

Analysis of **306 of 318 grant recipients** ($207.8M of $236.5M) from STF's 2024 Schedule I filing found:

- **ZERO grants** to any child safety, age verification, digital childhood, or tech policy organization
- **ZERO keyword matches** for child, safety, age, digital, online, internet, cyber, tech, or protect
- Grant portfolio: progressive civic engagement ($27.8M America Votes), reproductive rights ($14M Floridians Protecting Freedom), environmental ($11.8M League of Conservation Voters), voter registration ($7.8M Register America)
- **Internal Arabella transfers:** STF → NVF $162K (reverse flow), STF → Hopewell $1.4M, STF → North Fund $6.8M
- Only parent-related grant: **ParentsTogether Action** ($30K) — focused on economic parenting issues, NOT tech/online safety

**Final Arabella Network Finding:** Across all five entities (NVF + STF + North Fund + Windward + Hopewell), **4,433 grants** totaling **~$2.0 billion** have been analyzed, with **zero dollars** going to any organization related to child online safety, age verification, or the App Store Accountability Act. The Schedule I grant pathway is **definitively ruled out** across the entire Arabella network.

### Complete Arabella Network Transfer Map (2024)

```
NVF ──$121.3M──→ Sixteen Thirty Fund ──$6.8M──→ North Fund ──$5.3M──→ STF (circular)
NVF ──$8.8M────→ Hopewell Fund                  North Fund ──$250K──→ Windward
NVF ──$20.9M───→ North Fund                     North Fund ──$150K──→ Hopewell

STF ──$162K────→ NVF (reverse)
STF ──$1.4M────→ Hopewell Fund
STF ──$6.8M────→ North Fund
```

The NVF → STF → North Fund → STF circular flow ($121.3M → $6.8M → $5.3M) confirms these entities operate as a unified financial network with bidirectional and circular transfers.

### The Opaque Pipeline — Structurally Possible, Unproven

```
Meta Platforms, Inc.
     │
     ├──[CONFIRMED]──→ Headwaters Strategies ($338,500 CO lobbying)
     │                      │
     │                      └── Adam Eichberg ──→ NVF Board Chair
     │                                                  │
     │                                    [CONFIRMED: $121.3M transfers]
     │                                                  │
     │                                                  ▼
     │                                    Sixteen Thirty Fund (c)(4)
     │                                    [Donors NOT disclosed]
     │                                    [$236.5M in grants, 318 recipients]
     │                                    [ANALYZED: ZERO child safety grants]
     │                                                  │
     │                                    [RULED OUT via Schedule I]
     │                                    [Remaining paths: fiscal sponsorship,
     │                                     non-grant payments, lobbying expenditures]
     │
     ├──[CONFIRMED]──→ Digital Childhood Alliance (direct funding, per Bloomberg)
     │
     ├──[CONFIRMED]──→ Pelican State Partners (LA lobbying)
     │
     ├──[CONFIRMED]──→ Super PACs ($65M CA, ATEP)
     │
     └──[CONFIRMED]──→ 86+ federal lobbyists ($26.3M)
```

**What we know:** Eichberg chairs NVF. NVF sends $121M to Sixteen Thirty Fund. Sixteen Thirty Fund makes $236M in grants to 318 recipients. **All 318 recipients have now been analyzed — NONE are child safety or tech policy organizations.** As a 501(c)(4), Sixteen Thirty Fund's donors are **never publicly disclosed**.

**What this means:** The Schedule I grant mechanism is **ruled out** as the pathway for Meta → Arabella → DCA funding. If Meta funds flow through the Arabella network, they would have to travel via:
1. **Fiscal sponsorship** — DCA operating as a "sponsored project" within an Arabella entity (would not appear on Schedule I)
2. **Non-grant payments** — consulting fees, service contracts, or management fees (not on Schedule I)
3. **NVF lobbying expenditures** — NVF's $36.7M in lobbying expenditures (Part IX) could support advocacy without being classified as grants
4. **All Arabella entities now analyzed** — Windward ($249M, environmental), Hopewell ($197M, civic/health), North Fund ($59M, civic) — ALL ZERO child safety grants. Remaining paths: fiscal sponsorship, non-grant payments, NVF lobbying expenditures ($36.7M)

**Why it still matters:** The Eichberg dual role creates structural access to dark money infrastructure even though the most obvious pathway (Schedule I grants) is now excluded. The remaining pathways (fiscal sponsorship, non-grant payments) are inherently less transparent than Schedule I.

---

## IV. CONNECTED ORGANIZATIONS AND PERSONNEL

### ConnectSafely Inc.

| Field | Value |
|-------|-------|
| EIN | 47-3168168 |
| Type | 501(c)(3) |
| Location | 3481 Greer Rd, Palo Alto, CA 94303 |
| Revenue | $784,500 (2024) |
| CEO | Larry Magid ($218,708 compensation) |

- Magid serves on **Meta's Safety Advisory Council**
- Receives funding from Facebook, Google, Microsoft, Snapchat
- **Opposes** certain child safety bills
- **Not funded by NVF** (confirmed via Schedule I analysis)

### NCOSE — DCA's Institutional Parent

The National Center on Sexual Exploitation provides DCA's leadership:
- CEO Dawn Hawkins **chairs DCA** simultaneously
- Casey Stefanski spent **10 years at NCOSE** before becoming DCA Executive Director
- NCOSE's VP Public Policy (Eleanor Gaetan) appears as DCA testimonial
- NCOSE provided the institutional infrastructure for DCA's rapid launch

**NCOSE's 501(c)(4) Affiliate — Confirmed:**

| Field | NCOSE (c)(3) | NCOSEAction (c)(4) |
|-------|-------------|-------------------|
| EIN | 13-2608326 | **88-1180705** |
| Address | 1201 F St NW, DC | 1201 F St NW, Ste 200, DC |
| Leadership | Marcel van der Watt (CEO) | Marcel van der Watt (Principal Officer) |
| Revenue | $7.3M (2023) | $0 (no filing yet) |
| IRS Ruling | December 1963 | **May 2025** |
| Filing | 990 required | 990-N (e-Postcard, ≤$50K) |

NCOSE's website: "NCOSEAction, a 501c(4) political action organization created by NCOSE, exists to ensure that good laws are passed and bad laws are prevented from being enacted."

**Fiscal sponsor candidate:** NCOSEAction has the correct tax status (c4), direct personnel overlap with DCA (Hawkins chairs DCA, reports to van der Watt who controls NCOSEAction), and its May 2025 IRS ruling aligns with DCA's operational timeline. Zero reported revenue may indicate either dormancy or that the first filing hasn't been processed.

### Pelican State Partners — Koch's Firm

| Field | Value |
|-------|-------|
| Founded | ~2020 (spun out of Roedel Parsons) |
| Key lobbyist | John Dunbar Koch (LB000349) |
| Partners | Rhodes, Kirkpatrick, Satpathi, Albrecht |
| Tech clients | **Meta Platforms**, Roblox, Uber, AT&T |
| Other clients | Walmart, BP America, CVS, Equifax, HCA Healthcare |
| Total clients | 30+ (2023 registration) |

Koch's surname is "Koch" — **no connection to Koch Industries** or the Koch political network. He is a traditional Louisiana multi-client lobbyist who added Meta as a client in 2024-2025 for the ASAA campaign.

### Other Coordination Entities

Per investigative reporting, DCA's messaging involves:
- **DCI Group** — lobbying/PR firm
- **Hilltop Public Strategies** — messaging coordination (also involved with ATEP super PAC)

---

## V. WEBSITE AND DIGITAL FORENSICS

### DCA Domain Analysis

| Feature | DCA | DCI |
|---------|-----|-----|
| Registrar | GoDaddy | GoDaddy |
| Created | 2024-12-18 | 2025-06-13 |
| Registration length | 4 years (through 2028) | 1 year |
| CDN | Cloudflare | Cloudflare |
| Email | Microsoft 365 | Microsoft 365 |
| Email marketing | Elastic Email | Elastic Email |
| Additional email | Google, Amazon SES | — |

DCA's 4-year registration and more sophisticated infrastructure indicate significantly more funding than DCI.

### Wayback Machine Analysis (100+ snapshots)

- First snapshot: **2024-12-19 03:51 UTC** — one day after domain registration
- Site launched fully formed with professional design, statistics, testimonials
- Heritage Foundation and NCOSE staff featured prominently from day one
- **No funder disclosures ever existed** on any version of the site
- Every blog post targets Apple/Google — Meta is never mentioned or criticized
- Cloudflare intermittently blocks archival (403 errors)
- Key sub-pages (/about-us/, /our-team/) only archived from September 2025

---

## VI. CAMPAIGN CONTRIBUTIONS — CO TRACER ANALYSIS

Analysis of Colorado TRACER bulk data (132MB, 2024-2026) for campaign contributions connecting investigation targets to ASAA bill sponsors.

### Meta Employee → ASAA Sponsor Contributions

| Date | Contributor | Employer | Amount | Recipient | Candidate |
|------|------------|----------|--------|-----------|-----------|
| **2025-06-02** | **Jake Levine** | **Meta** (Product Manager, LA) | **$450** | Matt Ball for Colorado | **Matt Ball** (SB26-051 sponsor) |
| **2025-06-02** | **Jake Levine** | **Meta** | **$725** | Ball for All Leadership Fund | **Matt Ball** leadership PAC |
| 2025-03-24 | Kyle Gardner | Google (Policy Manager) | $450 | Matt Ball for Colorado | Matt Ball |
| 2025-06-14 | James Rosenthal | Pinterest (Attorney) | $450 | Matt Ball for Colorado | Matt Ball |

**Key Finding:** A Meta Product Manager contributed **$1,175** to ASAA sponsor Matt Ball's campaign apparatus on the same day. A Google Policy Manager also contributed to the same legislator. Multiple tech company employees from companies directly affected by ASAA targeted the same bill sponsor.

### Headwaters Strategies Staff — No ASAA-Sponsor Contributions

- **Adam Eichberg:** 21 contributions/$10,176 (2023-2025) — broadly Democratic, $1,776 to Bennet for Governor. **No contributions to Ball or Paschal.**
- **Will Coyne:** 36 contributions/$10,035 (2023-2025) — similar pattern. **No contributions to Ball or Paschal.**
- Both list "Headwaters Strategies" as employer, "Lobbyist"/"Consultant" as occupation
- Pattern: standard lobbyist behavior — wide distribution at $450 max contribution limit
- Bipartisan exceptions (both gave to Barbara Kirkmeyer, Republican)

### No Meta PAC or Corporate Contributions

No contributions from Meta PAC, Facebook PAC, or any Meta corporate entity to either Ball or Paschal found in Colorado TRACER data.

### Multi-State Contribution Search (FollowTheMoney.org)

Search of FollowTheMoney.org entity profiles across all four ASAA states found **no direct campaign contributions** from Meta PAC, Facebook PAC, Digital Childhood Alliance, Adam Eichberg, or Headwaters Strategies to any ASAA bill sponsor.

**ASAA Bill Sponsors Identified:**

| State | Bill | Sponsor(s) |
|-------|------|-----------:|
| Utah | SB-142 | Sen. Todd Weiler (R) |
| Louisiana | HB-570 | Rep. Kim Carver (R-Bossier City) |
| Texas | SB 2420 | Sen. Angela Paxton (R), Rep. Caroline Fairly (R) |
| Colorado | SB26-051 / HB25-1287 | Sen. Matt Ball (D), Rep. Amy Paschal (D), Rep. Jarvis Caldwell (R), Rep. Meghan Lukens (D) |

**Key Findings:**
- **Todd Weiler (UT, SB-142):** Has a long-standing policy of **not accepting corporate contributions** — returned $20K+ in unsolicited checks in 2012. Reportedly has **not discussed ASAA directly with Meta.** DCA served as the intermediary to a legislator who could not be directly lobbied through contribution channels.
- **Kim Carver (LA, HB-570):** First-term legislator. HB-570 passed unanimously (99-0, 39-0). DCA's Stefanski and Meta's Nicole Lopez both testified in support. No Meta contributions found.
- **Angela Paxton & Caroline Fairly (TX, SB 2420):** Meta's **Forge the Future super PAC** reported **$1.3M in Texas expenditures** ahead of March 2026 primaries, backing "pro-innovation" Republican candidates. No direct Meta PAC → sponsor contributions confirmed.
- **Matt Ball (CO, SB26-051):** **Appointed** (not elected), limiting standard fundraising disclosure. Jake Levine (Meta PM) contributed $1,175 via CO TRACER (established in prior analysis).

**Strategic Implication:** The absence of direct contributions clarifies Meta's influence model — legislators don't need to be "bought" when DCA frames the issue as child protection. The influence operates through lobbying and advocacy channels, not traditional campaign contributions.

---

## VII. WHAT THE EVIDENCE SHOWS

### Proven

1. **Meta funds DCA** — confirmed by Bloomberg, partially admitted by Stefanski under oath
2. **Meta deployed 86+ lobbyists** across 45 states for ASAA and related campaigns
3. **Meta spent $26.3M on federal lobbying** in 2025 (all-time record)
4. **Meta paid Headwaters Strategies $338,500** for Colorado lobbying (2019-2026)
5. **Adam Eichberg** simultaneously leads Meta's CO lobbying firm and chairs the NVF board
6. **NVF transfers $121.3M** to Sixteen Thirty Fund (c)(4) annually
7. **NVF does NOT directly fund** any child safety or tech policy organizations via Schedule I
8. **DCA and DCI share infrastructure** — same registrar, CDN, email, and marketing platform
9. **Pelican State Partners represents Meta** as a lobbying client in Louisiana
10. **DCA leadership comes from NCOSE** — three of four senior staff have NCOSE connections
11. **DCA's John Read** spent 30 years at DOJ Antitrust investigating app stores
12. **ASAA has passed in 3 states** (UT, LA, TX) with Texas paused by a federal judge
13. **Sixteen Thirty Fund does NOT fund** any child safety or tech policy organizations via Schedule I (306/318 recipients analyzed)
14. **All 5 Arabella entities analyzed:** 4,433 grants (~$2.0B) with ZERO child safety/tech policy funding — Schedule I pathway definitively ruled out across entire network
15. **A Meta employee (Jake Levine)** contributed $1,175 to ASAA sponsor Matt Ball's campaign apparatus
16. **A Google Policy Manager (Kyle Gardner)** also contributed $450 to Matt Ball — multiple tech company employees targeting the same ASAA sponsor
17. **Eichberg and Coyne did NOT contribute** to ASAA bill sponsors Ball or Paschal despite $20K+ combined political giving
18. **No direct Meta PAC contributions to any ASAA sponsor** across UT, LA, TX, CO — confirmed via FollowTheMoney.org multi-state search
19. **Todd Weiler does not accept corporate contributions** — DCA served as policy intermediary to legislator unreachable through standard contribution channels
20. **DCA has no EIN in the IRS Business Master File** — not found in any of four regional extracts covering all US tax-exempt organizations; consistent with fiscal sponsorship or pre-first-filing status
21. **DCI confirmed in IRS BMF** (EIN 39-3684798) — Delaware incorporation, registered agent at 213 N Market St Wilmington, ruling November 2025
22. **Meta's Forge the Future super PAC** spent **$1.3M in Texas** ahead of March 2026 primaries, backing "pro-innovation" Republican candidates
23. **DCA's website deployed < 24 hours after domain registration** — fully functional advocacy site with professional design, statistics, Heritage/NCOSE testimonials; indicates pre-built staging deployment, not grassroots launch
24. **77-day domain-to-legislation pipeline** — DCA domain registered Dec 18, 2024; Utah SB-142 signed Mar 5, 2025. Site pre-loaded with ASAA talking points before any bill had passed
25. **Meta deployed 12 lobbyists for Louisiana HB-570** which passed 99-0 — disproportionate deployment indicates text-control and amendment-blocking, not vote persuasion
26. **Three California tech policy employees** from Meta, Google, and Pinterest contributed to Matt Ball within 90 days — all from ASAA-affected companies, all out-of-state, targeting a newly-appointed senator
27. **Pelican State Partners represents both Meta AND Roblox** in Louisiana — both ASAA beneficiaries, enabling "broad industry support" framing
28. **DCA's coalition count inflated from 50+ to 140+** with only 6 organizations ever publicly named; no member list has ever been published on the website
29. **NCOSE has a confirmed 501(c)(4) affiliate** — NCOSEAction (EIN 88-1180705), IRS ruling May 2025, same address and leadership as NCOSE. Principal officer: Marcel van der Watt (also NCOSE President/CEO)
30. **Network for Good is a Donor Advised Fund**, not a payment processor — DCA is classified as "Project" (ID 258136) in the system; For Good explicitly limits grants to 501(c)(3) organizations
31. **A Meta lobbyist drafted HB-570's legislative language** — confirmed by sponsor Rep. Kim Carver; the bill as originally written placed age verification burden exclusively on app stores, not platforms
32. **Sen. Jay Morris's amendment expanded HB-570** to include app developers alongside app stores — the key amendment battle, resulting in a conference committee compromise
33. **Nicole Lopez** (Meta Dir. of Global Litigation Strategy for Youth) testified in both Louisiana and South Dakota for ASAA bills — Meta's national ASAA spokesperson
34. **STF's $31M lobbying budget** and **$13.1M in "other professional fees"** contain zero mentions of child safety, digital policy, age verification, or app stores in the 990 filing
35. **John R Read** (DCA Senior Policy Advisor) lists "Digital Childhood Alliance" as employer in CO TRACER records — contributed $100 to AG candidate Hetal Doshi (Oct 2025)
36. **Matt Ball received 8% of total fundraising from tech industry employees** — the only 2026 CO senate candidate with contributions from Meta, Pinterest, Instacart, Anthropic, and Google employees; 4 of 8 dual-maxed donors are tech employees
37. **NCOSE Schedule R reveals two-entity evolution** — original NCOSE Action (EIN 86-2458921, c4→c3) replaced by Institute for Public Policy (EIN 88-1180705, c4). All 19 NCOSE↔Institute transaction indicators marked "No" despite same leadership
38. **For Good DAF pathway definitively ruled out** — 59,736 grant recipients across 5 years (~$1.73B) searched; zero matches for DCA, DCI, NCOSE, NCOSEAction, or any related entity
39. **NCOSE lobbying spending tripled** from $78K to $204K concurrent with DCA launch and ASAA legislative push (FY2023→FY2024)
40. **Forge the Future super PAC explicitly lists ASAA-aligned policy priority** — "Empowering parents with oversight of children's online activities across devices and digital environments"
41. **Hilltop Public Solutions bridges Meta's super PAC and DCA operations** — co-leads ATEP ($45M) AND involved in DCA messaging coordination. First firm confirmed in both tracks
42. **Meta super PACs are state-level entities** (not FEC-registered), deliberately scattering filings across state ethics commissions to avoid centralized searchability
43. **Meta's total documented political spending: $70+ million** — $45M ATEP + $20M META California + $5M California Leads, flowing downstream to Forge the Future (TX, R) and Making Our Tomorrow (IL, D)
44. **Casey Stefanski never appears on any NCOSE 990 filing** despite reportedly working there 10 years — not among officers, directors, key employees, or five highest-compensated
45. **Meta's LD-2 filings explicitly list the App Store Accountability Act** (H.R. 3149/S. 1586) as a lobbied bill — first direct on-the-record evidence from Meta's own federal filings connecting its $26.3M lobbying spend to the specific legislation DCA advocates for
46. **Meta simultaneously lobbies FOR ASAA and ON KOSA/COPPA 2.0** — supporting legislation that burdens Apple/Google while opposing/amending legislation that burdens Meta. Both appear in the same LD-2 filing.
47. **LD-2 narrative mirrors DCA messaging** — "youth safety and federal parental approval" framing in Meta's federal filings matches DCA's "parental approval" and "child protection" advocacy language

### Structurally Possible but Unproven

1. Meta funds flow through Arabella network via **non-grant mechanisms**: fiscal sponsorship, consulting fees, or lobbying expenditures (Schedule I pathway ruled out; For Good DAF pathway now also ruled out)
2. DCA operates under **NCOSEAction** (EIN 88-1180705) — personnel chain is direct (van der Watt→Hawkins→Stefanski), but NCOSE reports zero transactions with its c4 and DCA doesn't appear on Schedule R
3. NVF's $36.7M in lobbying expenditures support age verification advocacy
4. Jake Levine's contribution to Matt Ball was coordinated by Meta's government affairs team rather than purely personal
5. ~~NCOSE has an undiscovered 501(c)(4) affiliate~~ — **CONFIRMED: EIN 88-1180705, plus earlier EIN 86-2458921**
6. STF's $31M lobbying fees and $13.1M professional fees could include age verification advocacy, but aggregate reporting prevents confirmation
7. Angela Paxton (TX ASAA sponsor) was among the unnamed Texas state senators supported by Forge the Future
8. NCOSE's lobbying spend tripling is causally related to DCA/ASAA activity (timing is concurrent but program descriptions don't mention ASAA)
9. DCA's NFG donation page is purely cosmetic — actual funding comes from Meta directly, not small-dollar DAF donations

### Not Investigated / Pending

1. **FOIA responses** due 2026-03-13 (CO SOS) and 2026-03-14 (CO AG, LA Ethics)
4. ~~DCA incorporation records~~ — COMPLETED
5. **CalAccess** individual lobbyist registrations for Meta in California
6. ~~Windward Fund and Hopewell Fund~~ — COMPLETED
7. ~~North Fund Schedule I~~ — COMPLETED
8. ~~OpenCorporates cross-reference~~ — COMPLETED
9. ~~Meta federal lobbying LD-2 forms~~ — COMPLETED: ASAA explicitly listed as lobbied bill; "youth safety and federal parental approval" in narrative
10. ~~FollowTheMoney.org multi-state search~~ — COMPLETED
11. ~~Meta's ATEP super PAC~~ — COMPLETED: State-level PACs, Forge the Future ASAA-aligned, Hilltop bridges PAC+DCA
12. **DC DLCP / Delaware ICIS** interactive searches for DCA incorporation (requires browser access)
13. **Meta's semi-annual state contributions PDF** — direct corporate contributions to state candidates
14. **Texas Ethics Commission** — Forge the Future full expenditure recipients (would reveal unnamed state senators including potential Paxton connection)
15. **IRS Form 8872** — ATEP political organization disclosure filings
16. **NCOSEAction (EIN 88-1180705) first 990 filing** — when available, would reveal any DCA-related spending
17. **NCOSE Action (EIN 86-2458921)** — original c4, reclassified to c3, then dropped from Schedule R. What happened to this entity?

---

## VIII. THE STRATEGIC LOGIC

### Why Meta Funds ASAA

The App Store Accountability Act requires **app stores** (Apple, Google) to verify user ages before downloads. It does **not** require social media platforms to verify ages within their own apps. If ASAA becomes national law:

1. Apple and Google bear the compliance cost of age verification infrastructure
2. Meta's apps (Facebook, Instagram, WhatsApp, Threads) face no direct age-check mandate
3. Parents' regulatory complaints shift from "Meta let my child access harmful content" to "Apple/Google failed to verify my child's age"
4. Meta can claim it supports child safety while its competitors absorb the regulatory burden

### Why Use Dark Money

Meta's direct lobbying is publicly disclosed and widely criticized. By funding DCA through opaque channels:

1. ASAA appears to have **grassroots conservative support** rather than Big Tech backing
2. The conservative coalition (Heritage Foundation, Moms for Liberty, NCOSE) provides **bipartisan credibility**
3. A **"concerned Utah mom"** (McKay) provides the human face
4. A **former DOJ antitrust prosecutor** (Read) provides legal credibility and insider knowledge
5. As a 501(c)(4), DCA has **no legal obligation** to disclose Meta's funding
6. The Arabella network structure, if used, adds a further **layer of untraceable pass-through funding**

### Why the Eichberg Connection Matters

Adam Eichberg's dual role is not necessarily illegal, but it creates a structural conflict of interest:
- As Headwaters co-founder, he lobbies on behalf of Meta in Colorado
- As NVF Board Chair, he governs an organization that transfers $121M+ annually to a 501(c)(4) with complete donor opacity
- The same person who receives Meta's lobbying payments oversees the governance of the nation's largest dark money pass-through entity
- Whether this overlap is coincidental or instrumental is the central unresolved question

---

## IX. SOURCES INDEX

### IRS / Nonprofit Data
- NVF Schedule I Analysis: `data/processed/nvf_schedule_i_analysis.md`
- STF Schedule I Analysis: `data/processed/stf_schedule_i_analysis.md`
- North Fund Schedule I Analysis: `data/processed/north_fund_schedule_i_analysis.md`
- Windward & Hopewell Schedule I Analysis: `data/processed/windward_hopewell_schedule_i_analysis.md`
- Arabella 990 Findings: `data/processed/arabella_990_findings.md`
- NVF 990 Findings: `data/processed/nvf_990_findings.md`

### Lobbying Disclosure
- Headwaters Expenditures: `data/processed/headwaters_expenditure_findings.md`
- Koch Lobbyist: `data/processed/koch_lobbyist_findings.md`
- California Lobbying: `data/processed/california_lobbying_findings.md`
- Meta National Lobbying: `data/processed/meta_national_lobbying_findings.md`

### DCA Investigation
- DCA Team & Formation: `data/processed/dca_team_and_formation_findings.md`
- DCA Wayback Analysis: `data/processed/dca_wayback_findings.md`
- DCA DNS/WHOIS: `data/processed/dca_dns_whois_findings.md`
- DCA Corporate Registry: `data/processed/dca_corporate_registry_findings.md`

### Campaign Contributions
- CO TRACER Findings: `data/processed/co_tracer_contribution_findings.md`
- FollowTheMoney Multi-State: `data/processed/followthemoney_multistate_findings.md`

### Corporate Registry / IRS BMF
- DCA/DCI Incorporation Analysis: `data/processed/dca_incorporation_updated.md`

### Cross-Reference Analysis
- Anomaly & Corruption Pattern Analysis: `data/processed/cross_reference_anomaly_analysis.md`
- Five Threads Investigation: `data/processed/five_threads_investigation.md`
- NCOSE / For Good / FEC Investigation: `data/processed/ncose_forgood_fec_investigation.md`

### Federal Lobbying Disclosure
- Meta LD-2 Lobbying Disclosures: `data/processed/meta_ld2_lobbying_disclosures.md`

### Legislative Analysis
- Utah/Texas Findings: `data/processed/utah_texas_legislative_findings.md`
- LA HB-570 Corrected: `data/processed/la_hb570_corrected.md`
- CO Witness Findings: `data/processed/co_ga_witness_findings.md`

### External Sources
- OpenSecrets Meta Profile: https://www.opensecrets.org/federal-lobbying/clients/summary?id=D000033563
- ProPublica NVF: https://projects.propublica.org/nonprofits/organizations/205806345
- ProPublica Sixteen Thirty: https://projects.propublica.org/nonprofits/organizations/264486735
- F Minus (Pelican State): https://fminus.org/clients/pelican-state-partners-llc/
- LA Ethics (Koch): https://eap.ethics.la.gov/Lobbyist/upload/349/
- CO SODA API: https://data.colorado.gov/resource/dxfk-9ifj.json
- Deseret News Op-Ed: https://www.deseret.com/opinion/2025/12/07/child-safety-bill-backed-by-meta/
- ACT | The App Association: https://actonline.org/2025/05/23/into-the-metaverse-the-money-and-motivations-behind-metas-app-store-gambit/
- Bloomberg Government: https://news.bgov.com/bloomberg-government-news/meta-on-path-for-record-year-spend-on-california-tech-lobbying
- Dome Politics: https://domepolitics.com/2026/02/meta-breaks-all-time-lobbying-record-as-georgia-lawmakers-consider-online-safety-bills/
- CO TRACER Bulk Data: https://tracer.sos.colorado.gov/PublicSite/DataDownload.aspx
- Sixteen Thirty Fund 990: https://www.sixteenthirtyfund.org/wp-content/uploads/2025/11/Sixteen-Thirty-Fund-2024-Public-Disclosure-Copy-rG58c3r55H5J50YadU6i.pdf
