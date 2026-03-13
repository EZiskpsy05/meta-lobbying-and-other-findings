# New Venture Fund Schedule I Grant Recipient Analysis

**Research Date:** 2026-03-12
**Data Source:** IRS Form 990 XML e-files via ProPublica Nonprofit Explorer (S3 bulk data)
**Years Analyzed:** 2022, 2023, 2024
**EIN:** 20-5806345

---

## Executive Summary

Analysis of 2,669 grant recipients across three years of NVF Schedule I filings found **NO grants to any target child safety, age verification, or tech policy organizations**. NVF is primarily a progressive advocacy funder focused on civil rights, environment, international development, and education. However, $151M in internal Arabella network transfers (especially $121M to the Sixteen Thirty Fund 501(c)(4)) represent an opaque pipeline that could indirectly fund child safety advocacy without appearing in NVF's own Schedule I.

---

## 1. Dataset Overview

| Tax Year | Grant Recipients | Total Grants |
|----------|-----------------|-------------|
| 2022 | 992 | ~$487M |
| 2023 | 823 | ~$393M |
| 2024 | 854 | ~$401M |
| **Total** | **2,669** | **~$1.28B** |

### Grant Purpose Category Breakdown (All Years Combined)

| Purpose Category | Count | Total Amount |
|-----------------|-------|-------------|
| Civil Rights, Social Action, Advocacy | 1,191 | $548,023,213 |
| International Development | 78 | $311,246,165 |
| Environmental Programs | 465 | $135,638,346 |
| Youth Development and Education | 394 | $73,357,689 |
| Technology and Innovation | 121 | $54,317,648 |
| Conservation and Climate | 34 | $50,042,000 |
| Health | 117 | $31,605,009 |
| Capacity Building | 109 | $22,087,902 |
| All Other | 160 | $55,165,148 |

---

## 2. Target Organization Search Results

### 2.1 Direct Organization Name Search

**SEARCHED FOR:** ConnectSafely, ICMEC, NCMEC, FOSI, Thorn, Common Sense Media, Digital Childhood Alliance, Digital Childhood Institute, NCOSE, 5Rights Foundation, FairPlay, CDT, NetChoice, Chamber of Progress, TechNet, EFF, Family Online Safety Institute

**RESULT: ZERO MATCHES**

None of the target organizations received grants from NVF in any of the three years analyzed. This is a definitive negative finding based on full Schedule I data.

### 2.2 Digital/Online/Internet Safety Keyword Search

**SEARCHED FOR:** Grants where organization name OR purpose contained any combination of (digital, online, internet, cyber, tech) AND (safety, protect, safe, harm, abuse)

**RESULT: ZERO MATCHES**

NVF made no grants whose purpose or recipient name suggests digital/online safety, child online protection, or age verification work.

### 2.3 Child/Youth-Specific Grants

394 grants totaling $73,357,689 were categorized as "Youth Development and Education." These are overwhelmingly:
- **Education access/equity** (Cambiar Education $12.2M, Equal Chance for Education, scholarship programs)
- **Diabetes camps for children** (Camp Leo, Florida Camp for Children with Diabetes, etc.)
- **Child welfare/advocacy** (Children's Defense Fund $17.5K, UNICEF $400K)
- **Early childhood education** (NAEYC, Head Start programs)
- **Youth civic engagement** (Generation Citizen, Young Peoples Alliance)

**No grants related to:** Online safety, age verification, app store regulation, digital childhood, social media harm

### 2.4 Grants with "Child" in Organization Name

37 grants across 3 years. All are traditional child welfare organizations:
- Children's Defense Fund ($17,500)
- Child Care Law Center ($200K + $21.6K)
- International Society for Prevention of Child Abuse ($116K)
- Policy Institute for Children of Louisiana ($21.6K + $287K)
- UNICEF ($400K)
- Coleman Advocates for Children and Youth ($350K + $100K + $258K)

**None related to digital/online child safety or tech policy.**

---

## 3. Internal Arabella Network Transfers

**CRITICAL FINDING:** NVF transferred $150,995,684 to other Arabella network entities:

| Recipient | 2022 | 2023 | 2024 | Total |
|-----------|------|------|------|-------|
| **Sixteen Thirty Fund** (c)(4) | $34,770,000 | $27,601,875 | $58,932,923 | **$121,304,798** |
| **North Fund** | $5,740,000 | $7,112,995 | $8,055,000 | $20,907,995 |
| **Hopewell Fund** | $1,260,000 | $3,081,000 | $4,441,891 | $8,782,891 |
| **Total Internal** | **$41,770,000** | **$37,795,870** | **$71,429,814** | **$150,995,684** |

### Significance

The **$121.3M transfer to the Sixteen Thirty Fund** is the single most important finding in this analysis. The Sixteen Thirty Fund is a 501(c)(4) that:
- **Does NOT disclose its donors** (IRC Section 6033)
- Made $236.5M in grants in 2024 across 318 recipients
- Its own Schedule I would need to be analyzed separately
- Could fund DCA, child safety advocacy, or tech policy organizations without NVF's Schedule I revealing the connection

**In other words:** If Meta or any entity wanted to fund child safety/age verification advocacy through the Arabella network, the path would be:

```
Donor → NVF (c)(3) → Sixteen Thirty Fund (c)(4) → Advocacy group
                      [donors NOT disclosed]      [Schedule I reveals recipients]
```

The NVF → Sixteen Thirty transfer is visible on NVF's Schedule I (this analysis). But the Sixteen Thirty Fund's own donors are never publicly disclosed, and its grant recipients require a separate Schedule I analysis.

---

## 4. Location-Based Analysis

### Washington, DC Grants
- **344 grants** totaling **$343,183,092**
- Top recipients: Sixteen Thirty Fund ($121M), America Votes ($41M), Climate and Clean Energy Equity Fund ($18M), North Fund ($21M)
- Mostly civil rights/advocacy and environmental organizations
- **No child safety or tech policy organizations identified**

### Palo Alto, CA Grants
- 5 grants totaling $1,002,171
- Schmidt Family Foundation, Connect Humanity, Moore Foundation
- **ConnectSafely (3481 Greer Rd, Palo Alto) did NOT receive any NVF grants**

### Alexandria, VA Grants
- 14 grants totaling $11,361,522
- Global Impact, New Virginia Majority, National Science Foundation
- **ICMEC (Alexandria, VA) did NOT receive any NVF grants**

---

## 5. Conclusions

### What This Analysis Proves

1. **NVF does not directly fund** ConnectSafely, ICMEC, NCMEC, DCA, DCI, FOSI, Thorn, or any identified child safety / age verification advocacy organization through its Schedule I grants.

2. **NVF's grant portfolio** is overwhelmingly focused on progressive civic engagement, voting rights, environmental programs, and international development — not technology policy or child safety.

3. **NVF transfers $121M+ to the Sixteen Thirty Fund**, which operates as a 501(c)(4) with full donor opacity and its own $236M+ grant portfolio.

### What This Analysis Does NOT Rule Out

1. **Sixteen Thirty Fund pass-through**: The $121M NVF → Sixteen Thirty pipeline could ultimately reach child safety or tech policy groups. Requires separate Sixteen Thirty Fund Schedule I analysis.

2. **Fiscal sponsorship**: Projects operating under NVF's umbrella as "sponsored projects" may not appear as separate grant recipients on Schedule I. NVF had 964 employees and ~600 volunteers in 2023 — some of these may work on sponsored projects related to tech policy.

3. **Other Arabella entities**: Hopewell Fund and Windward Fund each have their own Schedule I data not yet analyzed.

4. **Indirect influence**: NVF's $36.7M in lobbying expenditures (including $31.2M in grants to other orgs for lobbying) could support age verification advocacy without appearing as Schedule I grants.

---

## 6. Recommended Next Steps

1. **Sixteen Thirty Fund Schedule I analysis** — Download and parse the 318 grant recipients from the 2024 filing. This is the most likely place to find child safety / tech policy funding.
   - ProPublica: https://projects.propublica.org/nonprofits/organizations/264486735

2. **NVF Technology and Innovation grants** — 121 grants totaling $54.3M. Review these for any tech policy adjacent work.

3. **NVF sponsored projects list** — Search for any publicly listed NVF-sponsored projects related to tech policy, age verification, or child safety.

4. **Sixteen Thirty Fund donor investigation** — While donors are not publicly disclosed, congressional investigations and investigative reporting may have identified some donors.

---

## Data Files

- **Full grant list:** `data/processed/nvf_all_grants.csv` (2,669 rows)
- **Keyword matches:** `data/processed/nvf_keyword_matches.json`
- **Raw XML files:** `data/raw/990_xml/nvf_2022.xml`, `nvf_2023.xml`, `nvf_2024.xml`

## Sources

- ProPublica Nonprofit Explorer API: https://projects.propublica.org/nonprofits/organizations/205806345
- IRS Form 990 XML bulk data (via ProPublica S3 redirect)
- NVF 2023 Public Disclosure Copy: https://newventurefund.org/wp-content/uploads/2024/11/2023-New-Venture-Fund-Form-990-Public-Disclosure-Copy.pdf
