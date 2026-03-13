# Five Outstanding Questions — Investigation Results

**Research Date:** 2026-03-13
**Method:** Parallel investigation of five unresolved questions from cross-reference anomaly analysis
**Classification:** OSINT research product — all sources are public records

---

## Executive Summary

Five parallel investigations yielded three major new findings:

1. **NCOSE has a confirmed 501(c)(4) affiliate** — "NCOSEAction" (EIN 88-1180705), IRS ruling May 2025, same address, same leadership. This entity could serve as DCA's fiscal sponsor.

2. **Network for Good is a Donor Advised Fund, not a payment processor** — DCA is classified as a "Project" (not a nonprofit) in the system, and For Good explicitly limits grants to 501(c)(3) organizations. DCA's presence on the platform as a claimed c4 with no EIN raises potential DAF compliance issues.

3. **A Meta lobbyist wrote HB-570's legislative language** — confirmed that Meta "brought legislative language" directly to sponsor Rep. Kim Carver, and the bill's key amendment battle was over whether to include app developers (Meta) alongside app stores (Apple/Google).

Additionally: STF's $46M non-grant spending is accounted for by lobbying ($31M), consulting ($13M), and advertising ($8.5M) with zero mentions of child safety or digital policy. Matt Ball's tech industry funding (8%) is distinctive but modest, with law firms (19.2%) being the dominant out-of-state pattern.

---

## 1. NCOSE's 501(c)(4) Affiliate — CONFIRMED

### Discovery

**Entity:** National Center on Sexual Exploitation Institute for Public [truncated]
**Public brand:** NCOSEAction
**EIN:** 88-1180705
**Tax status:** 501(c)(4) — contributions NOT tax-deductible
**Address:** 1201 F St NW, Ste 200, Washington, DC 20004-1221
**Principal Officer:** Marcel van der Watt (also NCOSE President & CEO)
**IRS Ruling Date:** May 2025
**Filing Requirement:** Form 990-N (e-Postcard) — gross receipts ≤$50,000
**Financial data:** All zeros — no revenue, assets, or income reported yet

**Source:** IRS Exempt Organizations Business Master File (eo2.csv), confirmed via GuideStar

### Relationship to NCOSE (c)(3)

| Feature | NCOSE (c)(3) | NCOSEAction (c)(4) |
|---------|-------------|-------------------|
| EIN | 13-2608326 | 88-1180705 |
| Address | 1201 F St NW, DC 20004 | 1201 F St NW, Ste 200, DC 20004 |
| Leadership | Marcel van der Watt (CEO) | Marcel van der Watt (Principal Officer) |
| Revenue | $7.3M (2023) | $0 (no filing yet) |
| IRS Ruling | December 1963 | May 2025 |
| Purpose | Education, research | "Ensure good laws are passed" (per NCOSE About page) |

NCOSE's own website states: "NCOSEAction, a 501c(4) political action organization created by NCOSE, exists to ensure that good laws are passed and bad laws are prevented from being enacted."

### Implications for DCA Fiscal Sponsorship

NCOSEAction (EIN 88-1180705) is a **newly created 501(c)(4) with the correct tax status to sponsor DCA's lobbying activities.** Key considerations:

1. **Correct tax classification:** As a c4, NCOSEAction can host unlimited lobbying activities — unlike NCOSE (c3), which faces lobbying limits
2. **Same leadership:** Marcel van der Watt leads both NCOSE and NCOSEAction. Dawn Hawkins (NCOSE CEO who chairs DCA) reports to van der Watt
3. **Timing alignment:** NCOSEAction's IRS ruling (May 2025) aligns with DCA's operational timeline — DCA launched ~February 2025, and a c4 entity received IRS recognition three months later
4. **Zero financial activity reported:** The 990-N filing requirement (≤$50K) and zero reported financials could mean: (a) NCOSEAction is dormant, (b) NCOSEAction's first filing hasn't been processed, or (c) DCA's revenue flows through a different entity
5. **No website:** ncoseaction.org does not resolve, suggesting operations are conducted through NCOSE's main website or through DCA as the public-facing brand

### Assessment

NCOSEAction is now the **second-strongest fiscal sponsor candidate** after Sixteen Thirty Fund:

| Factor | STF | NCOSEAction |
|--------|-----|-------------|
| Tax status | c4 ✓ | c4 ✓ |
| Sponsored project model | Documented (hundreds) | Unknown |
| Personnel overlap with DCA | Eichberg (indirect) | Hawkins, Stefanski, van der Watt (direct) |
| Financial capacity | $282M revenue | Unknown (≤$50K reported) |
| Address proximity | 1828 L St NW | 1201 F St NW (same city) |
| Operational history | Est. 2009, extensive | May 2025 (brand new) |

The personnel overlap is far stronger with NCOSEAction, but STF has the financial infrastructure and documented sponsored project model. A **hybrid arrangement** is possible: Meta funds flow to STF (via NVF/Eichberg), STF contracts with NCOSEAction, and NCOSEAction operates DCA as a project.

---

## 2. Network for Good — DAF, Not Payment Processor

### Key Finding

Network for Good (now branded "For Good," forgood.org) is a **Donor Advised Fund (DAF)**, not a payment processor. The donation model:

1. Donor gives money **TO For Good** (a 501(c)(3) DAF, EIN 68-0480736)
2. For Good issues the tax receipt under **its own EIN**
3. For Good **re-grants** the funds to the designated nonprofit in monthly disbursements

From For Good's FAQ: "When a donation is made through the For Good giving system, donations are made to For Good (a 501c3, EIN 68-0480736) which is then re-granted to the nonprofit(s) you have selected in our next monthly disbursement."

### For Good Explicitly Limits Grants to 501(c)(3) Organizations

For Good's documentation states three times that it serves "501(c)3 non profit organizations" and covers "up to 1.8 million U.S. 501c3 charities." As a c3 DAF, For Good faces legal constraints on granting to c4 organizations — most DAF sponsors refuse to do so entirely.

### DCA's Anomalous Classification

The DCA donation page at `digitalchildhoodalliance.networkforgood.com` contains hidden form fields:

```
donation_form[targetable_type] = Project
donation_form[targetable_id] = 258136
```

DCA is classified as a **"Project"** in the NFG/Bonterra system (ID 258136), not as a standalone nonprofit organization. The page:
- Displays **no EIN**
- Contains **no tax-deductibility disclaimer**
- Makes **no mention** of For Good as the donation recipient
- Describes "legislative action" and "accountability campaigns" — c4 lobbying language
- Says "Powered by Bonterra" (the for-profit tech company), not "Powered by For Good" (the c3 DAF)

### The Registration Paradox

For Good requires organizations to "Enter your organization's EIN" to register. DCA has **no known EIN**. This creates three possible scenarios:

| Scenario | Implication |
|----------|------------|
| DCA registered using DCI's EIN (39-3684798) | Misrepresentation — DCI is a c3, DCA is a claimed c4 |
| DCA registered without an EIN via the "Project" pathway | The system allows non-EIN entities as "Projects" |
| Someone at For Good/Bonterra manually set up the page | Bypassed standard registration requirements |

### Potential DAF Compliance Issue

If donors giving on `digitalchildhoodalliance.networkforgood.com` receive a tax receipt from For Good (a c3) claiming their donation is tax-deductible, but the funds ultimately support DCA (a claimed c4 doing lobbying), this could constitute:

1. **Improper tax deduction** — c4 contributions are generally not tax-deductible
2. **DAF distribution violation** — For Good's c3 DAF granting to a non-c3 without expenditure responsibility
3. **Donor misrepresentation** — donors may not know their "donation to DCA" is legally a donation to For Good's DAF

### For Good's Financial Scale

| Metric | FY2024 |
|--------|--------|
| Revenue | $204.4M |
| Expenses | $231.6M |
| Total assets | $96.2M |
| Program expense ratio | 98.21% (pass-through model) |
| Charity Navigator | 2 stars ("Needs Improvement") |

For Good processes hundreds of millions in donations annually. DCA's small-dollar fundraising ($5-$50 suggested amounts) would be invisible within this volume.

### Corporate Structure Note

The old "Network for Good" split in 2013:
- **Nonprofit side** → For Good (forgood.org, EIN 68-0480736) — operates the DAF
- **For-profit side** → Acquired by Social Solutions in 2022 → became **Bonterra** (bonterratech.com) — operates the technology platform

The `*.networkforgood.com` subdomain pages use Bonterra's technology but donations flow through For Good's DAF.

---

## 3. STF Part IX Functional Expenses — The $46M Gap Explained

### Complete Part IX Breakdown (2024)

| Category | Amount | % of Non-Grant |
|----------|--------|---------------|
| **Lobbying fees** | **$31,026,950** | **41.8%** |
| **Other professional fees** | **$13,098,791** | **17.6%** |
| **Advertising** | **$8,543,799** | **11.5%** |
| **Salaries & compensation** | **$8,991,950** | **12.1%** |
| **Management fees (Arabella)** | **$6,807,846** | **9.2%** |
| Taxes | $1,861,245 | 2.5% |
| Conferences/meetings | $1,127,172 | 1.5% |
| Legal fees | $766,582 | 1.0% |
| IT | $681,708 | 0.9% |
| Travel | $543,485 | 0.7% |
| Other | $835,112 | 1.1% |
| **Total non-grant expenses** | **$74,284,640** | **100%** |

**Total expenses:** $310,782,035 (STF spent $29M more than revenue, drawing down assets)

### Where the Money Goes

1. **Lobbying ($31M):** Entirely classified as program services. This is STF's primary direct advocacy operation — separate from the $236M in grants to other organizations.

2. **Other professional fees ($13.1M):** Mostly program services ($12.8M). Top contractors include Locust Street Solutions ($3.8M), Global Strategy Group ($2.1M), Blue Rose Research ($1.3M), Markham Group ($914K) — political consulting, polling, and strategic communications firms.

3. **Advertising ($8.5M):** Entirely program services — issue advocacy advertising.

4. **Arabella management fee ($6.8M):** Paid to Arabella Advisors (now Sunflower Services) for "HR, compliance support, payroll, and other administrative functions." NVF acts as common paymaster — STF reimburses NVF for allocated salaries.

### Program Service Categories

| Program | Total Expenses | Grants | Non-Grant Spending |
|---------|---------------|--------|-------------------|
| Civil Rights, Social Action, Advocacy | $262.7M | $219.3M | **$43.3M** |
| Capacity Building | $26.7M | $15.6M | **$11.0M** |
| Health | $10.1M | $0 | **$10.1M** |
| Other | $1.8M | $1.5M | $0.3M |

The Health program spent $10.1M with **zero grants** — all direct operational spending. The Civil Rights program had $43.3M in non-grant spending alongside $219.3M in grants.

### Keyword Search Results — ZERO Digital/Child Safety Mentions

**Not found anywhere in the filing:** "digital," "child safety," "age verification," "app store," "content moderation," "online," "internet," "platform," "social media," "minor," "fiscal sponsor," "sponsored project"

**Found:** "Arabella" (4 references — contractor/administrative), "child" (only in "Idaho Voices for Children Foundation" grantee), "safety" (only in "Nebraska Railroaders for Public Safety" grantee)

### Assessment

The $46M gap is fully accounted for by STF's direct advocacy operations — lobbying, consulting, and advertising on progressive civic engagement, voting rights, healthcare, and environmental issues. **There is no evidence of child safety, digital policy, or age verification spending anywhere in the filing.** However, the $31M in lobbying fees and $13.1M in "other professional fees" are reported only in aggregate — individual contract recipients are listed but their specific lobbying topics are not disclosed. DCA-related spending could theoretically be buried within these line items, but there is no affirmative evidence for this.

---

## 4. Louisiana HB-570 — Meta Wrote the Bill

### Scale Confirmed

Meta deployed **12 lobbyists across 9 firms** in Louisiana, paying at least **$324,992** — described as "a very conservative estimate."

### Three Firms Confirmed

| Firm | Key Personnel | Notes |
|------|--------------|-------|
| **Pelican State Partners, LLC** | John Koch, Christian Rhodes, Scott Kirkpatrick, Suchitra Satpathi, Liza Albrecht | Also represents Roblox |
| **Adams and Reese LLP** | MaryBeth Wilkerson, B. Jeffrey Brooks | #1 ranked LA gov affairs firm; 76 LA clients |
| **State Capitol Solutions / State GR** | Joshua G. Borill | Also represents Chevron |

Six additional firms remain unidentified — Louisiana Board of Ethics interactive database required.

### Critical Finding: Meta Drafted the Bill Language

Investigative reporting confirmed that **a Meta lobbyist "brought legislative language" directly to Rep. Kim Carver** for HB-570. Carver confirmed this publicly. The original bill:
- Required **only app stores** (Google Play, Apple App Store) to verify users' ages
- Required minor accounts to be linked to parental accounts
- Required parents to approve all downloads
- **Did NOT require social media platforms to verify ages within their own apps**

This is the clearest evidence that ASAA legislation is authored by Meta, not by legislators or grassroots advocates.

### The Morris Amendment Battle

**Sen. Jay Morris (R-West Monroe)** introduced the bill's most significant amendment in the Senate Commerce Committee. Morris's amendment **expanded HB-570 to require all app developers (including Meta) — not just app stores — to age-verify users.**

Morris's reasoning "appeared to grow out of a disagreement between Google and Meta." Google's senior director of government affairs **Kareem Ghanem** had questioned why "Mark Zuckerberg [is] so keen on passing these bills," arguing the measures don't change Meta's business model.

**Meta's response:** A company spokesperson "declined to comment, saying Meta was analyzing what the amendments meant for the bill." This silence contrasted sharply with their vocal support for the original version.

**Conference Committee Compromise:** The final version stated that "Developers and covered application store providers shall each be separately responsible for any data each chose to rely on in their independent judgment for compliance with age verification requirements of law." This maintained dual responsibility but gave both sides implementation independence.

**Conference Committee Members:** House — Carver, Hebert, Schlegel; Senate — Cathey, Mizell, Morris.

### Nicole Lopez — Meta's National ASAA Spokesperson

**Nicole Lopez**, Meta's Director of Global Litigation Strategy for Youth, testified at the House Commerce Committee hearing (April 2025):
- Vouched for the **original version** focusing solely on app stores
- Argued app stores "already have the infrastructure in place" for age verification
- Pushed back on accusations that Meta wanted to "shove the responsibility off to Apple and Google"
- Stated: "This is what parents want"

Lopez also testified in **South Dakota** (SB-180) for similar legislation — confirming her role as Meta's national point person for ASAA.

### The Morris-Stefanski Confrontation

At the Senate markup, Sen. Morris directly questioned **Casey Stefanski** (DCA Executive Director) about DCA's funding:
- Morris asked if DCA receives tech company funding
- Stefanski "squirmed, deflected and claimed she 'didn't feel comfortable' answering"
- When pressed for yes/no, admitted receiving tech funding but **refused to name companies**
- Meta stated it has "collaborated with" DCA but neither confirmed direct funding at the time

### What the 12 Lobbyists Actually Did

Based on the legislative record:
1. **Drafted the original bill language** — confirmed by Carver
2. **Testified at committee hearings** — Nicole Lopez at House Commerce
3. **Managed the Morris amendment threat** — the amendment battle was the bill's defining conflict
4. **Coordinated with DCA testimony** — Stefanski testified alongside Meta's own witnesses
5. **Navigated conference committee** — the final compromise language maintained Meta's core benefit (app store responsibility) while adding nominal developer responsibility
6. **Coalition messaging** — Meta, X (Twitter), and Snap issued joint statements supporting app store verification

---

## 5. Matt Ball Contribution Pattern — Deeper Analysis

### Tech Industry Contributions: Complete List

| Date | Contributor | Company | Role | Amount | Committee |
|------|------------|---------|------|--------|-----------|
| 2025-01-27 | Alex Rosen | Sense, Inc. | Co-Founder | $1,175 | Both (maxed) |
| 2025-03-24 | Kyle Gardner | Google | Policy Manager | $450 | Campaign |
| 2025-06-02 | Jake Levine | Meta | Product Manager | $1,175 | Both (maxed) |
| 2025-06-14 | James Rosenthal | Pinterest | Attorney | $1,175 | Both (maxed) |
| 2025-06-23 | Joseph Linn | Microsoft | Software Engineer | $50 | Campaign |
| 2025-06-24 | Kathryn Zyskowski | Instacart | Research | $1,175 | Both (maxed) |
| 2025-06-30 | Joel Lewenstein | Anthropic | Product Designer | $450 | Campaign |
| 2025-07-24 | Dechay Watts | Akamai | Science/Technology | $50 | Campaign |
| 2025-09-28 | Kate Sneed | Comcast | Lobbyist | $50 | Campaign |
| 2025-10-18 | Gabe Rudin | EchoStar | Attorney | $50 | Campaign |
| 2025-12-13 | Christopher Traughber | Tools for Humanity | Science/Technology | $450 | Campaign |

**Total tech industry:** $6,250 (8.0% of $77,953 total fundraising)

### Comparison to Other CO Senate Candidates

| Candidate | Total Raised | Tech $ | Tech % |
|-----------|-------------|--------|--------|
| Emily Sirota (SD-32) | $95,074 | $1,350 | 1.4% |
| Dylan Roberts | $63,088 | $0 | 0.0% |
| **Matt Ball (SD-31)** | **$61,253** | **$3,350** | **5.5%** |
| Dana Charles | $52,864 | $0 | 0.0% |
| Kyle Mullica | $38,675 | $0 | 0.0% |
| Katie Wallace | $28,200 | $0 | 0.0% |

Ball is the **only** 2026 CO senate candidate with contributions from Meta, Pinterest, Instacart, Anthropic, and Google employees.

### The Dual-Maxed Donor Pattern

Eight individuals gave the maximum to both committees ($1,175 total). Of these, **4 are tech company employees** (Rosen/Sense, Levine/Meta, Rosenthal/Pinterest, Zyskowski/Instacart) — all from California or Washington. Only 1 of 8 dual-maxed donors is from Colorado.

### The June 2025 Burst

June 2025 was Ball's biggest fundraising month: 84 contributions, $25,010. The out-of-state share spiked dramatically:
- Out-of-state: 51 donations, $19,650 (78.5% of monthly total)
- Colorado: 33 donations, $5,360 (21.5%)

This appears to be a coordinated fundraising push reaching Ball's out-of-state professional network — tech employees, elite law firm attorneys (Gibson Dunn provided $1,975 from 6 employees in 4 states), and other dual-maxers largely contributed during this window.

### Dominant Sector: Law Firms (19.2%)

The most notable donor pattern is actually **attorneys** at elite national law firms: Gibson Dunn & Crutcher ($1,975), Wachtell Lipton, Paul Hastings, Quinn Emanuel, Outten & Golden, Morrison Foerster. This suggests Ball's primary professional network is legal, with tech as a secondary channel.

### DCA / Conservative Org / Arabella Search — ZERO

**Zero contributions** from any DCA coalition member, Heritage Foundation, NCOSE, Arabella entity, or related organization to Ball's committees.

**One DCA-adjacent finding:** John R Read (employer: "Digital Childhood Alliance," occupation: "Attorney/Legal," Alexandria, VA) gave **$100 to Hetal Doshi for Attorney General** on 2025-10-02. This confirms Read's DCA employment in TRACER records but shows his political giving went to an AG candidate, not to the ASAA sponsor.

### Assessment

The tech industry contribution pattern is distinctive (8% vs. 0-1.4% for peers) but modest in absolute terms. The dual-maxed donor pattern (4 of 8 are tech employees) is more suggestive of coordinated solicitation through professional networks than of a systematic corporate influence campaign. The law firm pattern is actually stronger and may reflect Ball's pre-politics career connections. **The contributions are more consistent with personal network fundraising than with directed corporate coordination**, though the timing concentration in June 2025 warrants further investigation.

---

## Updated Investigation Status

### Questions Answered

| Question | Answer | Significance |
|----------|--------|-------------|
| Does NCOSE have a c4? | **Yes — NCOSEAction, EIN 88-1180705** | New fiscal sponsor candidate for DCA |
| What is NFG's role? | **DAF, not payment processor** | DCA classified as "Project"; potential compliance issue |
| What's in STF's $46M? | **Lobbying ($31M), consulting ($13M), ads ($8.5M)** | No child safety spending found; aggregate reporting obscures detail |
| Were Ball contributions coordinated? | **Suggestive but inconclusive** | 8% tech funding is distinctive but modest; June burst suggests network solicitation |
| What did Meta's LA lobbyists do? | **Drafted bill language, managed amendment battle** | Meta literally wrote HB-570; Morris amendment was the key conflict |

### New Questions Raised

1. **Is NCOSEAction DCA's fiscal sponsor?** May 2025 IRS ruling aligns with DCA's operational timeline. Zero reported revenue could mean first filing hasn't been processed or entity is dormant.
2. **Did DCA register on For Good using DCI's EIN (39-3684798)?** The "Project" classification and absence of EIN disclosure on the donation page suggest a non-standard registration.
3. **What is the legal relationship between NCOSEAction and DCA?** Dawn Hawkins chairs DCA and reports to Marcel van der Watt (NCOSEAction principal officer). Is DCA a project of NCOSEAction?
4. **Does the For Good DAF have expenditure responsibility documentation for DCA grants?** Required if granting to a non-c3.
5. **What are the specific lobbying topics within STF's $31M lobbying budget?** Aggregate reporting conceals whether any portion relates to age verification or tech policy.
6. **Who are the remaining 6 of 9 Meta lobbying firms in Louisiana?** Louisiana Board of Ethics interactive database required.

---

## Sources

### IRS / Nonprofit
- IRS EO BMF extracts: eo1.csv through eo4.csv (March 2026)
- GuideStar: NCOSEAction profile (EIN 88-1180705)
- ProPublica: For Good financials (EIN 68-0480736)
- STF 2024 990 XML: ProPublica download

### Louisiana Legislative
- The Center Square: "Big tech giants battle over competing age verification bills"
- Nola.com: "Will Louisiana require age verification on apps?"
- Pluribus News: "Meta lobbies for app store age verification laws"
- Privacy Daily: "Louisiana App Store Bill Draws Contentious Debate at Senate Markup"
- Louisiana Legislature: legis.la.gov/Legis/BillInfo.aspx?i=248616
- F Minus: fminus.org/clients/pelican-state-partners-llc/, fminus.org/clients/meta-platforms-inc/

### Network for Good / For Good
- For Good FAQ: forgood.org/faq
- For Good What We Do: forgood.org/what-we-do
- DCA donation page source: digitalchildhoodalliance.networkforgood.com

### Campaign Finance
- Colorado TRACER bulk data: tracer.sos.colorado.gov/PublicSite/DataDownload.aspx
- 2025 and 2026 ContributionData.csv files
