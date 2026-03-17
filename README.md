_______________________________________________________________________________
Website: https://tboteproject.com
Most Recent Repository: https://tboteproject.com/git/hekate/attestation-findings
_______________________________________________________________________________
Help keep the server running!
Monero: 451CjP6mgu12yvmDLxLduYYw5Py3Nnb91RwoRYCnhMwhGKM5hxYSaAWapq7CdRQz3qRJbUqqrnYBzW7L4aUt7nhbAYGmLSX

Thank you for your support.

# Meta Platforms: Lobbying, Dark Money, and the App Store Accountability Act

An open-source intelligence investigation into how Meta Platforms built a multi-channel influence operation to pass age verification laws that shift regulatory burden from social media platforms onto Apple and Google's app stores.

Every finding in this repository is sourced from public records: IRS 990 filings, Senate LD-2 lobbying disclosures, state lobbying registrations, campaign finance databases, corporate registries, WHOIS/DNS records, Wayback Machine archives, and investigative journalism.

**Status:** Active investigation. 50 proven findings, 9 structurally possible but unproven hypotheses, multiple pending FOIA responses, and an active OSINT surveillance counter-investigation.

**Research period:** 2026-03-11 to present

## The Investigation at a Glance

Meta spent a record $26.3 million on federal lobbying in 2025, deployed 86+ lobbyists across 45 states, and covertly funded a "grassroots" child safety group called the Digital Childhood Alliance (DCA) to advocate for the App Store Accountability Act (ASAA). The ASAA requires app stores to verify user ages before downloads but imposes no requirements on social media platforms. If it becomes law, Apple and Google absorb the compliance cost while Meta's apps face zero new mandates.

**2026-03-16 UPDATE:** DCA's EIN has been identified: 33-2669790. "Digital Childhood Alliance Inc," Delaware, officer Melissa McKay, same address as sister org DCI (213 N Market St PMB 1039, Wilmington DE). Tax year 2024 gross receipts: under $25,000 (990-N e-Postcard filer). An organization coordinating a 20+ state legislative campaign with confirmed Meta funding reports less than $25K in total receipts. The real money never touches this EIN.

This investigation traced funding flows across five confirmed channels, analyzed $2.0 billion in dark money grants, searched 59,736 DAF recipients, parsed LD-2 filings, mapped campaign contributions across four states and reveals Heritage Foundation's role as an institutional credibility launderer for the DCA coalition.

## Key Visuals

### Meta's Lobbying Expenditures

![Meta lobbying spend chart showing record $26.3M in 2025](output/reports/chart1_meta_lobbying_spend.png)

Meta's federal lobbying spending jumped from $19M (2022-2023) to $24M (2024) to $26.3M (2025) as ASAA bills were introduced in roughly 20 states. In Louisiana alone, 12 lobbyists were deployed for a single bill that passed 99-0.

### $2.0 Billion in Arabella Network Grants: Zero to Child Safety

![Chart showing zero child safety grants across $2.0B in Arabella network grants](output/reports/chart2_arabella_grants_zero.png)

Across all five Arabella Advisors entities (New Venture Fund, Sixteen Thirty Fund, North Fund, Windward Fund, Hopewell Fund), 4,433 grants totaling approximately $2.0 billion were analyzed. Not a single dollar went to any child safety, age verification, or tech policy organization. The Schedule I grant pathway through the Arabella network is definitively ruled out.

### Meta's Multi-Channel Influence Network

![Network diagram mapping Meta's five influence channels](output/reports/chart3_influence_network.png)

Five confirmed channels connect Meta's spending to ASAA advocacy: direct federal lobbying ($26.3M), state lobbyist networks (45 states), the Digital Childhood Alliance (astroturf 501(c)(4)), super PACs ($70M+), and state legislative campaigns (4 laws passed). A sixth channel through the Arabella dark money network is structurally possible but unproven.

## Interactive Reports

Self-contained HTML documents with detailed investigation views:

- **[Full Investigation Documentation](output/reports/meta_investigation_documentation.html)** -- complete OSINT investigation report with all five channels, evidence tables, and source citations.
- **[Funding Network Timeline](output/timeline/funding_network_timeline.html)** -- chronological development of Meta's lobbying infrastructure, DCA's formation, and ASAA legislative progress across states.
- **[Research Timeline](output/timeline/meta_timeline.html)** -- tracks the investigation itself, showing when each finding was established and how threads connected.

Clone the repo and open in a browser, or use Forgejo's raw file view.

## Repository Structure

```
data/
  processed/            30+ research findings and analysis documents
    cross_reference_anomaly_analysis.md    8 anomaly patterns across all channels
    five_threads_investigation.md          5 parallel investigation threads
    ncose_forgood_fec_investigation.md     NCOSE, For Good DAF, Meta super PAC analysis
    icmec_model_legislation_investigation.md  ICMEC vs DCA model legislation comparison
    heritage_foundation_connections.md     Heritage Foundation credibility laundering
    other_tech_companies_asaa.md           Snap, X, Pinterest, Roblox ASAA positions
    connectsafely_990_analysis.md          ConnectSafely conflicts of interest
    tracking.md                            Master entity/finding tracker (75 entities, 11 bills)
    all_findings.json                      Structured database of all 248 findings
    ...                                    24 additional analysis files
  raw/
    osint_990/          Raw IRS 990 data extracts
    connectsafely_990/  ConnectSafely XML/PDF 990 filings (2015-2024)
  disclosures/          Colorado lobbyist monthly disclosure PDFs

output/
  reports/              Summary reports, charts, HTML documentation
  timeline/             Interactive timeline visualizations
  briefs/               Policy briefs and public comments

```

## The Five Confirmed Channels

### 1. Direct Lobbying

Meta retained 40+ lobbying firms and 87 federal lobbyists in 2025 (85% with prior government service). Meta's own LD-2 filings with the Senate explicitly list H.R. 3149/S. 1586, the App Store Accountability Act, as a lobbied bill. The filing narrative includes "protecting children, bullying prevention and online safety; youth safety and federal parental approval; youth restrictions on social media."

At the state level, confirmed operations include $338,500 to Headwaters Strategies (Colorado), $324,992+ across 9 firms and 12 lobbyists in Louisiana, and $1,036,728 in direct California lobbying (Q1-Q3 2025 alone). A Meta lobbyist brought the legislative language for Louisiana HB-570 directly to the bill's sponsor, Rep. Kim Carver, who confirmed this publicly.

### 2. Digital Childhood Alliance (Astroturf Advocacy)

DCA is a 501(c)(4) advocacy group that Meta covertly funds. Bloomberg exposed the funding relationship in July 2025. Under oath at a Louisiana Senate committee hearing, Executive Director Casey Stefanski admitted receiving tech company funding but refused to name donors.

**EIN 33-2669790 confirmed (2026-03-16).** "Digital Childhood Alliance Inc," Delaware, 213 N Market Street PMB 1039, Wilmington DE 19801. Officer: Melissa McKay. Tax year 2024 gross receipts: under $25,000. 990-N e-Postcard filer (zero financial disclosure). Same address as sister org DCI (EIN 39-3684798). Not on ProPublica, GuideStar, or Charity Navigator.

The under-$25K gross receipts cannot be reconciled with an organization coordinating a 20+ state legislative campaign with confirmed Meta funding, a paid executive director, a registered lobbyist (John Read), commissioned polling, and multi-state testimony programs. The real operating budget does not flow through this EIN. Donations process through the For Good DAF (formerly Network for Good) as "Project 258136." The most probable fiscal sponsor is NCOSEAction/Institute for Public Policy (EIN 88-1180705), NCOSE's confirmed 501(c)(4) affiliate with the same leadership.

DCA's domain was registered December 18, 2024. The website was live and fully formed the next day. Every blog post and testimony targets Apple and Google. Meta is never mentioned or criticized.

**Dual-entity structure:** DCA (c4, lobbying, admits tech funding) and DCI (c3, education, claims no tech funding) share the same Delaware address and founder (Melissa McKay). The lobbying vehicle was created six months before the research arm, reversing standard nonprofit formation order.

### 3. Super PACs ($70M+)

Meta committed over $70 million to four state-level super PACs: ATEP ($45M, bipartisan, co-led by Hilltop Public Solutions), META California ($20M), California Leads ($5M), and Forge the Future (Texas, Republican-aligned). Forge the Future's stated policy priority is "empowering parents with oversight of children's online activities," which mirrors ASAA language exactly.

Hilltop Public Solutions co-leads the $45M ATEP super PAC and is also involved in DCA's messaging coordination, making it the first firm confirmed in both Meta's PAC operation and the astroturf advocacy track.

All super PACs are registered at the state level rather than with the FEC, scattering disclosure filings across individual state ethics commissions instead of a single searchable federal database.

### 4. The Arabella Network Connection

Meta's Colorado lobbyist Adam Eichberg simultaneously serves as Board Chair of the New Venture Fund, the flagship 501(c)(3) of the Arabella Advisors network. NVF transfers $121.3 million annually to the Sixteen Thirty Fund, a 501(c)(4) with no donor disclosure requirements.

The Arabella network operates four entities from 1828 L Street NW, Washington DC (suites 300-A through 300-D) with combined annual revenue exceeding $1.3 billion. All five entities' grant recipients were analyzed (4,433 grants, approximately $2.0 billion). Zero dollars went to any child safety organization, definitively ruling out the Schedule I grant pathway.

If Meta money flows through the Arabella network to DCA, it travels via fiscal sponsorship, consulting fees, or lobbying expenditures, which are more opaque than grant disclosures.

### 5. State Legislative Campaigns

ASAA has been signed into law in four states:
- **Utah SB-142** (signed March 26, 2025, first in nation)
- **Texas SB 2420** (signed May 2025, paused by federal judge December 2025)
- **Louisiana HB-570** (signed June 30, 2025, effective July 1, 2026)
- **Alabama HB 161** (passed unanimously 2026)

Roughly 17 additional states have introduced or are considering ASAA bills, including Kansas, South Carolina, Ohio, Georgia, and Florida. The federal version was introduced in May 2025 by Rep. John James (R-MI) and Sen. Mike Lee (R-UT).

### 6. Other ASAA Supporters

Meta is not the only company backing ASAA. Snap and X issued joint statements with Meta supporting ASAA bills in Utah, Texas, and South Dakota. Pinterest's CEO publicly endorsed the federal ASAA in December 2025. Snap's LD-2 filings confirm lobbying on H.R. 3149/S. 1586. Meta remains the only company confirmed funding DCA and the only company documented drafting bill language. Every confirmed ASAA supporter is a social media platform that benefits from shifting age verification to the app store layer. Every confirmed opponent operates an app store that would bear the compliance burden.

### 7. ICMEC: The Competing Model

Two distinct model legislation frameworks circulate at the state level, often conflated. ICMEC's Digital Age Assurance Act (DAAA) targets device/OS-level verification and places the burden on Apple, Google, and Microsoft as device manufacturers. DCA's App Store Accountability Act (ASAA) targets app store-level verification and places the burden on app stores specifically. Meta donates to ICMEC but funds DCA. Both approaches shift regulation away from social media platforms. ICMEC personnel testify for DAAA-style bills; DCA personnel testify for ASAA-style bills.

### 8. Heritage Foundation as Credibility Launderer

Heritage Foundation awarded Innovation Prizes to three of six named DCA coalition members: NCOSE, Institute for Family Studies ($50K), and Ethics and Public Policy Center ($50K). Annie Chestnut Tutor served as legislative assistant to Sen. Mike Lee (tech/telecom portfolio), then Heritage policy analyst, and appeared on the DCA website from its first day (December 19, 2024). Heritage and Moms for Liberty (both DCA coalition members) underwent a leadership merger when Tiffany Justice (M4L co-founder) became Heritage Action EVP in July 2025. Heritage provides conservative institutional credibility for a coalition whose funding traces back to Meta, forming a closed policy loop: Meta funds DCA, DCA's core members are Heritage-funded, Heritage staffs the advocacy.

## DCA EIN Discovery (2026-03-16)

EIN 33-2669790 was located via eintaxid.com. Prior investigation searches found DCA absent from the IRS Business Master File (all 4 regional extracts), ProPublica, GuideStar, Candid, Charity Navigator, and state corporate registries in CO, DC, DE, and VA. The EIN may have been assigned after those searches, or 990-N filers may lag in BMF indexing.

**The funding flow problem:**

```
Meta ($26.3M lobbying budget, 2025)
  |
  +-- Direct lobbying ($338K CO, $325K+ LA, etc.)
  |
  +-- DCA (EIN 33-2669790) <-- reports <$25K  <-- WHERE IS THE REST?
  |     Melissa McKay (officer)
  |     Casey Stefanski (exec director)
  |
  +-- For Good DAF (EIN 68-0480736) --> DCA "Project 258136"
  |     $204M annual pass-through volume (DCA invisible in this)
  |     59,736 grant recipients searched: zero matches
  |
  +-- NCOSEAction (EIN 88-1180705) <-- probable fiscal sponsor
  |     501(c)(4), same leadership as NCOSE
  |     Dawn Hawkins chairs DCA + runs NCOSE
  |     IRS ruling May 2025 (timing matches DCA launch)
  |     Zero reported transactions with parent NCOSE
  |
  +-- Hilltop Public Solutions / DCI Group (consulting firms)
        Coordinate messaging + grassroots campaigns
        Hilltop also co-leads $45M ATEP super PAC
```

Three EINs in this investigation share the same Delaware PMB address (213 N Market St PMB 1039, Wilmington):
- DCA: 33-2669790 (c4, <$25K, 990-N)
- DCI: 39-3684798 (c3, IRS ruling Nov 2025)
- Both: Officer Melissa McKay

## Proven Findings (50)

Each finding below is documented with sources in the corresponding analysis file.

### Direct Lobbying (1-19)

1. Meta funds DCA, confirmed by Bloomberg reporters and partially admitted by Stefanski under oath at the Louisiana Senate Commerce Committee hearing (April 2025).
2. Meta deployed 86+ lobbyists across 45 states for ASAA and related campaigns.
3. Meta spent $26.3 million on federal lobbying in 2025, an all-time record exceeding Lockheed Martin and Boeing.
4. Meta paid Headwaters Strategies $338,500 for Colorado lobbying between 2019 and 2026.
5. Adam Eichberg simultaneously co-founded Meta's Colorado lobbying firm (Headwaters Strategies) and chairs the New Venture Fund board.
6. NVF transfers $121.3 million to the Sixteen Thirty Fund (c4) annually.
7. NVF does not directly fund any child safety or tech policy organizations via Schedule I grants.
8. DCA and DCI share infrastructure: same registrar (GoDaddy), CDN (Cloudflare), email (Microsoft 365), and marketing platform (Elastic Email).
9. Pelican State Partners represents Meta as a lobbying client in Louisiana.
10. DCA leadership comes from NCOSE: three of four senior staff have NCOSE connections (Stefanski, Hawkins, McKay).
11. DCA's John Read spent 30 years at DOJ Antitrust investigating app stores and Big Tech.
12. ASAA signed into law in four states: Utah (SB-142, March 2025), Louisiana (HB-570, June 2025), Texas (SB 2420, May 2025, paused by judge December 2025), Alabama (HB 161, 2026).
13. The Sixteen Thirty Fund does not fund any child safety or tech policy organizations via Schedule I grants.
14. All five Arabella entities analyzed: 4,433 grants (approximately $2.0 billion) with zero dollars going to child safety or tech policy organizations.
15. A Meta employee (Jake Levine, Product Manager) contributed $1,175 to ASAA sponsor Matt Ball's campaign apparatus on June 2, 2025.
16. A Google Policy Manager (Kyle Gardner) also contributed $450 to Matt Ball. Multiple tech company employees from ASAA-affected companies targeted the same ASAA bill sponsor.
17. Eichberg and Coyne (Headwaters principals) did not contribute to ASAA bill sponsors Ball or Paschal despite $20,000+ combined political giving.
18. No direct Meta PAC contributions to any ASAA sponsor across Utah, Louisiana, Texas, or Colorado.
19. Todd Weiler (Utah SB-142 sponsor) does not accept corporate contributions and has not discussed ASAA directly with Meta. DCA served as the policy intermediary.

### DCA Investigation (20-24)

20. DCA EIN 33-2669790 confirmed (2026-03-16). "Digital Childhood Alliance Inc," Delaware, 213 N Market St PMB 1039, Wilmington DE. Officer: Melissa McKay. Tax year 2024 gross receipts: under $25,000. 990-N e-Postcard filer. Not on ProPublica, GuideStar, or Charity Navigator.
21. DCI confirmed in IRS BMF with EIN 39-3684798, Delaware incorporation at same address, IRS ruling November 2025.
22. DCA and DCI share identical Delaware address and same officer (Melissa McKay), confirming dual-entity structure under single control.
23. DCA reports under $25K despite confirmed Meta funding, proving primary funding flows through undisclosed channels (NCOSEAction, STF, or direct Meta payments).
24. DCA's website deployed less than 24 hours after domain registration: fully functional advocacy site with professional design, statistics, and Heritage/NCOSE testimonials.

### Legislative Process (25-33)

25. 77-day pipeline from DCA domain registration (December 18, 2024) to Utah SB-142 signing (March 5, 2025). Site pre-loaded with ASAA talking points before any bill had passed.
26. Meta deployed 12 lobbyists for Louisiana HB-570, which passed 99-0. Disproportionate deployment for text-control and amendment-blocking, not vote persuasion.
27. Three California tech policy employees from Meta, Google, and Pinterest contributed to Matt Ball within 90 days. All from ASAA-affected companies, all out-of-state, targeting a newly-appointed senator.
28. Pelican State Partners represents both Meta and Roblox in Louisiana. Both ASAA beneficiaries, enabling "broad industry support" framing.
29. DCA's coalition count inflated from 50+ to 140+ with only six organizations ever publicly named. No member list published on the website.
30. A Meta lobbyist drafted HB-570's legislative language, confirmed by sponsor Rep. Kim Carver.
31. Sen. Jay Morris's amendment expanded HB-570 to include app developers alongside app stores, leading to a conference committee compromise.
32. Nicole Lopez (Meta Director of Global Litigation Strategy for Youth) testified in both Louisiana and South Dakota for ASAA bills, serving as Meta's national ASAA spokesperson.
33. Meta's LD-2 filings explicitly list the App Store Accountability Act (H.R. 3149/S. 1586) as a lobbied bill.

### Fiscal Sponsorship and Dark Money (34-44)

34. NCOSE has a confirmed 501(c)(4) affiliate: NCOSEAction / Institute for Public Policy (EIN 88-1180705), IRS ruling May 2025, same address and leadership as NCOSE.
35. Network for Good is a Donor Advised Fund, not a payment processor. DCA classified as "Project" (ID 258136) in the system. For Good explicitly limits grants to 501(c)(3) organizations.
36. NCOSE Schedule R reveals a two-entity evolution: the original NCOSE Action (EIN 86-2458921, c4 reclassified to c3) was replaced by the Institute for Public Policy (EIN 88-1180705, c4). All 19 NCOSE-to-Institute transaction indicators are marked "No" despite shared leadership.
37. For Good DAF pathway definitively ruled out: 59,736 grant recipients across five years (approximately $1.73 billion) searched with zero matches for DCA, DCI, NCOSE, NCOSEAction, or any related entity.
38. The Sixteen Thirty Fund's $31 million lobbying budget and $13.1 million in professional fees contain zero mentions of child safety, digital policy, age verification, or app stores.
39. NCOSE lobbying spending tripled from $78,000 to $204,000 concurrent with DCA launch and the ASAA legislative push (FY2023 to FY2024).
40. Casey Stefanski never appears on any NCOSE 990 filing despite reportedly working there ten years. Not among officers, directors, key employees, or five highest-compensated.
41. Forge the Future super PAC explicitly lists an ASAA-aligned policy priority.
42. Hilltop Public Solutions bridges Meta's super PAC and DCA operations. Co-leads ATEP ($45M) and involved in DCA messaging coordination. First firm confirmed in both tracks.
43. Meta super PACs are state-level entities (not FEC-registered), scattering filings across state ethics commissions to avoid centralized searchability.
44. Meta's total documented political spending exceeds $70 million across four state-level super PACs.

### Cross-Reference and Coalition (45-50)

45. Meta simultaneously lobbies FOR ASAA and ON KOSA/COPPA 2.0, supporting legislation that burdens Apple and Google while opposing or amending legislation that would regulate Meta directly.
46. LD-2 narrative mirrors DCA messaging: "youth safety and federal parental approval" framing in Meta's federal filings matches DCA's "parental approval" and "child protection" advocacy language.
47. John R. Read (DCA Senior Policy Advisor) lists "Digital Childhood Alliance" as his employer in Colorado TRACER records.
48. Matt Ball received 8% of total fundraising from tech industry employees. Only 2026 Colorado senate candidate with contributions from Meta, Pinterest, Instacart, Anthropic, and Google employees.
49. Heritage Foundation awarded Innovation Prizes to three of six named DCA coalition members. Heritage staffs DCA advocacy through the Mike Lee to Heritage to DCA pipeline.
50. ConnectSafely CEO Larry Magid serves on Meta's Safety Advisory Council while running a nominally independent child safety organization. Revenue is 89.7% contributions, executive compensation consumes 57.5% of expenses, and Magid has publicly opposed certain child safety bills.

## Structurally Possible but Unproven

1. Meta funds flow through the Arabella network via non-grant mechanisms (fiscal sponsorship, consulting fees, lobbying expenditures). The Schedule I and For Good DAF pathways are both ruled out.
2. DCA operates under NCOSEAction (EIN 88-1180705) as fiscal sponsor despite having its own EIN (33-2669790). DCA's under-$25K gross receipts mean operational funding still flows through another entity. The personnel chain is direct (van der Watt to Hawkins to Stefanski), but NCOSE reports zero transactions with its c4 affiliate.
3. NVF's $36.7 million in lobbying expenditures support age verification advocacy.
4. Jake Levine's contribution to Matt Ball was coordinated by Meta's government affairs team.
5. STF's $31M lobbying fees and $13.1M professional fees include age verification advocacy, but aggregate reporting prevents confirmation.
6. Angela Paxton (Texas ASAA sponsor) was among the unnamed state senators supported by Forge the Future.
7. NCOSE's lobbying spend tripling is causally related to DCA/ASAA activity.
8. DCA's For Good donation page is cosmetic. Actual funding comes directly from Meta, not small-dollar DAF donations.

## External Sources

### Federal Lobbying and Legislative Records

| Source | URL |
|--------|-----|
| OpenSecrets Meta Profile | https://www.opensecrets.org/federal-lobbying/clients/summary?id=D000033563 |
| OpenSecrets Meta Lobbyists | https://www.opensecrets.org/federal-lobbying/clients/lobbyists?cycle=2025&id=D000033563 |
| Senate LDA Filing (Q1 2025) | https://lda.senate.gov/filings/public/filing/b73445ed-15e5-42e7-a1e8-aeb224755267/print/ |
| Congress.gov H.R. 3149 | https://www.congress.gov/bill/119th-congress/house-bill/3149 |
| Congress.gov S. 1586 | https://www.congress.gov/bill/119th-congress/senate-bill/1586 |

### IRS Nonprofit Filings

| Source | URL |
|--------|-----|
| DCA EIN 33-2669790 | https://eintaxid.com/company/332669790-digital-childhood-alliance-inc/ |
| ProPublica NVF | https://projects.propublica.org/nonprofits/organizations/205806345 |
| ProPublica Sixteen Thirty Fund | https://projects.propublica.org/nonprofits/organizations/264486735 |
| ProPublica NCOSEAction | https://projects.propublica.org/nonprofits/organizations/881180705 |
| ProPublica ConnectSafely | https://projects.propublica.org/nonprofits/organizations/473168168 |
| NVF 2023 Form 990 | https://newventurefund.org/wp-content/uploads/2024/11/2023-New-Venture-Fund-Form-990-Public-Disclosure-Copy.pdf |

### State Lobbying and Campaign Finance

| Source | URL |
|--------|-----|
| Colorado SODA API | https://data.colorado.gov/resource/dxfk-9ifj.json |
| Colorado TRACER | https://tracer.sos.colorado.gov/PublicSite/DataDownload.aspx |
| F Minus (Pelican State Partners) | https://fminus.org/clients/pelican-state-partners-llc/ |
| FollowTheMoney (Meta) | https://www.followthemoney.org/entity-details?eid=54466150 |

### State Legislative Records

| Source | URL |
|--------|-----|
| Louisiana HB-570 | https://www.legis.la.gov/Legis/BillInfo.aspx?i=248616 |
| Utah SB-142 | https://le.utah.gov/~2025/bills/static/SB0142.html |
| Colorado SB26-051 | https://leg.colorado.gov/bills/SB26-051 |

### Organizational Profiles

| Source | URL |
|--------|-----|
| DCA Website | https://www.digitalchildhoodalliance.org/ |
| DCA Stefanski Bio | https://www.digitalchildhoodalliance.org/meet-digital-childhood-alliance-executive-director-casey-stefanski/ |
| NVF Board (Eichberg) | https://newventurefund.org/who-we-are/board-of-directors/adam-eichberg-chair-of-the-board/ |
| Headwaters Strategies | https://headwatersstrategies.com/ |
| InfluenceWatch (Eichberg) | https://www.influencewatch.org/person/adam-eichberg/ |
| ICMEC Model DAAA | https://cdn.icmec.org/wp-content/uploads/2024/10/Digital-Age-Assurance-Act-2024.pdf |
| ICMEC Supporters | https://www.icmec.org/our-supporters/ |

### Investigative Reporting

| Source | URL |
|--------|-----|
| Bloomberg/Insurance Journal (Meta+DCA) | https://www.insurancejournal.com/news/national/2025/07/25/833246.htm |
| Deseret News (Meta Manipulation) | https://www.deseret.com/opinion/2025/12/07/child-safety-bill-backed-by-meta/ |
| The Center Square (Stefanski) | https://www.thecentersquare.com/louisiana/article_e97200f8-13d0-4b1f-90a9-e9a7093d329f.html |
| Pluribus News (ASAA) | https://pluribusnews.com/news-and-events/meta-lobbies-for-app-store-age-verification-laws/ |
| Jessica Reed Kraus (Mom Groups) | https://jessicareedkraus.substack.com/p/how-meta-funded-mom-groups-teach |
| Kansas Reflector (DCA) | https://kansasreflector.com/2026/03/05/tech-companies-vie-for-influence-over-kansas-app-store-age-verification-legislation/ |
| Tech Transparency Project | https://www.techtransparencyproject.org/articles/inside-metas-spin-machine-on-kids-and-social-media |

## Analysis Files

### Cross-Reference and Anomaly Analysis
- [Cross-Reference Anomaly Analysis](data/processed/cross_reference_anomaly_analysis.md) -- 8 anomaly patterns across all investigation channels
- [Five Threads Investigation](data/processed/five_threads_investigation.md) -- NCOSE c4, For Good DAF, STF expenses, LA HB-570, Ball contributions
- [NCOSE, For Good, and FEC Investigation](data/processed/ncose_forgood_fec_investigation.md) -- Schedule R evolution, DAF dead end, Meta super PAC architecture

### DCA and Coalition Investigation
- [DCA Team and Formation](data/processed/dca_team_and_formation_findings.md)
- [DCA Wayback Analysis](data/processed/dca_wayback_findings.md)
- [DCA DNS/WHOIS](data/processed/dca_dns_whois_findings.md)
- [DCA Incorporation Updated](data/processed/dca_incorporation_updated.md)
- [Heritage Foundation Connections](data/processed/heritage_foundation_connections.md) -- institutional credibility laundering
- [Other Tech Companies ASAA](data/processed/other_tech_companies_asaa.md) -- Snap, X, Pinterest, Roblox positions

### IRS and Nonprofit Data
- [NVF Schedule I Analysis](data/processed/nvf_schedule_i_analysis.md)
- [STF Schedule I Analysis](data/processed/stf_schedule_i_analysis.md)
- [North Fund Schedule I Analysis](data/processed/north_fund_schedule_i_analysis.md)
- [Windward and Hopewell Schedule I](data/processed/windward_hopewell_schedule_i_analysis.md)
- [ConnectSafely 990 Analysis](data/processed/connectsafely_990_analysis.md) -- conflicts of interest
- [ConnectSafely UK Grant](data/processed/connectsafely_uk_grant_investigation.md)

### Lobbying Disclosure
- [Meta National Lobbying](data/processed/meta_national_lobbying_findings.md)
- [Meta LD-2 Disclosures](data/processed/meta_ld2_lobbying_disclosures.md)
- [Headwaters Expenditures](data/processed/headwaters_expenditure_findings.md)
- [California Lobbying](data/processed/california_lobbying_findings.md)
- [Forge the Future TX Expenditures](data/processed/forge_the_future_tx_expenditures.md)

### Legislative Analysis
- [ICMEC Model Legislation](data/processed/icmec_model_legislation_investigation.md) -- DAAA vs ASAA comparison
- [Global Coordination Research](data/processed/global_coordination_research.md) -- international age verification comparison
- [Utah and Texas Findings](data/processed/utah_texas_legislative_findings.md)
- [Louisiana HB-570](data/processed/la_hb570_corrected.md)
- [Colorado GA Witness Findings](data/processed/co_ga_witness_findings.md)

### Campaign Contributions
- [Colorado TRACER Findings](data/processed/co_tracer_contribution_findings.md)
- [Matt Ball SB26-051 Analysis](adameichfindings/matt-ball-sb26-051.md)
- [FollowTheMoney Multi-State](data/processed/followthemoney_multistate_findings.md)

### Data
- [All Findings (JSON)](data/processed/all_findings.json) -- structured database of 248 findings
- [Master Entity Tracker](data/processed/tracking.md) -- 75 entities, 11 bills, 17 lobbyists

## Methodology and Tools

A human researcher directed all research decisions, selected sources, evaluated findings, and wrote the public-facing posts. Claude Code (Anthropic's CLI tool, running Claude Opus) was used as a research assistant for:

- Bulk data processing: parsing 4,433 IRS Schedule I grant records, 59,736 DAF recipients, 132MB of Colorado TRACER campaign finance data, and IRS Business Master File extracts covering all US tax-exempt organizations
- Cross-referencing findings across 24+ analysis files and identifying patterns spanning multiple research threads
- Web searches against public databases (OpenSecrets, ProPublica, state lobbying portals, WHOIS/DNS, Wayback Machine, eintaxid.com)
- VPN detection and threat analysis pipeline development

Claude Code did not independently choose what to investigate, decide what constitutes a finding, or determine what to publish. Every factual claim cites a primary source (IRS filing, Senate disclosure, state database, legislative record, or published reporting) that can be independently verified. The tool does not change whether Meta's LD-2 filing lists H.R. 3149, whether DCA's EIN reports under $25K, or whether Stefanski admitted tech funding under oath. The records exist or they don't.

Verify any finding using the source URLs and database identifiers provided throughout. Start with the primary records, not with this repository.

## License

OSINT research product. All findings based on public records. Source data cited throughout.
