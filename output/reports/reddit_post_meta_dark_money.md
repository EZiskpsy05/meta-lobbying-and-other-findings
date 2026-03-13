# [OC] I analyzed $1.5 billion in dark money grants and Meta's lobbying records. Here's how Meta built a covert influence machine to pass laws targeting Apple and Google.

---

**TL;DR:** Meta spent a record $26.3M on federal lobbying in 2025, deployed 86+ lobbyists across 45 states, and covertly funded a "grassroots" child safety group called the Digital Childhood Alliance to push the App Store Accountability Act (ASAA) — a law that forces Apple and Google to do age verification, while Meta's own apps face zero new requirements. I parsed IRS 990 filings, state lobbying disclosures, campaign finance records, Wayback Machine archives, and corporate registries. Three charts tell the story.

---

## The Investigation

Over the past several months, I've been conducting an OSINT (open-source intelligence) investigation into Meta Platforms' lobbying and dark money operations surrounding the App Store Accountability Act. Every source is a public record — IRS filings, state lobbying disclosures, campaign finance databases, corporate registries, and archived websites.

What I found is a multi-layered influence operation spanning direct lobbying, covert nonprofit funding, dark money network connections, super PACs, and astroturf advocacy — all designed to pass legislation that shifts regulatory burden from Meta onto Apple and Google.

---

## Chart 1: Meta's Lobbying Spend Hit an All-Time Record

[chart1_meta_lobbying_spend.png]

Meta spent **$26.29 million** on federal lobbying in 2025 — an all-time record that exceeded Lockheed Martin and Boeing. They deployed **86+ registered lobbyists** (up 32% from 65 in 2024) and hired lobbyists in **45 of 50 states**.

The spending escalation directly correlates with the ASAA campaign. In 2022-2023, spending hovered around $19M. Then it jumped to $24M in 2024 and $26.3M in 2025 as ASAA bills were introduced in ~20 states.

In Louisiana alone, Meta deployed **12 lobbyists** for a single bill (HB-570). In California, they spent over **$1 million** in just the first three quarters of 2025, plus **$65 million** through super PACs.

**Sources:** OpenSecrets federal lobbying database, Dome Politics, Quiver Quantitative, Bloomberg Government

---

## Chart 2: $1.5 Billion in Dark Money Grants — $0 to Child Safety

[chart2_arabella_grants_zero.png]

This is the finding that floored me.

Meta's Colorado lobbyist, **Adam Eichberg** (co-founder of Headwaters Strategies, which received $338,500 from Meta), simultaneously serves as **Board Chair of the New Venture Fund (NVF)** — the flagship 501(c)(3) of the Arabella Advisors dark money network, the largest in the United States.

The Arabella network operates four entities out of the same building at **1828 L Street NW, Washington, DC** (suites 300-A through 300-D), with combined annual revenue exceeding **$1.3 billion**:

| Entity | Type | Revenue |
|--------|------|---------|
| New Venture Fund | 501(c)(3) | $669M |
| Sixteen Thirty Fund | 501(c)(4) | $282M |
| Windward Fund | 501(c)(3) | $311M |
| Hopewell Fund | 501(c)(3) | $114M |

NVF transfers **$121.3 million per year** to the Sixteen Thirty Fund — a 501(c)(4) that has **no legal obligation to disclose its donors**.

So I parsed the IRS Form 990 Schedule I filings for both NVF and the Sixteen Thirty Fund. That's **2,975 grants** totaling approximately **$1.5 billion**.

I searched for every child safety, age verification, and tech policy organization I could think of — ConnectSafely, NCMEC, ICMEC, Thorn, Common Sense Media, NCOSE, 5Rights Foundation, FairPlay, CDT, NetChoice, EFF, Digital Childhood Alliance, Digital Childhood Institute, and dozens more. I searched by keyword: child, safety, age, digital, online, internet, cyber, tech, protect, app store, social media.

**Zero matches.** Not a single dollar out of $1.5 billion went to anything related to child online safety, age verification, or tech policy.

The money goes to progressive civic engagement ($420M), environmental causes ($285M), reproductive rights ($180M), internal Arabella transfers ($159M), and state-level organizing ($200M). It's a legitimate progressive grantmaking operation — but it has absolutely nothing to do with child safety.

**What this means:** The most obvious pathway for Meta money to flow through the Arabella network to DCA (via Schedule I grants) is **ruled out**. If Meta uses this network, it would have to be through fiscal sponsorship or non-grant payments — mechanisms that are even more opaque than Schedule I.

**Sources:** IRS Form 990 Schedule I filings via ProPublica Nonprofit Explorer (NVF 2022-2024, STF 2024), Sixteen Thirty Fund public disclosure copy

---

## Chart 3: Meta's Multi-Channel Influence Network

[chart3_influence_network.png]

This chart maps the five confirmed channels Meta uses to advance ASAA:

**1. Direct Federal Lobbying** — $26.3M through 86+ lobbyists, 24 firms, 85% "revolving door"

**2. State Lobbyist Network** — Hired in 45 states. Confirmed firms include:
- **Headwaters Strategies** (Colorado) — $338,500 from Meta. Co-founder Adam Eichberg is simultaneously NVF Board Chair.
- **Pelican State Partners** (Louisiana) — John Dunbar Koch's firm. Also represents Roblox (another ASAA beneficiary). Meta was added as a client specifically in 2024-2025 for the ASAA campaign.

**3. Digital Childhood Alliance** — A 501(c)(4) "grassroots" advocacy group that Meta covertly funds:
- **Bloomberg exposed** Meta as the funder in July 2025
- Executive Director Casey Stefanski (10 years at NCOSE) **partially admitted under oath** to receiving tech company funding but refused to name companies
- Leadership comes from NCOSE (National Center on Sexual Exploitation) — 3 of 4 senior staff have NCOSE connections
- Senior Policy Advisor John Read spent **30 years at DOJ Antitrust Division** investigating app stores
- The "grassroots mom" face is Melissa McKay, an American Fork, Utah resident
- Coalition includes Heritage Foundation, Moms for Liberty, Institute for Family Studies — providing conservative credibility
- Domain registered **December 18, 2024**. Website was live and fully formed **one day later**. No funder disclosures have ever existed on any version of the site (verified via 100+ Wayback Machine snapshots)
- **Every single blog post and testimony targets Apple and Google. Meta is never mentioned or criticized.**

**4. Super PACs** — $65M total: ATEP ($45M bipartisan PAC) + META California ($20M)

**5. State Legislative Campaigns** — ASAA has passed in 3 states:
- Utah SB-142 (signed March 2025) — first in nation
- Texas SB 2420 (signed May 2025) — paused by federal judge December 2025
- Louisiana HB-570 (signed June 2025) — where Stefanski was confronted about funding
- ~17 more states pending, including Kansas, South Carolina, Ohio, Georgia

---

## The Strategic Logic: Why Meta Does This

The App Store Accountability Act requires **app stores** (Apple, Google) to verify user ages before downloads. It does **not** require social media platforms to verify ages within their own apps.

If ASAA becomes national law:
1. Apple and Google bear the compliance cost of age verification
2. Meta's apps (Facebook, Instagram, WhatsApp, Threads) face no direct mandate
3. Parental complaints shift from "Meta showed my kid harmful content" to "Apple failed to check my kid's age"
4. Meta gets to publicly claim it supports child safety while its competitors absorb the burden

This is why Meta broke ranks with its own trade associations — TechNet and Chamber of Progress **opposed** California's version of this law, while Meta itself **supported** it.

---

## The Eichberg Connection: Why It Matters

Adam Eichberg's dual role is the single most significant structural finding:

- As **Headwaters co-founder**, he lobbies on behalf of Meta in Colorado ($338,500 received)
- As **NVF Board Chair**, he governs an organization that transfers $121M+ annually to a 501(c)(4) with complete donor opacity
- The same person who receives Meta's lobbying payments oversees the governance of the nation's largest dark money pass-through entity

I also found that a **Meta Product Manager (Jake Levine)** personally contributed **$1,175** to Colorado State Senator Matt Ball — the sponsor of SB26-051, one of the ASAA bills. A **Google Policy Manager** also contributed $450 to the same legislator. (Colorado TRACER campaign finance data.)

Meanwhile, Eichberg and his Headwaters co-founder Will Coyne made $20,000+ combined in Colorado political contributions — but **neither contributed a cent to any ASAA bill sponsor**. Their giving pattern is standard lobbyist relationship-building, broadly distributed across dozens of Democratic candidates.

---

## What's Still Unknown

1. Whether Meta funds flow through the Arabella network via non-grant mechanisms (fiscal sponsorship, consulting fees)
2. The exact dollar amount Meta has given to DCA
3. Whether Jake Levine's contribution to Matt Ball was coordinated by Meta's government affairs team
4. Windward Fund, Hopewell Fund, and North Fund Schedule I grant recipients (not yet analyzed)
5. FOIA responses pending from Colorado Secretary of State, Colorado Attorney General, and Louisiana Ethics Board

---

## Sources (all public records)

- **Federal lobbying:** OpenSecrets (opensecrets.org)
- **IRS 990 filings:** ProPublica Nonprofit Explorer
- **Colorado lobbying:** CO SOS SODA API (data.colorado.gov)
- **Colorado contributions:** TRACER bulk data (tracer.sos.colorado.gov)
- **Louisiana lobbying:** LA Board of Ethics, F Minus database (fminus.org)
- **DCA website history:** Wayback Machine CDX API (web.archive.org)
- **Sixteen Thirty Fund 990:** sixteenthirtyfund.org public disclosure
- **Reporting:** Bloomberg, Dome Politics, ACT | The App Association, Deseret News, Bloomberg Government

---

*This is an ongoing OSINT investigation. All findings are based exclusively on public records. I'll update as FOIA responses arrive and additional filings are analyzed.*

**Charts:** OC, generated from parsed IRS 990 data, OpenSecrets records, and state disclosure databases.
