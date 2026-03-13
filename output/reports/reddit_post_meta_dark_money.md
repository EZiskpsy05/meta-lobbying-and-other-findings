TL;DR: I collected and compared the full legislative text of age verification bills in California, Colorado, Louisiana, Texas, Utah, and New York. Every single one defines "Operating System Provider" broadly enough to include anyone who "develops, licenses, or controls" an OS on any general-purpose computing device — volunteers who maintain Debian, Fedora, and Arch included. None contain a single exemption for open-source or community-developed software. I then traced the lobbying registrations behind these bills. Meta deployed 86+ lobbyists across 45 states, spent a record $26.3M on federal lobbying in 2025, poured $70M+ into state-level super PACs deliberately structured to avoid centralized disclosure, and a Meta lobbyist literally brought the legislative language for Louisiana's HB-570 directly to the bill's sponsor — confirmed by the sponsor herself. Meta also covertly funds a "grassroots" advocacy group called the Digital Childhood Alliance, which has no EIN in the IRS system and no incorporation record in any state. The same consulting firm (Hilltop Public Solutions) that co-leads Meta's $45M super PAC also coordinates DCA's messaging, perhaps the first confirmed link between Meta's political spending and its astroturf advocacy. Meanwhile, Meta's own Horizon OS already has 83% compliance with these mandates. Linux distributions much less, if any. The EU's equivalent framework explicitly exempts FOSS. The US versions do not. Every source below is a public record.

This isn't a repost of https://www.reddit.com/r/linux/comments/1rmhxk1/i_pulled_the_actual_bill_text_from_5_state_age/ I am not the original author of the post by aaronsb or associated with him; but I did title it similarly for public attention on this subreddit given what I see as the importance of Meta's involvement and the findings of lobbying, "dark" money, and otherwise.

What the bills actually say
I'm going to focus on the specific statutory language because the devil is entirely in the definitions. Most coverage of these bills talks about them in vague terms like "age checks at OS setup." The actual text is worse than that.

California AB-1043 (signed Oct 2025, effective Jan 1, 2027) defines "Operating system provider" under §1798.500(g) as "a person or entity that develops, licenses, or controls the operating system software on a computer, mobile device, or any other general purpose computing device."

That's not limited to companies. That's not limited to mobile. If you maintain an operating system that runs on a general-purpose computing device, you are an "operating system provider" under California law in 10 months. That could be Android, iOS, Linux, Windows, BSD, and even something as obscure or niche as TempleOS.

The bill then requires every OS provider to: (a) provide an accessible interface at account setup requiring a birth date or age, (b) expose a real-time API providing age bracket signals (under 13, 13-16, 16-18, 18+) to any application on the system. Penalties are $2,500 per affected child for negligent violations and $7,500 for intentional ones, enforced by the California AG.

Exemptions under §1798.504(f) cover broadband ISPs, telecom services, and physical products. There is zero exemption for open-source software, community-maintained distributions, non-commercial projects, or volunteer developers.

Colorado SB26-051 (passed Senate 28-7 on March 3, 2026, now in the House) uses identical structure and definitions in the same order: Account Holder, Age-Bracket Data, Age Signal, Application, Covered Application Store, Developer, Device, Operating System Provider, User. Same four age brackets, same penalty structure ($2,500/$7,500), same broadband/telecom/physical-only exemptions. The effective date is Jan 1, 2028. CO adds a narrow enterprise software exemption but nothing for FOSS. There are currently on going meetings regarding this bill in the Senate albeit I can't share any more information about this at the moment.

Louisiana HB-570 the "App Store Accountability Act" is the one where a Meta lobbyist brought the actual legislative language directly to sponsor Rep. Kim Carver. Carver confirmed this publicly. The bill as originally written placed age verification burden exclusively on app stores (Apple, Google), not on platforms like Meta. It was signed June 30, 2025, effective July 1, 2026, after passing unanimously at every stage (House 99-0, Senate 39-0). More on this below

New York S8102A goes further than all of these. It requires manufacturers of internet-enabled devices to conduct "commercially reasonable and technically feasible age assurance" at the point of device activation and explicitly forbids self-reporting. The allowed verification methods would be determined by the Attorney General.

These are not independent legislative efforts. The structural similarity between CA AB-1043 and CO SB26-051 confirms they derive from the same model legislation (the ICMEC "Digital Age Assurance Act" template). The definitions use the same terms in the same order, impose the same penalties, and carve out the same exemptions. Bills have been introduced or are pending in Illinois (3 bills), Texas, Utah, Kansas, South Carolina, Ohio, Georgia, Florida, and at the federal level (KOSA, App Store Accountability Act).

Current status tracker:

State	Bill	Status
CA	AB-1043	Enacted - effective Jan 1, 2027
CO	SB26-051	Passed Senate - in House committee
LA	HB-570	Enacted - effective July 1, 2026
UT	SB-142	Enacted -⚑ first in nation
TX	SB-2420	Enjoined by federal judge
NY	S8102A	Pending
IL	HB-3304, HB-4140, SB-2037	Pending
US (Federal)	KOSA, ASAA	Pending
What this means for Linux, technically
These bills assume every OS has: (1) a centralized account system that collects user identity data, (2) a real-time API that applications can query for a user's age bracket, and (3) integration between this system and whatever mechanism distributes software. Windows has Microsoft Accounts. macOS has Apple ID. Android has Google Accounts.

Linux distributions have adduser. They do not collect birth dates. There is no centralized identity service, no D-Bus API returning age brackets, and no mechanism for apt, dnf, pacman, flatpak, or snap to gate packages based on user age. Implementing this would require:

An account system with age bracket storage (does not exist)

A standardized D-Bus age attestation daemon (does not exist)

Parent-child account linking and parental consent verification (does not exist)

Package manager age-rating enforcement across apt, dnf, pacman, flatpak, snap (does not exist)

A unified parental controls dashboard (does not exist)

Age-gated default user profiles (does not exist)

The "Covered Application Store" definition in these bills is any publicly available platform that distributes applications is broad enough to cover every Linux package repository. One reading of AB-1043 would require age gates on apt install firefox.

And then there's the economics. Commercial age verification vendors (Yoti, Veriff, Jumio) charge $0.10-$2.00 per check, require proprietary SDKs incompatible with GPL licensing, demand API keys tied to commercial accounts, and operate cloud-only with no self-hosted option. A mid-size Linux distribution with ~1M users would face $100K-$2M/year in verification fees with no offsetting revenue. That exceeds many community distros' entire annual budgets. This is of course dependent if the bill(s) require self-attestation or otherwise.

MidnightBSD has already announced it will exclude California residents entirely starting January 1, 2027.

Meta wrote one of these bills
This, to many on this subreddit, is already known. Rep. Kim Carver (R-Bossier City), the sponsor of Louisiana HB-570, publicly confirmed that a Meta lobbyist brought the legislative language directly to her. The bill as originally written required only app stores (Google Play, Apple App Store) to verify user ages. It did not require social media platforms Meta's products to verify ages within their own apps.

Meta deployed 12 lobbyists across 9 confirmed firms for this single bill in Louisiana, paying at least $324,992 (described as a "very conservative estimate"). Confirmed firms include Pelican State Partners (who also represents Roblox, another ASAA beneficiary enabling "broad industry support" framing), Adams and Reese LLP (#1 ranked Louisiana government affairs firm with 76 LA clients), and State Capitol Solutions.

Nicole Lopez, Meta's Director of Global Litigation Strategy for Youth, testified at the House Commerce Committee hearing. She vouched for the version targeting only app stores, argued app stores "already have the infrastructure in place," and pushed back on accusations that Meta wanted to shift responsibility to Apple and Google. Lopez also testified in South Dakota for similar legislation — she's Meta's national point person for ASAA.

The key amendment battle came from Senator Jay Morris (R-West Monroe), who expanded the bill to include app developers alongside app stores. Morris's reasoning grew out of the conflict between Google and Meta. Google's senior director of government affairs had publicly questioned why "Mark Zuckerberg is so keen on passing these bills," pointing out the measures don't change Meta's business model.

When Morris introduced his amendment, Meta "declined to comment, saying Meta was analyzing what the amendments meant for the bill." This silence contrasted sharply with their vocal support for the original version they had drafted.

The conference committee compromise maintained dual responsibility but gave both sides implementation independence. The final bill passed unanimously. Meta got what it needed: the primary burden remained on app stores.

At that same Senate markup, Senator Morris directly questioned DCA Executive Director Casey Stefanski about DCA's funding. Stefanski reportedly squirmed, deflected, and said she wasn't comfortable answering. When pressed for a yes or no, she admitted receiving tech company funding but refused to name the companies.

Why did Meta deploy 12 lobbyists for a bill that passed 99-0? Because the votes were never the concern. The lobbyists were there to control the text and block amendments — like Morris's that would have put the burden back on Meta.

Who benefits from the compliance gap?
Meta's Horizon OS (the operating system on Quest VR headsets) already has 5 built-in compliance features: Meta Account age verification, a Get Age Category API, Family Center parental tools, Quest Store age ratings, and default protections for minor accounts. I assessed Horizon OS at 83.3% compliance readiness with these mandates. Linux distributions score 13.9%.

Meta is not opposing these bills. I pulled lobbying records from the Colorado Secretary of State's SODA API and found Meta has 4 registered lobbyists on SB26-051 through Headwaters Strategies in a "Monitoring" position. Not amending, not opposing. Just watching.

This is notable because on every other child safety bill in Colorado, Meta takes an "Amending" position actively fighting to change bills that regulate social media platforms. From 117 lobbying records across 22 bills:

Bills regulating social media → Meta: "Amending" (fighting changes)

HB25-1287: Social Media Tools for Minor Users

SB25-086: Protections for Users of Social Media

HB24-1136: Healthier Social Media Use by Youth

SB24-158: Social Media Protect Juveniles

Bill putting burden on OS providers → Meta: "Monitoring" (watching passively)

SB26-051: Age Attestation on Computing Devices

Meta fights bills that regulate Meta. Meta watches bills that regulate its competitors and open-source alternatives.

In California, Meta spent $1,036,728 on state lobbying in the first three quarters of 2025 and publicly supported AB-1043 breaking ranks with its own trade associations (TechNet and Chamber of Progress both opposed it). Meta supported a bill that burdens OS providers and app stores while leaving social media platforms untouched.

$70M+ in political spending, deliberately scattered
Meta has poured over $70 million into state-level super PACs — and structured every one of them to avoid the FEC's centralized, searchable database.

Entity	Meta $	Type	Key Detail
ATEP	$45M	527 PAC, bipartisan	Co-led by Hilltop Public Solutions
META California	$20M	State PAC	Chaired by Brian Rice (Meta VP Public Policy)
California Leads	$5M	State PAC	CA candidates
Forge the Future	(from ATEP)	State PAC (TX)	ASAA-aligned policy priorities
Making Our Tomorrow	(from ATEP)	State PAC (IL)	Chaired by Brian Rice
ATEP's $45M flows downstream to Forge the Future in Texas and Making Our Tomorrow in Illinois. By registering every PAC at the state level rather than federally, Meta scatters filings across dozens of separate state ethics commission databases different formats, different disclosure timelines, no centralized search. Each individual filing is technically a public record. Aggregating them into a coherent picture requires manually querying each state. This is structural opacity by fragmentation.

Forge the Future's website explicitly lists three policy priorities, and number two is: "Empowering parents with oversight of children's online activities across devices and digital environments." That is functionally identical to the ASAA's framing parental oversight through device and app-store-level controls. This is the first direct evidence that Meta's super PAC spending is ideologically connected to the ASAA legislative campaign.

Of 20 Meta-backed candidates across Texas and North Carolina primaries, 19 won (per Washington Post, March 12, 2026). Forge the Future supported at least two unnamed Texas state senators — whether one of them was Angela Paxton, the ASAA sponsor, cannot be confirmed from available reporting.

The "grassroots" org that doesn't legally exist
The Digital Childhood Alliance has been testifying in favor of these bills across states, presenting itself as a coalition of 50+ (later inflated to 140+, with only 6 organizations ever publicly named) conservative child safety organizations. Here is what I found:

DCA has no EIN in the IRS Business Master File. I searched all four regional extracts (eo1-eo4.csv) covering every tax-exempt organization in the United States. DCA is not there. I also found no incorporation record in Colorado, DC, Delaware, Virginia, OpenCorporates (200M+ companies), ProPublica, GuideStar, or Charity Navigator.

DCA's domain (digitalchildhoodalliance.org) was registered December 18, 2024 via GoDaddy with privacy protection and a 4-year registration through 2028. The website was live and fully formed one day later — a professionally designed advocacy site pre-loaded with ASAA talking points, Heritage Foundation and NCOSE testimonials, and statistical claims. This is a staging deployment, not a grassroots launch. 77 days later, Utah SB-142 (the first ASAA law in the nation) was signed.

DCA processes donations through Network for Good / For Good (EIN 68-0480736), which is a Donor Advised Fund not a payment processor. For Good explicitly states three times in its documentation that it serves "501(c)(3) non profit organizations." DCA is classified as a "Project" (ID 258136) in the system, not as a standalone nonprofit. I searched all 59,736 For Good grant recipients across five years (~$1.73 billion in total disbursements) and found zero grants to DCA, DCI, NCOSE, NCOSEAction, or any related entity. The donation page appears to be cosmetic — DCA's actual funding comes from Meta directly, not from small-dollar donations.

DCA's leadership comes from NCOSE:

Name	Title	Background
Casey Stefanski	Executive Director	10 years at NCOSE but never appears on any NCOSE 990 as officer, key employee, or among the five highest-compensated
Dawn Hawkins	Chair	CEO, National Center on Sexual Exploitation (dual role)
Melissa McKay	Board President	Utah parent, DCI founder, #FixAppRatings activist
John Read	Senior Policy Advisor	30 years at DOJ Antitrust Division investigated app stores
🖳 The Stefanski detail is unusual. A "Senior Director of Global Partnerships" at a $5.4M organization for 10 years who never appears on a single 990 suggests either an inflated title, below-threshold compensation, or something else about the employment arrangement.

NCOSE's 501(c)(4) structure turns out to be more complicated than initially apparent. Tracing NCOSE's Schedule R filings across four years reveals a two-entity evolution:

FY2021: NCOSE created "NCOSE Action" (EIN 86-2458921) as a 501(c)(4) in Virginia

FY2022: NCOSE Action was reclassified from c4 to c3 supporting organization

FY2023: A new c4 appeared — "National Center on Sexual Exploitation Institute for Public Policy" (EIN 88-1180705), with the same address and Marcel van der Watt as principal officer

FY2024: The original NCOSE Action disappeared from Schedule R entirely. Only the new Institute remains.

NCOSE cycled through two separate 501(c)(4) entities. The first was created, reclassified to c3, and then dropped. The second was created to replace it. What happened to the first entity (EIN 86-2458921) is unknown.

🖳 Despite NCOSE's website describing NCOSEAction as "created by NCOSE," and Schedule R listing the Institute as a "controlled organization" with NCOSE as "direct controlling entity," and van der Watt leading both entities simultaneously — all 19 transaction indicators between NCOSE and the Institute are marked "No" on Schedule R. No grants, no shared employees, no shared facilities, no reimbursements, no transfers of any kind. Zero transactions between a parent and its own controlled c4, while staff move freely between them.

🖳 Concurrently, NCOSE's lobbying spending tripled from $78,000 (FY2023) to $204,000 (FY2024) — coinciding precisely with DCA's launch and the ASAA legislative push across multiple states. NCOSE's program descriptions don't mention ASAA, but the timing is notable.

Meta confirmed as funder: Bloomberg reporters exposed Meta as a DCA funder in July 2025. The Deseret News detailed the arrangement in December 2025. No version of DCA's website has ever disclosed its funding sources — I checked over 100 Wayback Machine snapshots. Every single blog post and testimony targets Apple and Google. Meta is never mentioned or criticized.

The connection between Meta's PAC money and the astroturf
This is the finding that ties two previously separate tracks together.

Hilltop Public Solutions — a Democratic consulting firm — appears in three separate contexts in this investigation:

Co-leads ATEP, Meta's $45M bipartisan super PAC (alongside Republican strategist Brian Baker)

Involved in DCA's messaging coordination, identified in prior investigative reporting

Connected to Forge the Future, the downstream Texas PAC whose policy priorities explicitly mirror ASAA framing

This makes Hilltop the first confirmed entity bridging Meta's political spending operation and the DCA advocacy campaign. The same firm that helps Meta elect "tech-friendly" state legislators also helps coordinate messaging for the nominally independent grassroots organization pushing those legislators to pass ASAA.

The dark money connection
Meta's Colorado lobbying runs through Headwaters Strategies, which has received $338,500 from Meta since December 2019, with monthly payments jumping from ~$5K/month to $14-30K/month starting July 2023 — coinciding with the acceleration of state-level age verification bills.

Headwaters co-founder Adam Eichberg simultaneously serves as:

A registered Meta lobbyist in Colorado

Chair of the Board of the New Venture Fund (NVF) — the flagship entity of the Arabella Advisors network, the largest dark money pass-through infrastructure in US politics ($669M revenue, $768M assets)

Founding board member of the Windward Fund (another Arabella entity, $311M revenue)

The Arabella network operates four entities out of the same building at 1828 L Street NW, Washington DC (suites 300-A through 300-D), with combined annual revenue exceeding $1.3 billion. NVF transfers $121.3M per year to the Sixteen Thirty Fund, a 501(c)(4) with no legal obligation to disclose its donors.

I parsed the IRS Form 990 Schedule I filings across all five Arabella entities — NVF, Sixteen Thirty Fund, Windward Fund, Hopewell Fund, and North Fund. That's 4,433 grants totaling approximately $2.0 billion. I searched for every child safety, age verification, and tech policy organization I could find.

Zero matches. Not a single dollar out of $2 billion went to anything related to child online safety, age verification, or tech policy. The Sixteen Thirty Fund's $31M lobbying budget and $13.1M in "other professional fees" are reported only in aggregate — I searched the complete 990 filing for "digital," "child safety," "age verification," "app store," "online," "platform," and "social media" and found zero matches. The grant pathway through the Arabella network is definitively ruled out. If Meta funds flow through this network, they would have to travel via fiscal sponsorship, consulting fees, or non-grant payments — mechanisms inherently less transparent than Schedule I.

The Eichberg connection matters not because it proves a funding pipeline, but because the person receiving Meta's lobbying payments in Colorado chairs the governance structure of the nation's largest anonymous donor-funded advocacy network. That structural overlap is documented and publicly verifiable regardless of whether money moves through it.

The EU figured this out already
The EU's Digital Services Act takes a fundamentally different approach:

Age verification obligations apply to Very Large Online Platforms (45M+ monthly EU users) — not to OS providers

FOSS projects that don't act as intermediary services are explicitly outside DSA scope (Recital 13)

Micro and small enterprises receive additional exemptions

The EU Digital Identity Wallet (EUDIW) under eIDAS 2.0 is open-source, self-hostable, uses zero-knowledge proofs — no per-check fees, no proprietary SDKs, no API keys

Feature	EU Model	US Model
Regulation target	Platforms (>45M users)	Operating systems (all)
FOSS exemption	Yes (5 mechanisms)	None
Age verification method	EUDIW (open-source wallet)	Commercial vendors (Yoti, Veriff)
Cost to FOSS distros	$0	$100K-$2M/year in per-check fees
Privacy architecture	Privacy-by-design, selective disclosure	Biometric data to vendor cloud
Offline capability	Yes (wallet-based)	No (requires internet per check)
The US bills assume every OS is built by a corporation. The EU approach assumes otherwise.

Asking the questions
I've tried to present findings, not conclusions. But here are the questions I think the Linux community should be asking:

Why does the company that wrote Louisiana's HB-570 — confirmed by the bill's own sponsor — draft legislation that exempts its social media platforms while imposing unfunded mandates on open-source operating systems?

Why do these bills define "Operating System Provider" broadly enough to include volunteer maintainers, but contain zero FOSS exemptions — while the EU's equivalent framework explicitly exempts open-source projects?

Why is Meta the only major tech company taking a passive "Monitoring" position on OS-level age attestation bills while actively fighting every social media regulation bill?

Why does Meta fund an advocacy group (DCA) that has no EIN in the IRS system, no incorporation record in any state, and never discloses its funding — while the same consulting firm (Hilltop Public Solutions) coordinates DCA's messaging AND co-leads Meta's $45M super PAC?

Why does Meta's $45M super PAC fund a downstream Texas PAC (Forge the Future) whose policy priorities are functionally identical to the ASAA bills DCA is pushing?

Why does NCOSE — DCA's institutional parent — report zero transactions with its own controlled 501(c)(4) on Schedule R while staff move freely between entities and lobbying spending triples concurrent with DCA's launch?

System76's CEO Carl Richell met with CO Senator Matt Ball on March 9, who suggested excluding open-source software from SB26-051. Why did it take a single company's CEO showing up at a state capitol for legislators to realize their bill would affect volunteer-run software projects? And why wasn't the FOSS exemption in the template to begin with?

If the goal is child safety, why does the legislation regulate the operating system — which has no contact with children instead of the social media platforms where the actual harm occurs? And why did the company whose lobbyist drafted one of these bills write it to specifically exclude social media platforms from the requirements?

What you can do
Comment on your state's pending legislation. If you're in CO, IL, or NY, these bills are still in committee. The FOSS exemption conversation is happening right now; System76 opened the door in Colorado. Thank you, Carl Ritchell and System76.

Contact the EFF, FSF, and Software Freedom Conservancy. They need the specific statutory language and compliance gap numbers.

If you maintain a distribution, start thinking about your compliance strategy now. CA AB-1043 takes effect January 1, 2027. Louisiana HB-570 takes effect July 1, 2026.

Read the actual bill text. CA AB-1043 is Chapter 675, searchable on leginfo.legislature.ca.gov. CO SB26-051 is on leg.colorado.gov. Don't rely on news summaries the definitions are what matter.

Sources (all public records)
Bill text: CA AB-1043 (Chapter 675), CO SB26-051, LA HB-570 (Act 481 of 2025), NY S8102A, TX SB-2420, UT SB-142

Colorado lobbying: CO Secretary of State SODA API (data.colorado.gov) — datasets vp65-spyn, dxfk-9ifj, df5p-p6jt

Louisiana lobbying: LA Board of Ethics, F Minus database (fminus.org/clients/pelican-state-partners-llc/, fminus.org/clients/meta-platforms-inc/)

California lobbying: CalAccess (cal-access.sos.ca.gov), Bloomberg Government

Super PACs: Forge the Future website (texasforgefuturepac.com — policy priorities), Texas Ethics Commission, Illinois State Board of Elections, Politico (ATEP, Feb 2, 2026), Washington Post (candidate results, Mar 12, 2026)

DCA OSINT: RDAP (rdap.org), Wayback Machine CDX API (web.archive.org, 100+ snapshots), WHOIS/DNS records, IRS EO BMF (eo1-eo4.csv), OpenCorporates, GuideStar

NCOSE: IRS Form 990 (FY2020-FY2024) including Schedule R; NCOSEAction / Institute for Public Policy (EIN 88-1180705) via IRS BMF and GuideStar; original NCOSE Action (EIN 86-2458921) via Schedule R history

Network for Good / For Good: forgood.org/faq, forgood.org/what-we-do, DCA donation page source (targetable_type=Project, targetable_id=258136), For Good 990s 2020-2024 via ProPublica (EIN 68-0480736, 59,736 grant recipients searched)

IRS 990 filings: ProPublica Nonprofit Explorer — NVF (EIN 20-5806345), STF 2024 990 (sixteenthirtyfund.org public disclosure copy, including Part IX functional expenses), DCI (EIN 39-3684798), Windward Fund, Hopewell Fund, North Fund, NCOSE (EIN 13-2608326), ConnectSafely (EIN 47-3168168)

Campaign finance: CO TRACER bulk data (tracer.sos.colorado.gov), FollowTheMoney.org multi-state search, FEC API (api.open.fec.gov — Meta PAC C00502906)

Reporting: Bloomberg (Meta-DCA funding, July 2025), Deseret News (Dec 2025 op-ed), The Center Square (Morris-Stefanski confrontation), ACT | The App Association, Dome Politics, Pluribus News, Nola.com, Privacy Daily (Senate markup), Texas Tribune (Forge the Future), Illinois Sun-Times (Making Our Tomorrow)

LA legislative history: legis.la.gov (HB-570), Rep. Kim Carver public confirmation of Meta-drafted language, conference committee record

Technical analysis: freedesktop.org, GNOME, KDE docs; Meta developer docs (developer.meta.com/horizon); EUDIW GitHub; EUR-Lex (DSA, eIDAS 2.0); T-Scy consortium

Federal lobbying: OpenSecrets (opensecrets.org)

Full dataset, OSINT tasklist, and all processed findings will be published on a repository soon, with sources embedded into each .md (markup file) within the next few days

This is an ongoing OSINT investigation. Pending: Texas Ethics Commission records for Forge the Future expenditure recipients (would confirm whether ASAA sponsor Angela Paxton was supported), NCOSEAction's first 990 filing, and IRS Form 8872 for ATEP political organization disclosures. If you have access to any of these or to lobbying data from states I haven't covered (IL, NY, UT), please reach out.

I'm NOT claiming: I am not claiming Meta wrote every one of these bills (the Louisiana one is confirmed by the sponsor; the others use a shared ICMEC template). I am not claiming there is a direct Arabella-to-DCA funding pipeline (I specifically checked $2B in grants and found no evidence). I am not claiming child safety isn't a legitimate concern. What I AM documenting is: (a) the company whose lobbyist drafted HB-570 wrote it to exclude its own platforms, (b) the advocacy group pushing these bills nationally has no legal existence in the IRS system and is confirmed funded by Meta, (c) the same consulting firm bridges Meta's super PAC and DCA's messaging operations, (d) none of the bills exempt open-source software while the EU equivalent does, and (e) the compliance gap structurally advantages Meta's closed OS over every Linux distribution. The data is above. Draw your own conclusions.

Other Speculation

Meta's lobbying for age verification mandates at the operating system level is not primarily about child safety on social media. It is about the next computing platform.

Meta's Horizon OS; the operating system powering the Quest line of VR/AR headsets is a closed, vertically integrated platform that already has 83.3% compliance with the age attestation requirements in California AB-1043 and Colorado SB26-051. Linux distributions, which form the basis of every viable open-source alternative in the XR (extended reality) space, have 13.9% compliance and would need an estimated 3-5 years of coordinated cross-project development to reach parity.

The age verification bills do not just threaten desktop Linux. They threaten any future open-source operating system for any general-purpose computing device including the headsets, handhelds, and spatial computing platforms that Meta, Apple, and Valve are competing to define.

Horizon OS is Meta's operating system for the Quest line of VR/AR headsets (Quest 2, Quest 3, Quest 3S, and future devices). Key characteristics:

Architecture:

Built on Android Open Source Project (AOSP) with heavy Meta modifications

Microkernel-influenced design with process isolation and hardware abstraction

Closed source — Meta controls the entire stack from hardware through OS through app store

Uses a modified Linux kernel (GPL-licensed, source published via github.com/facebookincubator/oculus-linux-kernel)

Platform control:

Meta Account required for device activation — age and identity collected at setup

Quest Store is the sole first-party app distribution channel (sideloading possible but unsupported)

All apps submit to Meta's review process and IARC age rating requirements

Family Center provides parental oversight, screen time limits, app approval, and activity reports

Minor accounts default to restricted social features, limited discoverability, and private-by-default settings

Market position:

Quest headsets dominate the standalone VR market

Horizon OS was opened to third-party hardware manufacturers in 2024 (Lenovo, ASUS)

Meta positions Horizon OS as the "Android of XR" — an open-enough platform that hardware partners adopt while Meta retains ecosystem control

Revenue model:

Hardware sold near cost or at a loss (subsidized platform strategy)

Revenue from Quest Store commissions (30% cut, matching Apple/Google)

Data collection and advertising integration (Meta accounts, social graph, usage telemetry)

Enterprise licensing (Quest for Business)

III. THE COMPLIANCE GAP
What the bills require vs. what each platform has
California AB-1043 and Colorado SB26-051 impose identical structural requirements. Here is how Horizon OS and a typical Linux distribution score against them:

Horizon OS: 30/36 points (83.3% readiness)

Requirement	Horizon OS Feature	Score
Age verification at account setup	Meta Account collects DOB at sign-up; Get Age Category API exposes age bracket to all apps	3/3
Parental consent for minors	Family Center requires parent to create/approve child accounts	3/3
Data handling for minors	Meta Privacy Center governs data practices; child-specific data limits exist	2/3
Age-appropriate content controls	Quest Store enforces IARC age ratings; Family Center blocks/approves apps	3/3
Transparency reporting	Meta publishes community standards transparency reports (partial coverage)	1/3
App store age-rating enforcement	Quest Store requires IARC ratings for all apps; no unrated apps permitted	3/3
Reasonable age determination	Built-in Get Age Category API (ovr_AgeCategory_Get) returns age bracket	3/3
Parental/guardian consent under 16	Family Center provides parent-child account linking with verified guardian	3/3
Prohibit sale/sharing of minors' data	Privacy Center governs; child-specific restrictions in place	2/3
Duty of care to prevent harm	Personal boundary system, content moderation, harassment reporting built in	2/3
Parental supervision tools	Screen time limits, app approval, activity reports, friend oversight, purchase controls	3/3
Strongest default privacy for minors	Minor accounts: private-by-default, restricted social, limited discoverability	2/3
Linux distribution (generic): 5/36 points (13.9% readiness)

Requirement	Linux Status	Score
Age verification at account setup	No standard age-verification API; AccountsService has no age field	0/3
Parental consent for minors	No built-in parental consent mechanism	0/3
Data handling for minors	Linux does not track/share user data centrally compliance by absence	1/3
Age-appropriate content controls	Flatpak/Snap have OARS age-rating metadata; no enforcement	1/3
Transparency reporting	Not applicable at OS level	0/3
App store age-rating enforcement	Flathub has OARS content ratings; apt/dnf/pacman have none	1/3
Reasonable age determination	No capability exists	0/3
Parental/guardian consent under 16	No capability exists	0/3
Prohibit sale/sharing of minors' data	Linux does not collect data — compliance by absence	1/3
Duty of care to prevent harm	No OS-level duty-of-care features	0/3
Parental supervision tools	GNOME malcontent exists (app restrictions, usage limits) — limited coverage	1/3
Strongest default privacy for minors	No concept of minor-account defaults in standard Linux	0/3
The economic impossibility
Even if the technical work were completed, ongoing compliance requires commercial age verification infrastructure:

Factor	Horizon OS	Linux Distribution
Age verification cost	Built into Meta Account (marginal)	$0.10-$2.00 per check (Yoti, Veriff, Jumio)
Annual cost for 1M users	~$0 (already collected)	$100K-$2M
SDK licensing	Proprietary (internal)	Proprietary SDKs incompatible with GPL
API keys	Internal infrastructure	Requires commercial account; distributing keys in open-source packages exposes them to abuse
Offline capability	Yes (age stored locally in Meta Account)	No — cloud-only verification, requires internet per check
Revenue to offset cost	Quest Store commissions (30%)	$0
A mid-size Linux distribution's entire annual budget may be less than the age verification fees alone. Debian's annual expenses are approximately $300K. Ubuntu's parent company Canonical had revenue of ~$250M, but community distributions like Mint, Manjaro, or elementary OS operate on budgets of $50K-$500K.

IV. THE XR PLATFORM WAR
Current landscape
The XR operating system market is an emerging platform war analogous to the smartphone OS competition of 2007-2012:

Platform	OS	Type	Age Compliance	Market Position
Meta Quest	Horizon OS	Closed, Android-based	83% ready	Market leader (standalone VR)
Apple Vision Pro	visionOS	Closed	~90% ready (Apple ID)	Premium segment
Valve Steam Deck / Index	SteamOS	Linux-based, open	~14% ready	Gaming-focused
Sony PSVR2	PS5 OS	Closed, proprietary	~80% ready (PSN accounts)	Console-tethered
Pico (ByteDance)	Pico OS	Android-based, closed	Unknown	China-focused
Any future open XR platform	Linux-based	Open	14% ready	Does not yet exist
The critical observation: every closed platform is already compliant or near-compliant. Every open/Linux-based platform is not. The legislation doesn't just advantage Meta it advantages the entire closed-platform model over the open one.

Why XR matters for this legislation
The bills don't say "smartphones" or "VR headsets." They say "any general-purpose computing device." AB-1043 §1798.500(g) defines the scope as "a computer, mobile device, or any other general purpose computing device." SB26-051 uses "ANY GENERAL-PURPOSE COMPUTING DEVICE."

XR headsets are general-purpose computing devices. They run web browsers, productivity applications, social platforms, and games. Under these bills, every XR operating system must implement age attestation. The platforms that already have it win.

All research findings, compiled data, sources, and more can be found at the Github Repo:
https://github.com/upper-up/meta-lobbying-and-other-findings
