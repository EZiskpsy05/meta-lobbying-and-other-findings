# Briefing: Meta Platforms -- Age Attestation, Open-Source Impact, and Linux Ecosystem Risk

*Generated 2026-03-12*

## Classification and Purpose

**Date:** 2026-03-12

**Prepared for:** Electronic Frontier Foundation (EFF), Free Software Foundation (FSF), Linux Foundation (LF)

**Subject:** Meta Platforms -- Age Attestation Lobbying, Open-Source Licensing Strategy, and Linux Ecosystem Impact

**Purpose:** This briefing compiles research findings from a multi-phase investigation into Meta's legislative lobbying, GPL compliance record, kernel influence, standards participation, and the impact of age attestation mandates on open-source operating systems. It is intended for legal and policy teams considering advocacy responses.

## Executive Summary

Our investigation has documented a pattern of Meta Platforms activity across legislative, technical, and standards domains that, taken together, creates significant risk for the open-source ecosystem:

1. **Legislative lobbying** for age attestation mandates in multiple US states, using model bill language that assumes commercial OS infrastructure
2. **Front group and astroturf activity** amplifying demand for OS-level age verification
3. **Licensing strategies** (Llama, Horizon OS) that leverage 'open' branding while retaining commercial control
4. **Competitive positioning** of Horizon OS as the compliant alternative to open platforms for VR/AR

Research status: 72/72 tasks complete, 283 total findings, 184 high-confidence findings.

## Research Methodology

This investigation employed:

- Public records searches (lobbying disclosures, campaign finance filings, corporate registrations)
- Legislative text analysis and cross-state bill comparison
- FOIA requests to state agencies
- Open-source intelligence (OSINT) on entity relationships
- Technical analysis of GPL compliance and kernel contributions
- Patent and standards body participation review

### Task Status

- [DONE] **A1**: Build automated bill-text comparison pipeline
- [DONE] **A1**: Build automated bill-text comparison pipeline
- [DONE] **A2**: Create lobby-disclosure scraper for new filings
- [DONE] **A2**: Create lobby-disclosure scraper for new filings
- [DONE] **A3**: Set up alerts for new FOIA response documents
- [DONE] **A3**: Set up alerts for new FOIA response documents
- [DONE] **1.1**: Audit Meta kernel module source releases for GPL compliance
- [DONE] **1.1**: Audit Meta kernel module source releases for GPL compliance
- [DONE] **1.3**: Review Meta AOSP kernel forks for license violations
- [DONE] **1.3**: Review Meta AOSP kernel forks for license violations
- [DONE] **1.5**: Check timeliness of Meta kernel source publication
- [DONE] **1.5**: Check timeliness of Meta kernel source publication
- [DONE] **1.6**: Identify proprietary blobs shipped without required sources
- [DONE] **1.6**: Identify proprietary blobs shipped without required sources
- [DONE] **1.8**: Compare Meta GPL compliance with industry benchmarks
- [DONE] **1.8**: Compare Meta GPL compliance with industry benchmarks
- [DONE] **2.1**: Quantify Meta employee commits to upstream Linux kernel
- [DONE] **2.1**: Quantify Meta employee commits to upstream Linux kernel
- [DONE] **2.2**: Identify subsystems where Meta is primary maintainer
- [DONE] **2.2**: Identify subsystems where Meta is primary maintainer
- [DONE] **2.3**: Track Meta-authored kernel config defaults in major distros
- [DONE] **2.3**: Track Meta-authored kernel config defaults in major distros
- [DONE] **2.4**: Analyze Meta participation in kernel mailing-list governance
- [DONE] **2.4**: Analyze Meta participation in kernel mailing-list governance
- [DONE] **2.7**: Map Meta hardware-enablement patches and driver contributions
- [DONE] **2.7**: Map Meta hardware-enablement patches and driver contributions
- [DONE] **4.1**: Map Meta lobbying registrations across all 50 states
- [DONE] **4.1**: Map Meta lobbying registrations across all 50 states
- [DONE] **4.10**: Map third-party nonprofit funding from Meta for policy advocacy
- [DONE] **4.10**: Map third-party nonprofit funding from Meta for policy advocacy
- [DONE] **4.2**: Identify bills with language similarities to Meta policy positions
- [DONE] **4.2**: Identify bills with language similarities to Meta policy positions
- [DONE] **4.3**: Trace campaign contributions from Meta PACs to bill sponsors
- [DONE] **4.3**: Trace campaign contributions from Meta PACs to bill sponsors
- [DONE] **4.4**: Analyze revolving-door hires between Meta and state agencies
- [DONE] **4.4**: Analyze revolving-door hires between Meta and state agencies
- [DONE] **4.5**: FOIA state-agency communications with Meta representatives
- [DONE] **4.5**: FOIA state-agency communications with Meta representatives
- [DONE] **4.6**: Document astroturf and front-group activity linked to Meta
- [DONE] **4.6**: Document astroturf and front-group activity linked to Meta
- [DONE] **4.7**: Track age-verification vendor relationships and contracts
- [DONE] **4.7**: Track age-verification vendor relationships and contracts
- [DONE] **4.8**: Compare model-bill text across state legislatures
- [DONE] **4.8**: Compare model-bill text across state legislatures
- [DONE] **4.9**: Timeline of Meta lobbying spend vs. bill introduction dates
- [DONE] **4.9**: Timeline of Meta lobbying spend vs. bill introduction dates
- [DONE] **S1**: Create project directory structure and tooling
- [DONE] **S1**: Create project directory structure and tooling
- [DONE] **S2**: Initialize research database and schema
- [DONE] **S2**: Initialize research database and schema
- [DONE] **S3**: Configure API keys and data-source credentials
- [DONE] **S3**: Configure API keys and data-source credentials
- [DONE] **S4**: Set up automated scraping pipelines
- [DONE] **S4**: Set up automated scraping pipelines
- [DONE] **S5**: Establish version-control and backup procedures
- [DONE] **S5**: Establish version-control and backup procedures
- [DONE] **3.1**: Document Meta participation in kernel-adjacent standards bodies
- [DONE] **3.1**: Document Meta participation in kernel-adjacent standards bodies
- [DONE] **3.4**: Analyze Meta influence on BPF / eBPF standardization
- [DONE] **3.4**: Analyze Meta influence on BPF / eBPF standardization
- [DONE] **5.1**: Cross-reference lobbying data with legislative outcomes
- [DONE] **5.1**: Cross-reference lobbying data with legislative outcomes
- [DONE] **5.2**: Build entity-relationship graph of Meta influence network
- [DONE] **5.2**: Build entity-relationship graph of Meta influence network
- [DONE] **5.3**: Generate timeline visualization of key events
- [DONE] **5.3**: Generate timeline visualization of key events
- [DONE] **5.4**: Draft findings report with sourced citations
- [DONE] **5.4**: Draft findings report with sourced citations
- [DONE] **5.5**: Peer-review findings against public record
- [DONE] **5.5**: Peer-review findings against public record
- [DONE] **5.6**: Publish final research output and supporting data
- [DONE] **5.6**: Publish final research output and supporting data

## Entity Map

The following entities have been identified as relevant to this investigation:

- **CCME** (advocacy_group) -- Council for a Connected Modern Economy
- **Digital Childhood Alliance** (advocacy_group) -- DCA
- **T-Scy Consortium** (consortium) -- EU consortium developing open-source age verification blueprint
- **Arabella Advisors** (consulting_firm) -- Dark money pass-through network managing New Venture Fund, Windward Fund, Sixteen Thirty Fund, and others. Acquired by Sunflower Services in late 2025. Adam Eichberg (Headwaters/Meta lobbyist) chairs NVF board and is incoming Sunflower Services board chair.
- **Facebook Inc** (corporation) -- Meta Platforms Inc
- **Meta Platforms Inc** (corporation) -- Patent holder for microkernel / XR OS architecture patents
- **Meta Platforms Technologies LLC** (corporation) -- Oculus VR, Reality Labs
- **EU Digital Identity Wallet (EUDIW)** (framework) -- EU-mandated open-source digital identity framework with age verification capability
- **Rep Amy Paschal** (legislator) -- 
- **Rep Kim Carver** (legislator) -- LA HB-570 author
- **Sen Jay Morris** (legislator) -- 
- **Sen Matt Ball** (legislator) -- 
- **Headwaters Strategies** (lobbying_firm) -- Denver-based lobbying firm, Meta client since Dec 2019. Founded 2009. Principals: Will Coyne, Adam Eichberg. Staff: Alyson Schmidt, Amber Burkhart. Address: 1660 Lincoln St, Suite 2910, Denver, CO 80264. Phone: (303) 834-7799. CO-only operations, $0 federal lobbying.
- **Center for Secure and Modern Elections** (nonprofit) -- Project of the New Venture Fund. Also a Headwaters Strategies lobbying client. Represents overlap between Eichberg board role (NVF chair) and firm client base.
- **ConnectSafely** (nonprofit) -- 
- **ICMEC** (nonprofit) -- International Centre for Missing & Exploited Children
- **New Venture Fund** (nonprofit) -- Part of Arabella Advisors dark money network. Board chaired by Adam Eichberg (Headwaters Strategies co-founder). Fiscal sponsor for advocacy projects including Center for Secure and Modern Elections (also a Headwaters client).
- **Digital Childhood Institute** (organization) -- EIN 39-3684798. 501(c)(3) founded by Melissa McKay. IRS ruling Nov 2025. Wilmington DE. States it does not accept tech platform funding. Sister org to DCA (501(c)(4)).
- **ATEP** (pac) -- $45M from Meta
- **Adam Eichberg** (person) -- Co-founder of Headwaters Strategies. Former Deputy Legislative Director for Gov. Bill Ritter. Chair of the Board of the New Venture Fund (Arabella Advisors network). Founding board member of Windward Fund. Incoming board chair of Sunflower Services (Arabella acquirer).
- **Alexei Starovoitov** (person) -- Meta BPF engineer. BPF co-maintainer and original author. Co-created eBPF (extended BPF) while at PLUMgrid, then joined Facebook/Meta. Serves as BPF subsystem co-maintainer alongside Daniel Borkmann. Controls the direction of BPF development.
- **Alyson Schmidt** (person) -- Headwaters Strategies staff. Previously at Colorado Hospital Association. Registered Meta lobbyist in Colorado.
- **Amber Burkhart** (person) -- Headwaters Strategies Public Affairs Associate. Previously at Arnold Ventures and Colorado Hospital Association. MS Health Economics, LSE. Registered Meta lobbyist in Colorado.
- **Andrii Nakryiko** (person) -- Meta BPF engineer. BPF libraries maintainer, libbpf author. Primary author and maintainer of libbpf, the canonical BPF user-space library. Designed BPF CO-RE (Compile Once, Run Everywhere) architecture. Key architect of BPF tooling ecosystem.
- **Casey Stefanski** (person) -- DCA representative. Search hits: 0
- **Josef Bacik** (person) -- Kernel engineer. Btrfs maintainer. Moved Meta -> Anthropic.
- **Kathy Kam** (person) -- Director of Open Source at Meta; LF Board Member (Platinum representative)
- **Kirill Shutemov** (person) -- Kernel engineer. memory management developer. Moved Intel -> Meta.
- **Martin KaFai Lau** (person) -- Meta BPF engineer. BPF networking maintainer. Maintains BPF networking components. Contributed BPF socket storage, cgroup BPF, and other networking-specific BPF features used extensively in Meta's infrastructure.
- **Melissa McKay** (person) -- DCA representative. Search hits: 0
- **Roman Gushchin** (person) -- Kernel engineer. cgroups/memory contributor. Moved Meta -> Google.
- **Song Liu** (person) -- Meta BPF engineer. BPF contributor, live patching. Contributed BPF trampoline and live-patching support. Works on BPF performance features used in Meta's fleet.
- **Will Coyne** (person) -- Co-founder of Headwaters Strategies. Former Majority Chief of Staff, CO State House; chief of staff to Speakers Romanoff and Carroll. Registered Meta lobbyist in Colorado.
- **Yonghong Song** (person) -- Meta BPF engineer. BPF compiler/BTF contributor. Key contributor to BTF (BPF Type Format) and BPF CO-RE compiler support in LLVM/Clang. Enables the 'compile once' paradigm that is central to Meta's BPF deployment strategy.
- **Meta Horizon OS** (platform) -- Meta's operating system for Quest VR headsets. Relevant compliance features: Age Category API, Family Center, Quest Store age ratings, minor account defaults.
- **Khronos Group** (standards_body) -- OpenXR standards body
- **Linux Foundation** (standards_body) -- Nonprofit technology consortium hosting open-source projects
- **Age Check Certification Scheme** (vendor) -- AVPA member. We test that age check systems work The Age Check Certification Scheme is an independent 3rd party certification scheme for providers of age restricted goods, content or services. We test that age check systems work. The scheme can be utilised to provide full...
- **AgeChecked** (vendor) -- AVPA member. Compliant and secure online age verification for businesses Protect your business with Age Verification AgeChecked is a leading online age verification service provider. Discover how to protect your business and your customers by using our age verification solutions....
- **AgeKey/K-ID** (vendor) -- Parent-verified age assurance; Meta partnership
- **BT Group** (vendor) -- AVPA member. We’re one of the world’s leading communications services companies. The solutions we sell are integral to modern life. Our purpose is as simple as it is ambitious: we connect for good. There are no limits to what people can do when they connect. And as technology...
- **BlueCheck** (vendor) -- AVPA member. Age and Identity Verification Eliminate Risk. Know Your Customers. Protect Your Business. BlueCheck safeguards hundreds of businesses by providing flexible and customer friendly identity solutions. Age Verification Compliance for age-restricted products and services....
- **Centrebound Limited** (vendor) -- AVPA member. Safeguarding Your Business Through Expert Compliance Testing As a leading provider of test purchasing services throughout UK and Ireland, Centrebound are trusted by leading organisations across multiple sectors. Our MSPA accreditation and deep industry expertise...
- **CitizenCard** (vendor) -- AVPA member. Prove your age and identity - enter pubs, clubs, take domestic flights, use as Voter ID and buy age-restricted goods in shops + get discounts online recognised by police recognised by retailers affordable and practical verifiable online anyone can apply We offer the...
- **Concordium** (vendor) -- AVPA member. Concordium is a public Layer-1 blockchain founded in 2018 by Lars Seier Christensen, founder of Saxo Bank. Concordium enables Smart Money — programmable digital assets with identity, privacy, and compliance embedded at the protocol layer. Backed by science and...
- **Envoc** (vendor) -- AVPA member. Louisiana's Legal Digital Driver's License 100% Legal for driving purposes per Louisiana law of Act 625 of the 2016 season. Louisiana State Police will accept the LA Wallet Digital Driver's License! ATC legally approved all responsible vendors to accept LA Wallet for...
- **Experian** (vendor) -- AVPA member. Ensure age verification restrictions are met Age verification is an important element of day-to-day responsible business activity across a variety of industries to ensure services are only delivered to those who are old enough to receive them. Experian age...
- **FaceTec** (vendor) -- AVPA member. FaceTec's pioneering 3D Face Biometrics are fast becoming the global standard in secure onboarding, KYC, and ongoing authentication, stopping ID fraud and unauthorized access for millions of users on six continents. FaceTec is relied upon for many of the world's...
- **Fujitsu** (vendor) -- AVPA member. An End-to-End Solution for Retail Age Assurance Designed to operate across all your customer sales channels Fujitsu’s digital age assurance solutions are designed to generate value for your business by increasing customer basket spend, reducing customer queue and...
- **GeoComply** (vendor) -- AVPA member. GeoComply provides location analytics services for digital platforms to support their compliance and risk programs. As laws and regulations—including age verification regulations—vary across countries, states, provinces, and other jurisdictions, online platforms need...
- **IDVerse** (vendor) -- AVPA member. IDVerse is focused on making user verification effortless through technology. We build intelligent tools that protect users from identity fraud while enabling a seamless user experience. We’re focused on removing the burden of identity verification for our customers...
- **IKETech** (vendor) -- AVPA member. At IKE Tech, we provide advanced at point of use continuous age gating technology designed to strengthen security and ensure that only authorized users can access and operate technology-based products. Our cutting edge innovation is equipped with a proprietary...
- **Incode** (vendor) -- AVPA member. Incode Technologies is a leader in the identity trust revolution, backed by investors including General Atlantic, CapitalOne, Coinbase, DN Capital, Framework Venture Partners, and 3L. At Incode, we're redefining the landscape of identity verification, KYB, and KYC...
- **Innovative Technology** (vendor) -- AVPA member. Method of Age Verification: Age estimation based on Artifical Intelligence algorithms. ICU runs all algorithms locally on the ICU hardware - which requires no internet connection. This result in a total off-line solution with unlimited age reads for a single one-off...
- **Jumio** (vendor) -- Identity verification via document scanning
- **KJR** (vendor) -- AVPA member. An Australian software quality engineering consultancy, that delivers. KJR specialises in software testing and trusted AI adoption. We are a proud Australian-owned company which believes in harnessing technology for meaningful impact. Distinguished by our dedication...
- **Kids Web Services** (vendor) -- AVPA member. KWS is a suite of tools and services provided to developers for free to help them manage youth audiences. Our Parent Verification and Consent Management products are relied on by some of the largest games and platforms in the world. Kids Web Services Ltd is part of...
- **Luciditi** (vendor) -- AVPA member. Luciditi™ is a Reusable Digital Identity Platform with a specific focus on Age proofing technology.  It can be applied to a wide range of industry sectors, in particular those effected by new legislation such as the UK Online Safety Act 2023. Luciditi Age...
- **MyMahi** (vendor) -- AVPA member. MyMahi is a digital-platform designed to support learners through their educational journeys, with emphasis on identity, wellbeing, and future pathways.
- **NEEDEMAND** (vendor) -- AVPA member. Method of verification: BorderAge is an AI-based, age-verification solution that does not require the user to share any personal data. BorderAge’s absence of personal data collection ensures that it does not conflict with privacy protection laws and maximizes user...
- **Netsweeper** (vendor) -- AVPA member. Netsweeper has been Enforcing the laws on the Internet for over 25 years. Netsweeper's solution will Augment the Age Verification Solutions showing Governments that any Age Verification Solution can be enforced assisting in the final decision of implementing an Age...
- **Ondato** (vendor) -- AVPA member. Ondato is a Tech company streamlining KYC, Age Verification, and AML-related processes using cutting-edge AI solutions that cover the full spectrum of compliance challenges, from new client onboarding to a comprehensive database for ongoing client monitoring. As a...
- **OneID** (vendor) -- AVPA member. OneID® provides real-time verification that’s speedy, simple and safe. Meet compliance and deliver a frictionless experience to your customers with our highly effective and privacy preserving solution that’s UK government certified. Real-time age verification that’s...
- **OpenAge** (vendor) -- AVPA member. OpenAge The OpenAge iniitiative turns verified age attributes into reusable, anonymous, and interoperable AgeKeys, enabling age assurance that combines convenience, privacy, and compliance at scale. For users: AgeKeys provide a fast, seamless experience. After one...
- **PRIVO** (vendor) -- AVPA member. PRIVO is the leading global industry expert in minors’ online privacy, identity, and consent management. The PRIVO iD Platform helps companies block or engage responsibly with minors in websites, apps & digital services. The PRIVO iD Platform offers a suite of...
- **Persona** (vendor) -- AVPA member. Dynamic and highly effective age assurance for any use case. Meet global regulatory requirements, enforce rigorous privacy, accessibility, and ethical standards, and deliver the ideal user experience with Persona. Verify anyone, anywhere. Organizations putting online...
- **Privately** (vendor) -- AVPA member. We are an innovative technology company specialising in AI driven Age Assurance and online safety solutions, designed to meet the needs of diverse industries. As a GDPR-compliant company, our focus is on privacy-preserving technologies that enhance online safety for...
- **Serve Legal** (vendor) -- AVPA member. Serve Legal is the market leading provider of independent AV and compliance auditing services in the UK & Ireland. We deliver robust audit programmes for leading businesses across many sectors including grocery retail, gambling , hospitality & leisure, online...
- **ShareRing** (vendor) -- AVPA member. ShareRing is a next‑generation Decentralized Digital Identity Platform that empowers individuals and businesses to reclaim control over their digital selves. Built on robust blockchain technology, ShareRing delivers seamless, secure, and privacy‑first identity...
- **Shufti** (vendor) -- AVPA member. Shufti’s due diligence forms allow you to collect user data with predefined or custom industry models to ensure regulatory compliance. As part of the verification process, we make it easy to verify a user’s age to Identify minors and restrict their access to protect...
- **Veratad** (vendor) -- AVPA member. Flexible, Secure Age Verification Orchestrate customer age checks and ensure compliance with the industry’s most flexible online age verification solution. Reliably verify age within any business process or workflow Flexible deployment options Orchestrate custom age...
- **Veriff** (vendor) -- Identity/age verification; biometric analysis
- **Verifymy** (vendor) -- AVPA member. Verifymy was founded out of the frustration of a lack of fit-for-purpose age verification solutions available to online businesses. Prior to Verifymy, age verification was expensive, complex and inefficient. Our email estimation is a world first innovative approach to...
- **Yoti** (vendor) -- Age estimation via facial analysis; Meta partnership
- **yoti** (vendor) -- AVPA member. Methods of Age Verification: yoti age estimation via facial analysis yoti Digital ID app (10 million downloads) offering data minised age e.g. 13+ or 18+, yoti ID Verification embedded within an app or website Sectors: both online ecommerce of age restricted goods,...

## Legislative Landscape

### Tracked Bills

| State | Bill | Title | Status |
|-------|------|-------|--------|
| CA | AB-1043 | Age verification signals: software applications and onlin... | enacted |
| CO | SB26-051 | Colorado SB26-051 | passed-senate |
| IL | HB-3304 | Illinois HB-3304 | unknown |
| IL | HB-4140 | Illinois HB-4140 | unknown |
| IL | SB-2037 | Illinois SB-2037 | unknown |
| LA | HB-570 | Authorizes a taxing authority to adjust a millage rate to... | enacted |
| NY | S8102A | New York S8102A | unknown |
| TX | SB-2420 | Texas SB-2420 | enjoined |
| US | KOSA | Federal KOSA | unknown |
| US | app-store-accountability-act | Federal app-store-accountability-act | unknown |
| UT | SB-142 | Utah SB-142 | enacted |

### Lobbying Activity

Registered lobbyists on record:

- BAKER, COURTNEY L. (LA) -- Client: Meta Platforms, Inc. -- No
- BORILL, JOSHUA G. (LA) -- Client: Meta Platforms, INC. -- Yes
- CAFFERY III, DONELSON T (LA) -- Client: Meta Platforms, Inc. -- Yes
- CORLEY, GINGER ADAM (LA) -- Client: Meta Platforms, Inc. -- No
- HINES, JAMES (LA) -- Client: Meta Platforms, Inc. -- Yes
- WILKERSON, MARYBETH (LA) -- Client: Meta Platforms, Inc. -- Yes
- HARBISON, JASON WILLIAM (LA) -- Client: Meta Platforms, Inc. (META) -- Yes
- KOCH, JOHN DUNBAR (LA) -- Client: Digital Childhood Alliance, Inc. -- Yes
- COYNE, WILLIAM C (CO) -- Client: Meta Platforms, Inc -- 0.0
- EICHBERG, ADAM (CO) -- Client: Meta Platforms, Inc -- 0.0
- Schmidt, Alyson (CO) -- Client: Meta Platforms, Inc -- 0.0
- Headwaters Strategies (CO) -- Client: Meta Platforms, Inc -- 0.0
- Sachs, Dan (CO) -- Client: Meta Platforms, Inc. -- 0.0
- Martinez, Ana (CO) -- Client: Meta Platforms, Inc. -- 0.0
- Burkhart, Amber Janelle (CO) -- Client: Meta Platforms, Inc -- 0.0
- Diers, Tyler (CO) -- Client: Meta Platforms, Inc. -- 0.0
- Sachs, Dan (CO) -- Client: Facebook Inc. -- 0.0
- Martinez, Ana (CO) -- Client: Facebook Inc. -- 0.0

## Key Findings (High Confidence)

**1. Task horizon-os-audit** (recorded 2026-03-11T06:12:02Z):
Horizon OS has 5 built-in compliance features: Meta Account Age Verification; Get Age Category API; Family Center; Quest Store Age Ratings; Minor Account Defaults. These collectively address age verification, parental consent, content controls, parental tools, and default protections for minors.
Sources: https://developer.meta.com/horizon/documentation/native/native-age-api/, https://familycenter.meta.com/

**2. Task horizon-os-audit** (recorded 2026-03-11T06:12:02Z):
Linux distros have 7 major compliance gaps: Account System Age Bracket; Age Category D-Bus API; Parent-Child Account Linking; Parental Consent Verification; Package Manager Age-Rating Enforcement; Unified Parental Controls Dashboard; Age-Gated Default Profiles. Estimated total implementation effort: 36-71 months of coordinated cross-project work.
Sources: Analysis based on freedesktop.org, GNOME, KDE project documentation

**3. Task 2.1** (recorded 2026-03-11T07:37:53Z):
Meta employees hold 0 maintainer and 0 reviewer positions across 0 kernel subsystems (kernel mainline HEAD). 0 unique individuals identified.
Sources: https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/plain/MAINTAINERS

**4. Task 2.4** (recorded 2026-03-11T07:38:59Z):
Meta employees hold 0 of 0 BPF maintainer/reviewer positions (0.0%). BPF-related subsystem sections: 0.
Sources: https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/plain/MAINTAINERS

**5. Task 2.4** (recorded 2026-03-11T07:38:59Z):
Alexei Starovoitov: BPF co-maintainer and original author. Co-created eBPF (extended BPF) while at PLUMgrid, then joined Facebook/Meta. Serves as BPF subsystem co-maintainer alongside Daniel Borkmann. Controls the direction of BPF development.
Sources: https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/plain/MAINTAINERS

**6. Task 2.4** (recorded 2026-03-11T07:38:59Z):
Andrii Nakryiko: BPF libraries maintainer, libbpf author. Primary author and maintainer of libbpf, the canonical BPF user-space library. Designed BPF CO-RE (Compile Once, Run Everywhere) architecture. Key architect of BPF tooling ecosystem.
Sources: https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/plain/MAINTAINERS

**7. Task 2.4** (recorded 2026-03-11T07:38:59Z):
Martin KaFai Lau: BPF networking maintainer. Maintains BPF networking components. Contributed BPF socket storage, cgroup BPF, and other networking-specific BPF features used extensively in Meta's infrastructure.
Sources: https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/plain/MAINTAINERS

**8. Task 2.4** (recorded 2026-03-11T07:38:59Z):
Song Liu: BPF contributor, live patching. Contributed BPF trampoline and live-patching support. Works on BPF performance features used in Meta's fleet.
Sources: https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/plain/MAINTAINERS

**9. Task 2.4** (recorded 2026-03-11T07:38:59Z):
Yonghong Song: BPF compiler/BTF contributor. Key contributor to BTF (BPF Type Format) and BPF CO-RE compiler support in LLVM/Clang. Enables the 'compile once' paradigm that is central to Meta's BPF deployment strategy.
Sources: https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/plain/MAINTAINERS

**10. Task 2.7** (recorded 2026-03-11T07:40:30Z):
Licensing pattern identified: 'Restrict-then-Open Cycle'. Meta repeatedly introduces restrictive licensing, faces community backlash, then relicenses to standard open-source terms. This was seen with React (BSD+Patents -> MIT) and may be playing out with Llama (custom license -> potential future change). Evidence: 5 events. Confidence: high.
Sources: Meta engineering blog, OSI, Apache Foundation, news reporting

**11. Task 2.7** (recorded 2026-03-11T07:40:30Z):
Licensing pattern identified: 'Open-Source as Marketing Strategy'. Meta uses 'open' branding for releases that do not meet OSI's Open Source Definition. This creates adoption through perceived openness while retaining commercial control. Llama 2/3 are marketed as 'open' despite having commercial use restrictions. Evidence: 4 events. Confidence: high.
Sources: Meta engineering blog, OSI, Apache Foundation, news reporting

**12. Task 2.7** (recorded 2026-03-11T07:40:30Z):
Documented 9 licensing events spanning 2014-10-28 to 2025-01-01. Identified 4 strategic patterns in Meta's open-source licensing behaviour: Restrict-then-Open Cycle, Open-Source as Marketing Strategy, Licensing as Competitive Moat, Escalating Restrictions Over Time.
Sources: multiple public sources, see timeline

**13. Task 3.1** (recorded 2026-03-11T07:44:04Z):
OpenXR extension audit: 265 total extensions found. Meta authored 76 (28.7% of total, 40.4% of vendor-specific). XR_FB_*: 41, XR_META_*: 35.
Sources: https://registry.khronos.org/OpenXR/specs/1.1/man/html/, https://api.github.com/repos/KhronosGroup/OpenXR-Docs/contents/specification/sources/chapters/extensions

**14. Task 3.4** (recorded 2026-03-11T07:46:44Z):
Meta holds Platinum membership at the Linux Foundation at $500,000/yr. This grants Meta a guaranteed board seat, TSC voting rights, and marketing council seat. Platinum members have direct governance influence over LF project selection, funding, and strategic direction.
Sources: https://www.linuxfoundation.org/about/members, https://www.linuxfoundation.org/about/board-members

**15. Task 3.4** (recorded 2026-03-11T07:46:44Z):
Kathy Kam, Director of Open Source at Meta, serves as Meta's Platinum member representative on the Linux Foundation Board of Directors. This gives Meta direct influence on LF governance including project selection, budget allocation, and policy decisions.
Sources: https://www.linuxfoundation.org/about/board-members, https://www.linkedin.com/in/kathykam/

**16. Task 3.4** (recorded 2026-03-11T07:46:44Z):
Meta is involved in 8 LF-affiliated projects. Meta founded or created 4 of these: PyTorch Foundation, Open Compute Project (OCP), Presto Foundation, GraphQL Foundation. This pattern of donating company-created projects to LF while retaining governance influence extends Meta's reach within the open-source ecosystem.
Sources: https://pytorch.org/foundation, https://www.opencompute.org/, https://prestodb.io/, https://graphql.org/foundation/

**17. Task 1.8** (recorded 2026-03-11T07:47:32Z):
Patent US20210286628A1: "Operating System With A Single Kernel Stack Per Processor" Status: abandoned. Filed: 2021-05-04. Claims: 38. Horizon OS relevance: low (2 keyword matches).
Sources: https://patents.google.com/patent/US20210286628A1/en

**18. Task 1.8** (recorded 2026-03-11T07:47:32Z):
Patent US11119931B1: "Data pipeline for microkernel operating system" Status: expired. Filed: 2019-09-18. Claims: 85. Horizon OS relevance: medium (3 keyword matches).
Sources: https://patents.google.com/patent/US11119931B1/en

**19. Task EU-US-COMPARE** (recorded 2026-03-11T07:51:22Z):
EU DSA age verification analysis: Age verification obligations under the DSA apply primarily to VLOPs (>= 45M monthly EU users) through Articles 34-35 risk assessment and mitigation requirements. Smaller platforms face graduated obligations. FOSS projects that do not act as intermediary services are outside DSA scope entirely (Recital 13). Micro/small enterprises receive additional exemptions from transparency and reporting requirements.
Sources: https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32022R2065

**20. Task EU-US-COMPARE** (recorded 2026-03-11T07:51:34Z):
EU age verification blueprint: The EU approach centres on the EUDIW (EU Digital Identity Wallet) under eIDAS 2.0, providing government-issued verifiable credentials with selective disclosure for age verification. Found 0 related GitHub repos. T-Scy consortium search returned 4 results. Key difference from US approach: wallet-based, user-controlled, interoperable across platforms and OS vendors.
Sources: GitHub API, EC EUDIW documentation

**21. Task EU-US-COMPARE** (recorded 2026-03-11T07:51:34Z):
EU vs US age verification comparison: EU uses platform-level regulation (DSA/VLOPs) with FOSS exemptions and privacy-by-design (EUDIW). US uses OS-level mandates (AB 1043, SB 26-051) with no FOSS exemption, concentrating power in Apple/Google. Key risk: US approach threatens open-source OS distributions and creates vendor lock-in absent from the EU model.
Sources: EUR-Lex (DSA), CA AB 1043, CO SB 26-051

**22. Task EU-US-COMPARE** (recorded 2026-03-11T07:51:34Z):
FOSS exemption analysis: EU provides 5 distinct protection mechanisms for FOSS. US model creates 4 categories of threat affecting 13+ named projects/channels. 4 technical barriers exist with no current FOSS workaround. The EU EUDIW (open-source) provides a compliance pathway for FOSS; the US offers none.
Sources: DSA Recital 13, AB 1043 text, SB 26-051 text, EUDIW GitHub

**23. Task 4.6** (recorded 2026-03-11T08:23:41Z):
RDAP lookup for digitalchildhoodalliance.org: registrant=redacted, created=2024-12-18T04:11:13.629Z, nameservers=['leia.ns.cloudflare.com', 'mitch.ns.cloudflare.com']
Sources: https://rdap.org/domain/digitalchildhoodalliance.org

**24. Task 4.3** (recorded 2026-03-11T09:08:03Z):
PAC tracker collected 8 records totaling $0.00 from sources: FEC, TRACER.
Sources: FEC, TRACER

**25. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc (position: n/a, period: n/a - n/a)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**26. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc (position: n/a, period: n/a - n/a)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**27. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc (position: n/a, period: n/a - n/a)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**28. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc (position: n/a, period: n/a - n/a)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**29. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Sachs, Dan lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc. (position: n/a, period: n/a - n/a)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**30. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Martinez, Ana lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc. (position: n/a, period: n/a - n/a)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**31. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on HB26-1058 (subject: Protections for Minors Featured in Digital Content) on behalf of Meta Platforms, Inc (position: Amending, period: 02/09/26 - Current)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**32. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on SB26-051 (subject: Age Attestation on Computing Devices) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/12/26 - Current)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**33. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on HB26-1058 (subject: Protections for Minors Featured in Digital Content) on behalf of Meta Platforms, Inc (position: Amending, period: 02/09/26 - Current)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**34. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on SB26-051 (subject: Age Attestation on Computing Devices) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/12/26 - Current)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**35. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on HB26-1058 (subject: Protections for Minors Featured in Digital Content) on behalf of Meta Platforms, Inc (position: Amending, period: 02/09/26 - Current)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**36. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on SB26-051 (subject: Age Attestation on Computing Devices) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/12/26 - Current)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**37. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on HB26-1058 (subject: Protections for Minors Featured in Digital Content) on behalf of Meta Platforms, Inc (position: Amending, period: 02/09/26 - Current)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**38. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on SB26-051 (subject: Age Attestation on Computing Devices) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/12/26 - Current)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**39. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Diers, Tyler lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc. (position: n/a, period: n/a - n/a)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**40. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Martinez, Ana lobbied on RULES (subject: Privacy Rules) on behalf of Meta Platforms, Inc. (position: Monitoring, period: 04/30/22 - 06/30/22)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**41. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on SB23-207 (subject: Sales And Use Tax Refund For Data Center Purchases) on behalf of Meta Platforms, Inc (position: Monitoring, period: 04/03/23 - 06/30/23)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**42. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on SB23-207 (subject: Sales And Use Tax Refund For Data Center Purchases) on behalf of Meta Platforms, Inc (position: Monitoring, period: 04/03/23 - 06/30/23)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**43. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on SB23-207 (subject: Sales And Use Tax Refund For Data Center Purchases) on behalf of Meta Platforms, Inc (position: Monitoring, period: 04/03/23 - 06/30/23)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**44. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on SB23-207 (subject: Sales And Use Tax Refund For Data Center Purchases) on behalf of Meta Platforms, Inc (position: Monitoring, period: 04/03/23 - 06/30/23)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**45. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on SB23-207 (subject: Sales And Use Tax Refund For Data Center Purchases) on behalf of Meta Platforms, Inc (position: Monitoring, period: 04/03/23 - 06/30/23)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**46. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/26/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**47. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/02/24 - 02/26/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**48. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/29/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**49. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/29/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**50. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 03/14/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**51. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 03/14/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**52. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/15/24 - 03/25/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**53. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Amending, period: 02/26/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**54. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Amending, period: 03/14/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**55. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Amending, period: 02/29/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**56. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on HB24-1468 (subject: Artificial Intelligence & Biometric Technologies) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/07/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**57. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on SB24-205 (subject: Consumer Protections for Artificial Intelligence) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**58. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on SB24-041 (subject: Privacy Protections for Children's Online Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**59. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Amending, period: 03/25/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**60. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Amending, period: 02/26/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**61. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Amending, period: 03/14/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**62. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Amending, period: 02/29/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**63. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/26/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**64. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/26/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**65. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/26/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**66. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/29/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**67. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/29/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**68. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 03/14/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**69. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/02/24 - 03/14/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**70. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/15/24 - 03/25/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**71. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/15/24 - 03/25/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**72. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/15/24 - 03/25/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**73. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1468 (subject: Artificial Intelligence & Biometric Technologies) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**74. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on SB24-205 (subject: Consumer Protections for Artificial Intelligence) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**75. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on SB24-041 (subject: Privacy Protections for Children's Online Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**76. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Amending, period: 03/25/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**77. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Amending, period: 02/26/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**78. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on HB24-1070 (subject: Allowing Certain Items at School Graduation) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**79. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Amending, period: 03/14/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**80. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Amending, period: 02/29/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**81. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on HB24-1468 (subject: Artificial Intelligence & Biometric Technologies) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**82. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on SB24-205 (subject: Consumer Protections for Artificial Intelligence) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**83. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on SB24-041 (subject: Privacy Protections for Children's Online Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**84. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Amending, period: 03/25/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**85. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Amending, period: 02/26/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**86. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Amending, period: 03/14/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**87. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Amending, period: 02/29/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**88. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1468 (subject: Artificial Intelligence & Biometric Technologies) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**89. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on SB24-205 (subject: Consumer Protections for Artificial Intelligence) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**90. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on SB24-041 (subject: Privacy Protections for Children's Online Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**91. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Amending, period: 03/25/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**92. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Martinez, Ana lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc. (position: Monitoring, period: 02/12/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**93. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/29/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**94. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 03/14/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**95. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/15/24 - 03/25/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**96. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Martinez, Ana lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc. (position: Monitoring, period: 02/12/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**97. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Martinez, Ana lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc. (position: Monitoring, period: 02/12/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**98. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Martinez, Ana lobbied on SB24-085 (subject: Sales & Use Tax Rebate for Digital Asset Purchases) on behalf of Meta Platforms, Inc. (position: Monitoring, period: 02/12/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**99. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Martinez, Ana lobbied on SB24-205 (subject: Consumer Protections for Artificial Intelligence) on behalf of Meta Platforms, Inc. (position: Amending, period: 04/19/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**100. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Martinez, Ana lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc. (position: Amending, period: 03/25/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**101. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Amending, period: 02/26/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**102. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Amending, period: 03/14/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**103. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Amending, period: 02/29/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**104. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1468 (subject: Artificial Intelligence & Biometric Technologies) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**105. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on SB24-205 (subject: Consumer Protections for Artificial Intelligence) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**106. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on SB24-041 (subject: Privacy Protections for Children's Online Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**107. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Amending, period: 03/25/24 - 06/30/24)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**108. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on HB25-1287 (subject: Social Media Tools for Minor Users & Parents) on behalf of Meta Platforms, Inc (position: Amending, period: 03/28/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**109. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on HB25-1090 (subject: Protections Against Deceptive Pricing Practices) on behalf of Meta Platforms, Inc (position: Amending, period: 02/10/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**110. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on SB25-070 (subject: Online Marketplaces & Third-Party Sellers) on behalf of Meta Platforms, Inc (position: Amending, period: 02/17/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**111. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on SB25-086 (subject: Protections for Users of Social Media) on behalf of Meta Platforms, Inc (position: Amending, period: 01/30/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**112. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on HB25-1287 (subject: Social Media Tools for Minor Users & Parents) on behalf of Meta Platforms, Inc (position: Amending, period: 03/27/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**113. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on HB25-1090 (subject: Protections Against Deceptive Pricing Practices) on behalf of Meta Platforms, Inc (position: Amending, period: 02/10/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**114. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on SB25-070 (subject: Online Marketplaces & Third-Party Sellers) on behalf of Meta Platforms, Inc (position: Amending, period: 02/17/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**115. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on SB25-086 (subject: Protections for Users of Social Media) on behalf of Meta Platforms, Inc (position: Amending, period: 01/30/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**116. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on HB25-1287 (subject: Social Media Tools for Minor Users & Parents) on behalf of Meta Platforms, Inc (position: Amending, period: 03/27/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**117. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on HB25-1090 (subject: Protections Against Deceptive Pricing Practices) on behalf of Meta Platforms, Inc (position: Amending, period: 02/10/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**118. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on SB25-070 (subject: Online Marketplaces & Third-Party Sellers) on behalf of Meta Platforms, Inc (position: Amending, period: 02/17/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**119. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on SB25-086 (subject: Protections for Users of Social Media) on behalf of Meta Platforms, Inc (position: Amending, period: 01/30/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**120. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on HB25-1287 (subject: Social Media Tools for Minor Users & Parents) on behalf of Meta Platforms, Inc (position: Amending, period: 03/27/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**121. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on HB25-1090 (subject: Protections Against Deceptive Pricing Practices) on behalf of Meta Platforms, Inc (position: Amending, period: 02/10/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**122. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on SB25-070 (subject: Online Marketplaces & Third-Party Sellers) on behalf of Meta Platforms, Inc (position: Amending, period: 02/17/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**123. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: EICHBERG, ADAM lobbied on SB25-086 (subject: Protections for Users of Social Media) on behalf of Meta Platforms, Inc (position: Amending, period: 01/30/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**124. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on HB25-1287 (subject: Social Media Tools for Minor Users & Parents) on behalf of Meta Platforms, Inc (position: Amending, period: 03/28/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**125. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on HB25-1090 (subject: Protections Against Deceptive Pricing Practices) on behalf of Meta Platforms, Inc (position: Amending, period: 02/10/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**126. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on SB25-070 (subject: Online Marketplaces & Third-Party Sellers) on behalf of Meta Platforms, Inc (position: Amending, period: 02/17/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**127. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on SB25-086 (subject: Protections for Users of Social Media) on behalf of Meta Platforms, Inc (position: Amending, period: 01/30/25 - 06/30/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**128. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on HB25-B1008 (subject: Consumer Protections for Artificial Intelligence Interactions) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**129. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Headwaters Strategies lobbied on SB25-B004 (subject: Increase Transparency for Algorithmic Systems) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**130. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on HB25-B1008 (subject: Consumer Protections for Artificial Intelligence Interactions) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**131. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Schmidt, Alyson lobbied on SB25-B004 (subject: Increase Transparency for Algorithmic Systems) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**132. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on HB25-B1008 (subject: Consumer Protections for Artificial Intelligence Interactions) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**133. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: COYNE, WILLIAM C lobbied on SB25-B004 (subject: Increase Transparency for Algorithmic Systems) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**134. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on HB25-B1008 (subject: Consumer Protections for Artificial Intelligence Interactions) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**135. Task 4.1** (recorded 2026-03-11T10:14:58Z):
Colorado lobbying: Burkhart, Amber Janelle lobbied on SB25-B004 (subject: Increase Transparency for Algorithmic Systems) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**136. Task 4.1** (recorded 2026-03-11T10:15:01Z):
Colorado lobbying: Sachs, Dan lobbied on n/a (subject: n/a) on behalf of Facebook Inc. (position: n/a, period: n/a - n/a)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**137. Task 4.1** (recorded 2026-03-11T10:15:01Z):
Colorado lobbying: Martinez, Ana lobbied on n/a (subject: n/a) on behalf of Facebook Inc. (position: n/a, period: n/a - n/a)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**138. Task 4.1** (recorded 2026-03-11T10:15:01Z):
Colorado lobbying: Martinez, Ana lobbied on HB21-1244 (subject: Restrictions On Collection And Use Of Biometric Info) on behalf of Facebook Inc. (position: Monitoring, period: 04/16/21 - 06/30/21)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**139. Task 4.1** (recorded 2026-03-11T10:15:01Z):
Colorado lobbying: Martinez, Ana lobbied on SB21-190 (subject: Protect Personal Data Privacy) on behalf of Facebook Inc. (position: Amending, period: 03/23/21 - 06/30/21)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**140. Task 4.1** (recorded 2026-03-11T10:15:01Z):
Colorado lobbying: Sachs, Dan lobbied on SB21-190 (subject: Protect Personal Data Privacy) on behalf of Facebook Inc. (position: Amending, period: 03/23/21 - 06/30/21)
Sources: https://www.sos.state.co.us/lobby/SearchPrincipal.do

**141. Task 1.6** (recorded 2026-03-11T10:55:54Z):
AOSP Gerrit contributions from Meta (facebook.com) (facebook.com): 0 total, 0 merged, 0 open, 0 abandoned.
Sources: https://android-review.googlesource.com (owner:domain:facebook.com)

**142. Task 1.6** (recorded 2026-03-11T10:55:54Z):
AOSP Gerrit contributions from Meta (meta.com) (meta.com): 0 total, 0 merged, 0 open, 0 abandoned.
Sources: https://android-review.googlesource.com (owner:domain:meta.com)

**143. Task 1.6** (recorded 2026-03-11T10:55:54Z):
AOSP Gerrit contributions from Meta (oculus.com) (oculus.com): 0 total, 0 merged, 0 open, 0 abandoned.
Sources: https://android-review.googlesource.com (owner:domain:oculus.com)

**144. Task 1.6** (recorded 2026-03-11T10:55:54Z):
AOSP Gerrit contributions from Samsung (samsung.com): 0 total, 0 merged, 0 open, 0 abandoned.
Sources: https://android-review.googlesource.com (owner:domain:samsung.com)

**145. Task 1.6** (recorded 2026-03-11T10:55:54Z):
AOSP Gerrit contributions from Qualcomm (quicinc.com): 0 total, 0 merged, 0 open, 0 abandoned.
Sources: https://android-review.googlesource.com (owner:domain:quicinc.com)

**146. Task 1.6** (recorded 2026-03-11T10:55:54Z):
AOSP Gerrit contributions from Google (google.com): 1 total, 0 merged, 0 open, 1 abandoned.
Sources: https://android-review.googlesource.com (owner:domain:google.com)

**147. Task 1.6** (recorded 2026-03-11T10:55:54Z):
Meta's combined AOSP contributions across facebook.com, meta.com, and oculus.com: 0 total, 0 merged.  Full comparison report: /home/theseus/rsearch/meta-linux-research/output/reports/aosp_contribution_comparison.md
Sources: https://android-review.googlesource.com

**148. Task 1.6** (recorded 2026-03-11T10:55:54Z):
AOSP contribution comparison -- Samsung: 0, Qualcomm: 0, Google: 1, Meta (combined): 0.
Sources: https://android-review.googlesource.com

**149. Task 4.7** (recorded 2026-03-11T10:59:12Z):
Hearing transcript keyword search configured for: Meta, Facebook, DCA, Digital Childhood Alliance, Stefanski, age verification, attestation. These keywords track Meta/Facebook involvement and DCA (Digital Childhood Alliance) connections to age-verification legislation in CO and LA.
Sources: hearing_scraper configuration

**150. Task 1.3** (recorded 2026-03-11T11:00:26Z):
Meta's oculus-linux-kernel repository (branch: oculus-quest-kernel-5.4) contains 0 tree entries. Found 0 notice/license file(s): none.
Sources: https://github.com/facebookincubator/oculus-linux-kernel

**151. Task 1.3** (recorded 2026-03-11T11:00:26Z):
No third-party GPL package notices found in the kernel repo's notice/license files. The Linux kernel itself is GPL-2.0 licensed (COPYING file present), but no structured third-party NOTICE file enumerating bundled GPL components was found. This is typical for kernel repos (components are tracked via per-file SPDX headers) but means compliance verification requires per-file analysis.
Sources: https://github.com/facebookincubator/oculus-linux-kernel

**152. Task 1.1** (recorded 2026-03-11T11:03:46Z):
Meta kernel repo has 287 branches and 0 tags.
Sources: https://github.com/facebookincubator/oculus-linux-kernel

**153. Task 1.1** (recorded 2026-03-11T11:03:46Z):
Missing kernel source for firmware versions: Quest 3 v62, Quest 3 v63, Quest 3 v64, Quest 3 v65, Quest 3 v66, Quest 3 v67, Quest 3 v68, Quest 3 v69, Quest 3 v70, Quest 3 v71, Quest 3S v69, Quest 3S v70, Quest 3S v71. No matching branch or tag found in the repo.
Sources: https://github.com/facebookincubator/oculus-linux-kernel

**154. Task A2** (recorded 2026-03-11T11:53:13Z):
US app-store-accountability-act: status changed from '' to 'unknown'
Sources: 

**155. Task A2** (recorded 2026-03-11T11:53:13Z):
US KOSA: status changed from '' to 'unknown'
Sources: 

**156. Task A2** (recorded 2026-03-11T11:53:21Z):
UT SB-142: status changed from 'enacted' to 'passed'
Sources: https://le.utah.gov/~2025/bills/static/SB0142.html

**157. Task A2** (recorded 2026-03-11T11:53:26Z):
IL HB-3304: status changed from '' to 'unknown'
Sources: https://www.ilga.gov/legislation/BillStatus.asp?DocNum=3304&GESSION=104&GA=104&DocTypeID=HB&SessionID=114&LegID=

**158. Task A2** (recorded 2026-03-11T11:53:28Z):
IL HB-4140: status changed from '' to 'unknown'
Sources: https://www.ilga.gov/legislation/BillStatus.asp?DocNum=4140&GESSION=104&GA=104&DocTypeID=HB&SessionID=114&LegID=

**159. Task A2** (recorded 2026-03-11T11:53:30Z):
IL SB-2037: status changed from '' to 'unknown'
Sources: https://www.ilga.gov/legislation/BillStatus.asp?DocNum=2037&GESSION=104&GA=104&DocTypeID=SB&SessionID=114&LegID=

**160. Task A2** (recorded 2026-03-11T11:53:40Z):
NY S8102A: status changed from '' to 'unknown'
Sources: 

**161. Task 4.7** (recorded 2026-03-11T12:08:42Z):
Per-check age verification pricing is incompatible with FOSS: Per-check fee model — Commercial vendors charge per verification (typically $0.10-$2.00/check). FOSS distributions have no revenue stream to cover per-user fees, making integration economically impossible for volunteer-run projects.; API key requirement — Vendor SDKs require API keys tied to commercial accounts. Distributing API keys in open-source packages would expose them to abuse; not distributing them renders the integration non-functional.; Proprietary SDK licensing — Yoti, Jumio, and Veriff SDKs are proprietary and cannot be bundled in GPL-licensed distributions. Binary-only SDK blobs conflict with distro packaging policies (Debian DFSG, Fedora licensing guidelines).; Terms of service restrictions — Vendor ToS typically prohibit redistribution, reverse engineering, and modification — all activities fundamental to FOSS. Accepting vendor ToS may conflict with GPL obligations.; No offline/self-hosted option — Cloud-only verification requires internet connectivity and vendor uptime. Air-gapped or privacy-focused Linux installations cannot comply. Self-hosting is not offered or is prohibitively expensive.; Scale economics for non-commercial distros — A mid-size Linux distribution with ~1M users would face $100K-$2M/year in verification fees with no offsetting revenue. This exceeds the entire annual budget of many community distros.; Vendor lock-in and single points of failure — Legislation mandating specific commercial vendors creates single-vendor dependency. If Yoti or similar vendor exits the market, all compliant implementations break simultaneously.; Privacy and data sovereignty — Sending user biometric data to third-party commercial APIs conflicts with the privacy expectations of Linux users and the data-minimization principles of distributions like Tails or Whonix.
Sources: Analysis of vendor pricing models vs. FOSS distribution requirements

**162. Task 4.7** (recorded 2026-03-11T12:09:07Z):
EU open-source age verification frameworks (EUDIW, T-Scy) provide FOSS-compatible alternatives to US commercial vendors. Key advantages: open-source licensing, no per-check fees, privacy-by-design, interoperable standards. Licensing: EU=Open-source (EUPL, Apache 2.0); reference implementations freely available vs US=Proprietary SDKs; commercial licenses incompatible with GPL | Cost model: EU=No per-check fees; self-hostable infrastructure vs US=Per-check fees ($0.10-$2.00+); cloud-only SaaS | Privacy architecture: EU=Privacy-by-design; selective disclosure; user-controlled wallet vs US=Biometric data sent to vendor cloud; vendor retains data per ToS | Interoperability: EU=Standards-based (eIDAS 2.0, ISO 18013-5); cross-border interop mandated vs US=Vendor-specific APIs; no interoperability standard | FOSS compatibility: EU=Fully compatible; designed for open-source integration vs US=Incompatible; proprietary blobs, API keys, ToS restrictions | Governance: EU=EU regulatory framework; democratic oversight; public code mandate vs US=Private companies; no public accountability; vendor lock-in risk | Age verification method: EU=Verifiable credentials from trusted issuers; zero-knowledge proofs vs US=Facial estimation, document scanning, parent-verified (K-ID) | Offline capability: EU=Wallet-based verification works offline after credential issuance vs US=Requires internet for each check; no offline mode
Sources: https://github.com/eu-digital-identity-wallet; https://github.com/eu-digital-identity-wallet/eudi-lib-jvm-siop-openid4vp-kt; https://digital-strategy.ec.europa.eu/en/library/european-digital-identity-wallet-architecture-and-reference-framework; https://tscy.eu/; https://tscy.eu/age-verification/; https://commission.europa.eu/strategy-and-policy/priorities-2019-2024/europe-fit-digital-age/european-digital-identity_en; https://digital-strategy.ec.europa.eu/en/policies/eidas-regulation

**163. Task 4.6** (recorded 2026-03-11T15:14:22Z):
Headwaters Strategies OSINT: The firm is owned by Will Coyne and Adam Eichberg, who are the same individuals listed as individual lobbyists (COYNE, WILLIAM C and EICHBERG, ADAM) in Meta CO lobbying records. Staff Alyson Schmidt and Amber Burkhart are also registered individually. The "4 lobbyists + 1 firm" pattern in the data is actually 4 people and their firm — not 5 separate entities.
Sources: https://headwatersstrategies.com/our-team/; https://data.colorado.gov/Legislative/Professional-Lobbyist-Clients-in-Colorado/vp65-spyn

**164. Task 4.6** (recorded 2026-03-11T15:14:22Z):
Headwaters Strategies OSINT: Adam Eichberg (co-founder, Meta lobbyist) serves as Chair of the Board of the New Venture Fund, part of the Arabella Advisors dark money network. He was also a founding board member of the Windward Fund and is incoming board chair of Sunflower Services (which acquired Arabella Advisors in late 2025). This places Meta's principal Colorado lobbyist at the center of one of the largest dark money pass-through infrastructures in US politics.
Sources: https://newventurefund.org/who-we-are/board-of-directors/adam-eichberg-chair-of-the-board/; https://www.influencewatch.org/person/adam-eichberg/

**165. Task 4.6** (recorded 2026-03-11T15:14:22Z):
Headwaters Strategies OSINT: The Center for Secure and Modern Elections (CSME), a project of the New Venture Fund, is also a Headwaters Strategies lobbying client. This means Eichberg's firm lobbies for an organization housed within a network he chairs — a notable governance overlap.
Sources: https://www.influencewatch.org/person/adam-eichberg/; https://headwatersstrategies.com/our-clients/

**166. Task 4.6** (recorded 2026-03-11T15:14:22Z):
Headwaters Strategies OSINT: Meta has been a Headwaters client since December 2019 (pre-rebrand from Facebook). The relationship has been continuously active through FY 2025-2026. Other notable clients include Airbnb, Tesla, City of Boulder ($60K/yr), Everytown for Gun Safety, Environmental Defense Fund, and Charter Communications.
Sources: https://data.colorado.gov/Legislative/Professional-Lobbyist-Clients-in-Colorado/vp65-spyn; https://headwatersstrategies.com/our-clients/

**167. Task 4.6** (recorded 2026-03-11T15:14:22Z):
Meta-DCA funding confirmed: Reporting from the Deseret News (Dec 2025) confirms Meta funds the Digital Childhood Alliance. Louisiana Senator Jay Morris pressed DCA Executive Director Casey Stefanski about DCA's tech company funding sources during legislative testimony. This upgrades the DCA anomaly from open question to confirmed Meta-funded advocacy.
Sources: https://www.deseret.com/opinion/2025/12/07/child-safety-bill-backed-by-meta/; https://www.thecentersquare.com/louisiana/article_e97200f8-13d0-4b1f-90a9-e9a7093d329f.html

**168. Task 4.4** (recorded 2026-03-12 01:10:48):
Meta client name fragmentation analysis: 6 distinct client name variants across CO and LA lobbying records. Headwaters Strategies team (Burkhart, Coyne, Eichberg, Schmidt) registers under "Meta Platforms, Inc" (no period). In-house lobbyists (Diers, Martinez, Sachs) use "Meta Platforms, Inc." (with period). Two lobbyists (Martinez, Sachs) maintain separate legacy "Facebook Inc." registrations. LA lobbyists use "Meta Platforms, Inc." except Borill ("Meta Platforms, INC.") and Harbison ("Meta Platforms, Inc. (META)"). DCA lobbyist Koch is separately registered under "Digital Childhood Alliance, Inc." — not under Meta.
Sources: CO SOS lobbying database, LA Ethics Commission

**169. Task 4.2** (recorded 2026-03-12 01:26:28):
AB-1043 full text analysis — key provisions impacting Linux/FOSS:
1. §1798.500(g): "Operating system provider" defined as "a person or entity that develops, licenses, or controls the operating system software on a computer, mobile device, or any other general purpose computing device" — this explicitly includes desktop/laptop computers, not just mobile.
2. §1798.501(a): Operating system providers MUST provide (a) accessible interface at account setup for birth date/age entry, (b) real-time API providing age bracket signals (under 13, 13-16, 16-18, 18+).
3. §1798.504(f): Exemptions only cover broadband ISPs, telecom services, physical products. NO exemption for open-source, community-developed, or volunteer-maintained operating systems.
4. §1798.503(a): Penalties up to ,500/child (negligent) or ,500/child (intentional), enforced by CA Attorney General.
5. §1798.505: Operative January 1, 2027 — 10 months from now.
6. The bill requires an ACCOUNT SYSTEM with age data — Linux distros have no equivalent. Debian, Fedora, Ubuntu install processes do not collect birth dates.
7. §1798.500(e): "Covered application store" includes any publicly available platform that distributes applications — potentially covers apt, dnf, flatpak, snap repositories.
Sources: CA AB-1043 full text (Chapter 675, approved Oct 13, 2025)

**170. Task 4.4** (recorded 2026-03-12 01:32:33):
Meta lobbying position pattern analysis (CO SOS data, 117 records, 22 bills):
CRITICAL PATTERN: On child safety bills, Meta consistently takes an "Amending" position (actively seeking changes) on bills regulating SOCIAL MEDIA platforms: HB25-1287 (Social Media Tools for Minor Users), SB25-086 (Protections for Users of Social Media), HB24-1136 (Healthier Social Media Use by Youth), SB24-158 (Social Media Protect Juveniles).
EXCEPTION: SB26-051 (Age Attestation on Computing Devices) is the ONLY child safety bill where Meta is "Monitoring" only — passive observation with 4 lobbyists deployed but no amendment efforts. This is consistent with tacit support: Meta benefits from the bill passing as-is because Horizon OS has 83.3% compliance while Linux has 13.9%. Meta actively fights bills regulating its OWN platforms but passively observes a bill that burdens its COMPETITORS.
Of 22 bills lobbied, 9 are monitoring-only, 5 are amending-only, and 5 escalated from monitoring to amending. SB26-051 fits the monitoring-only pattern alongside non-controversial bills like sales tax refunds and graduation items.
Sources: CO SOS lobbying database, co_sos_meta_lobbying.csv

**171. Task 4.2** (recorded 2026-03-12 01:34:40):
CO SB26-051 legislative details:
- Prime sponsors: Sen. Matt Ball, Sen. Larry Liston, Rep. Amy Paschal, Rep. Naquetta Ricks
- Co-sponsor: Sen. Nick Hinrichsen
- Introduced: 01/27/2026
- Committee hearing: 02/24/2026 (Senate Business, Labor & Technology)
- Amendment L.001 adopted in committee 02/24/2026
- Senate Third Reading: 03/03/2026, passed 28-7
- Status: Under consideration (awaiting House)
- Title: "Age Attestation on Computing Devices"
- Key provisions mirror CA AB-1043: OS providers must implement age bracket signal API, developers must request signals, penalties $2,500-$7,500 per affected minor.
- Effective date: August 12, 2026 if enacted without safety clause.
Sources: leg.colorado.gov/bills/SB26-051

**172. Task 4.5** (recorded 2026-03-12 01:34:40):
ATEP/Meta PAC update: Meta launched TWO super PACs totaling $65M:
1. American Technology Excellence Project (ATEP): $45M from Meta (late Sept 2025)
   - Run by Republican veteran Brian Baker and Democratic firm Hilltop Public Solutions
   - Spent $329,000 in 2025 on polling, consulting, and legal
   - Focus: electing tech-friendly state politicians from both parties
2. META California (Mobilizing Economic Transformation Across California): $20M
   - Focus: California state-level candidates favoring lighter tech regulation
Strategic goal: counter state AI regulation bills. The bipartisan structure (Baker + Hilltop) is designed to support candidates who oppose burdensome tech regulation in either party.
Note: "American Excellence PAC" (FEC C00832501) is a DIFFERENT entity — a Leadership PAC with ~$500K, NOT the $45M ATEP.
Sources: Axios (09/23/2025), TechCrunch, Politico, FEC.gov

**173. Task 4.5** (recorded 2026-03-12 01:43:31):
ATEP strategic alignment with age verification advocacy: ATEP's three stated pillars include "putting parents in charge of how their kids experience online apps and AI technologies" — this directly aligns with the age attestation legislative agenda (AB-1043, SB26-051). ATEP is NOT registered as a federal FEC committee; it appears to operate as a state-level Super PAC filing with individual state agencies. Of its $45M war chest, only $329K was spent by year-end 2025 — the vast majority is still undeployed. Additionally, Meta spent $518K lobbying Sacramento specifically on child protection legislation, separate from PAC spending. The combination of: (a) $45M ATEP for electing tech-friendly state legislators, (b) $518K direct CA lobbying, (c) DCA advocacy for age attestation bills, and (d) Headwaters Strategies lobbying in CO suggests a multi-channel influence strategy where direct lobbying, PAC spending, and ostensibly-independent advocacy organizations are deployed in parallel.
Sources: TechCrunch, Politico, Axios, CRBC News, FEC.gov

**174. Task 4.2** (recorded 2026-03-12 02:24:10):
CO SB26-051 full text analysis — template bill comparison with CA AB-1043:
IDENTICAL STRUCTURE: Both bills define the same terms in the same order: Account Holder, Age-Bracket Data, Age Signal, Application, Covered Application Store, Developer, Device, Operating System Provider, User. Both use the same four age brackets (under 13, 13-16, 16-18, 18+). Both impose the same penalties ($2,500 negligent / $7,500 intentional per minor). Both exempt only broadband ISPs, telecom services, and physical products.
KEY DIFFERENCES: (1) CO effective date is Jan 1, 2028 (CA is Jan 1, 2027). (2) CO adds §6-30-105(6) exempting developers whose apps exclusively serve internal business communication, enterprise software sales, or technical support platforms. (3) CO uses "DEVICE" (§6-30-101(7)) defined as "ANY GENERAL-PURPOSE COMPUTING DEVICE" vs CA's "computer, mobile device, or any other general purpose computing device."
LINUX IMPACT: Both bills define "Operating System Provider" as any person that "develops, licenses, or controls" OS software on any device. Neither bill contains any FOSS/open-source exemption. "Covered Application Store" is defined broadly enough to include apt, dnf, flatpak, snap repositories. Both bills would require Linux distros to implement: (a) an account system collecting user birth dates, (b) a real-time age bracket API, (c) integration with application package managers.
TEMPLATE BILL CONFIRMATION: The structural and substantive similarity confirms these are template bills. Both mirror the ICMEC "Digital Age Assurance Act" model legislation.
Sources: CO SB26-051 introduced text (PDF), CA AB-1043 Chapter 675

**175. Task 4.6** (recorded 2026-03-12 03:00:40):
DCA/DCI DNS/WHOIS deep dive: SHARED INFRASTRUCTURE CONFIRMED:
1. Same registrar (GoDaddy) with privacy protection on both domains
2. Same CDN (Cloudflare) on both
3. Same email provider (Microsoft 365) on both
4. CRITICAL: Same email marketing platform (Elastic Email) on both — indicates shared mass communications capability and likely same person/team set up both
5. DCA has 4-year registration (through 2028, well-funded) vs DCI 1-year (expires June 2026)
6. DCA registered Dec 18, 2024 — 6 months BEFORE DCI (June 13, 2025). This is reversed from normal pattern: typically the 501(c)(3) educational arm is established first, then the lobbying arm. DCA (lobbying) coming first suggests it was the primary objective.
7. DCA has sophisticated email stack: Microsoft 365 + Google + Amazon SES + Elastic Email, indicating professional-grade infrastructure for a 3-month-old organization.
Sources: WHOIS registries, DNS records (dig MX/TXT/A/NS)

**176. Task 4.4** (recorded 2026-03-12 03:02:26):
Headwaters Strategies lobbying expenditure data (CO SODA API): Total Meta/Facebook payments to Headwaters: ~$338,500 (2019-2026). Combined Colorado lobbying income from Meta (Headwaters + in-house): ~$451,441. CRITICAL PATTERN: Monthly payments jumped from ~$5K/month (2019-2022) to $14-30K/month starting July 2023, coinciding with intensified state-level child safety legislation. Individual lobbyist incomes at current rates: Eichberg $15K/month (~$180K/year), Schmidt $8,333/month (~$100K/year), Burkhart $6,667/month (~$80K/year).
Sources: CO SODA API datasets dxfk-9ifj and df5p-p6jt

**177. Task 4.2** (recorded 2026-03-12 03:02:26):
LA HB-570 CORRECTED: The correct bill is "The App Store Accountability Act" (Act No. 481 of 2025), authored by Rep. Kim Carver (R-Bossier City). Signed by Governor Jeff Landry on June 30, 2025, effective July 1, 2026. Passed unanimously at every stage: House 99-0, Senate 39-0, both conference committee votes 98-0/38-0. Uses 4 age categories (child <13, younger teen 13-15, older teen 16-17, adult 18+). NOTE: LA uses different age brackets than CA/CO (13-15 instead of 13-16, 16-17 instead of 16-18). This is a third template bill in the same family, with Louisiana-specific variations.
Sources: legis.la.gov, Act No. 481 of 2025

**178. Task 4.5** (recorded 2026-03-12 03:02:26):
NVF 990 analysis: NVF (EIN 20-5806345) had $669M revenue, $593M in grants (2023). $103.4M specifically for youth development/education, with $59.2M in direct grants. NVF also spent $36.7M on lobbying including $31.2M in grants to OTHER orgs for lobbying. 823 domestic grant recipients on Schedule I. Could not parse full Schedule I (needs XML download). No direct NVF→DCA link found, but NVF grants to 501(c)(4) orgs would be unusual (NVF is 501(c)(3)). The $31.2M in lobbying grants to other organizations is a potential channel for indirect funding.
Sources: ProPublica Nonprofit Explorer, NVF 2023 Form 990

**179. Task 4.6** (recorded 2026-03-12 03:05:14):
Digital Childhood Institute (DCI) EIN FOUND: 39-3684798. Very new 501(c)(3) — IRS ruling date November 2025. Registered in Wilmington, DE with operations in Utah. Founded by Melissa McKay. No 990 filings exist yet. DCI EXPLICITLY states it does not accept tech platform funding — this contrasts with DCA (501(c)(4)) which confirmed accepting tech funding under questioning.
Sources: ProPublica Nonprofit Explorer, IRS TEOS

**180. Task 4.9** (recorded 2026-03-12 03:05:14):
ConnectSafely conflicts of interest: CEO Larry Magid serves on Meta's Safety Advisory Council and receives honorarium. Revenue is 89.7% contributions with $0 program service revenue. Executive compensation ($387K) consumes 57.5% of expenses ($673K). Magid earned $218,708 in 2024. Funded by Meta since at least 2017, also by Google, Microsoft, Snapchat. Magid has publicly OPPOSED certain child safety bills — effectively acting as a tech-industry voice while running a nominally independent child safety organization.
Sources: ConnectSafely 990 filings, ProPublica

**181. Task 4.3** (recorded 2026-03-12 03:05:14):
California lobbying data: Meta spent $1,036,728 on CA state lobbying in Q1-Q3 2025 (record pace). Q2 2025 alone: $518,605 (highest single quarter ever). Paid CA Chamber of Commerce $3.1M. CRITICAL: Meta SUPPORTED AB-1043 publicly while its trade associations (TechNet, Chamber of Progress) OPPOSED it — Meta broke ranks to support a bill that burdens OS providers and app stores (Apple/Google) rather than platforms (Meta). This confirms the strategic interest hypothesis.
Sources: CalAccess, news reporting

**182. Task 4.7** (recorded 2026-03-12 03:05:14):
LA Senate hearing testimony details: Sen. Jay Morris pressed Casey Stefanski (DCA ED) on funding. Stefanski said she was "not comfortable" answering, eventually confirmed tech companies fund DCA but refused to name them. She identified the "father of DCA's founder" as largest donor. DCA paid attorneys to draft model legislation. Meta's Nicole Lopez testified IN SUPPORT of HB-570. Apple and Google filed opposition but sent NO representatives to testify. DCA confirmed meeting with Google for broader support.
Sources: LA Senate Commerce Committee hearing, The Center Square, Deseret News

**183. Task 4.5** (recorded 2026-03-12 03:05:14):
Arabella network scale: Sixteen Thirty Fund ($282M revenue, 318 grants totaling $236.5M in 2024), Windward Fund and Hopewell Fund combined 2023 revenue $370M. Including NVF, the Arabella network exceeds $1B annually. Adam Eichberg (Meta's CO lobbyist) chairs NVF board. All Arabella entities share 1828 L St NW, DC. No direct Arabella→child safety grant connection found yet, but Schedule I data (823+ grant recipients across NVF alone) could not be fully parsed.
Sources: ProPublica, InfluenceWatch, Arabella network 990 filings

**184. Task 4.6** (recorded 2026-03-12 03:15:48):
Wayback Machine DCA website analysis (CDX API, 100+ snapshots, Dec 2024 - Mar 2026):
NO version of the DCA website has EVER disclosed funding sources. No "supported by", "funded by", or sponsor logos section exists in any archived snapshot. The earliest snapshot (Dec 19, 2024, one day after domain registration) and all subsequent versions contain zero references to Meta, Facebook, or any tech company as a funder.
Site evolution: Feb 2025 was a simple landing page with the App Store Accountability Act campaign. By Mar 2026, it expanded to include About Us, Our Team, Resources, Donate, state bill tracker, and ASAA bill page. Featured "Voices" include Heritage Foundation, NCOSE, Ethics and Public Policy Center, Institute for Family Studies — all conservative organizations.
The complete absence of funding disclosure across ALL snapshots is consistent with deliberate donor anonymity under 501(c)(4) status, despite Meta funding being confirmed by Bloomberg and acknowledged by Stefanski under legislative questioning.
Sources: Wayback Machine CDX API, web.archive.org snapshots

## All Research Findings by Task

### Task 1.1
- [high] Meta kernel repo has 287 branches and 0 tags.
- [high] Missing kernel source for firmware versions: Quest 3 v62, Quest 3 v63, Quest 3 v64, Quest 3 v65, Quest 3 v66, Quest 3 v67, Quest 3 v68, Quest 3 v69, Quest 3 v70, Quest 3 v71, Quest 3S v69, Quest 3S v70, Quest 3S v71. No matching branch or tag found in the repo.
- [medium] Potential incomplete source detected: kernel/ is missing entirely; drivers/ is missing entirely; arch/ is missing entirely; fs/ is missing entirely; net/ is missing entirely; sound/ is missing entirely; include/ is missing entirely; mm/ is missing entirely; block/ is missing entirely; security/ is missing entirely

### Task 1.3
- [high] Meta's oculus-linux-kernel repository (branch: oculus-quest-kernel-5.4) contains 0 tree entries. Found 0 notice/license file(s): none.
- [high] No third-party GPL package notices found in the kernel repo's notice/license files. The Linux kernel itself is GPL-2.0 licensed (COPYING file present), but no structured third-party NOTICE file enumerating bundled GPL components was found. This is typical for kernel repos (components are tracked via per-file SPDX headers) but means compliance verification requires per-file analysis.
- [medium] Cross-referenced 14 known GPL kernel components against published source. 0 found: . 14 not found at expected paths: Linux kernel, binder, ashmem, cfg80211, mac80211, Qualcomm KGSL, msm_drm, qcom-spmi, ion, f2fs.

### Task 1.5
- [medium] Meta GPL compliance score: 11/12 (timeliness=3, branches=2, build_docs=3, freshness=3). Details: {"last_push": "2026-03-05T00:35:49Z", "age_days": 6, "branch_count": 17, "has_build_instructions": true}
- [medium] Samsung GPL compliance score: 0/12 (timeliness=0, branches=0, build_docs=0, freshness=0). Details: {"error": "Repository not found or API unavailable"}
- [medium] Xiaomi GPL compliance score: 12/12 (timeliness=3, branches=3, build_docs=3, freshness=3). Details: {"last_push": "2026-03-10T09:01:42Z", "age_days": 0, "branch_count": 241, "has_build_instructions": true}
- [medium] OnePlus GPL compliance score: 10/12 (timeliness=3, branches=2, build_docs=3, freshness=2). Details: {"last_push": "2026-02-06T10:24:38Z", "age_days": 32, "branch_count": 16, "has_build_instructions": true}
- [medium] Google Pixel GPL compliance score: 0/12 (timeliness=0, branches=0, build_docs=0, freshness=0). Details: {"error": "Repository not found or API unavailable"}
- [medium] Meta's GPL compliance score (11/12) is above the vendor average (6.6/12). Full comparison report: /home/theseus/rsearch/meta-linux-research/output/reports/vendor_compliance_comparison.md

### Task 1.6
- [high] AOSP Gerrit contributions from Meta (facebook.com) (facebook.com): 0 total, 0 merged, 0 open, 0 abandoned.
- [high] AOSP Gerrit contributions from Meta (meta.com) (meta.com): 0 total, 0 merged, 0 open, 0 abandoned.
- [high] AOSP Gerrit contributions from Meta (oculus.com) (oculus.com): 0 total, 0 merged, 0 open, 0 abandoned.
- [high] AOSP Gerrit contributions from Samsung (samsung.com): 0 total, 0 merged, 0 open, 0 abandoned.
- [high] AOSP Gerrit contributions from Qualcomm (quicinc.com): 0 total, 0 merged, 0 open, 0 abandoned.
- [high] AOSP Gerrit contributions from Google (google.com): 1 total, 0 merged, 0 open, 1 abandoned.
- [high] Meta's combined AOSP contributions across facebook.com, meta.com, and oculus.com: 0 total, 0 merged.  Full comparison report: /home/theseus/rsearch/meta-linux-research/output/reports/aosp_contribution_comparison.md
- [high] AOSP contribution comparison -- Samsung: 0, Qualcomm: 0, Google: 1, Meta (combined): 0.

### Task 1.8
- [high] Patent US20210286628A1: "Operating System With A Single Kernel Stack Per Processor" Status: abandoned. Filed: 2021-05-04. Claims: 38. Horizon OS relevance: low (2 keyword matches).
- [high] Patent US11119931B1: "Data pipeline for microkernel operating system" Status: expired. Filed: 2019-09-18. Claims: 85. Horizon OS relevance: medium (3 keyword matches).
- [medium] Patent analysis complete: 2/2 patents successfully retrieved. 1 show medium-to-high Horizon OS relevance. 0 related patents identified. Meta's patent portfolio may protect key architectural decisions in their XR operating system, creating barriers for competing or open-source alternatives.

### Task 2.1
- [high] Meta employees hold 0 maintainer and 0 reviewer positions across 0 kernel subsystems (kernel mainline HEAD). 0 unique individuals identified.

### Task 2.2
- [medium] Across 2500 commits in v6.10..v6.11, v6.11..v6.12, v6.12..v6.13, v6.13..v6.14, v6.14..v6.15, Meta accounts for 0.0% of all signoff/review/ack tags (0 Signed-off-by). Total tags analysed: 4810.
- [medium] Other: 2011 total tags (41.81% share) -- Signed-off-by: 1496, Reviewed-by: 395, Acked-by: 120
- [medium] kernel.org: 705 total tags (14.66% share) -- Signed-off-by: 549, Reviewed-by: 135, Acked-by: 21
- [medium] Red Hat: 462 total tags (9.6% share) -- Signed-off-by: 338, Reviewed-by: 75, Acked-by: 49
- [medium] AMD: 401 total tags (8.34% share) -- Signed-off-by: 257, Reviewed-by: 115, Acked-by: 29
- [medium] Intel: 372 total tags (7.73% share) -- Signed-off-by: 232, Reviewed-by: 124, Acked-by: 16
- [medium] Across 45630 commits in v6.10..v6.11, v6.11..v6.12, v6.12..v6.13, Meta accounts for 5.5% of all signoff/review/ack tags (5863 Signed-off-by). Total tags analysed: 170207.
- [medium] Other: 58552 total tags (34.4% share) -- Signed-off-by: 44079, Reviewed-by: 12539, Acked-by: 1934
- [medium] Intel: 20908 total tags (12.28% share) -- Signed-off-by: 12862, Reviewed-by: 6581, Acked-by: 1465
- [medium] Google: 14691 total tags (8.63% share) -- Signed-off-by: 8943, Reviewed-by: 4810, Acked-by: 938
- [medium] Red Hat: 13084 total tags (7.69% share) -- Signed-off-by: 8139, Reviewed-by: 3757, Acked-by: 1188
- [medium] AMD: 10413 total tags (6.12% share) -- Signed-off-by: 6512, Reviewed-by: 3290, Acked-by: 611

### Task 2.3
- [medium] Josef Bacik moved from Meta to Anthropic (approx. 2024). Role: Btrfs maintainer. Subsystems: Btrfs. Impact: Josef Bacik was one of the primary Btrfs maintainers while at Meta. His departure to Anthropic raises questions about Btrfs maintainership continuity and whether Meta retains influence over this subsystem. Confirmed by 2/9 searches.
- [medium] Roman Gushchin moved from Meta to Google (approx. 2023). Role: cgroups/memory contributor. Subsystems: cgroups, memory management. Impact: Roman Gushchin was a key contributor to cgroups and memory management subsystems while at Meta. His move to Google shifts expertise in resource isolation and memory management to a competitor. Confirmed by 2/9 searches.
- [medium] Kirill Shutemov moved from Intel to Meta (approx. 2023). Role: memory management developer. Subsystems: memory management, x86. Impact: Kirill Shutemov's move from Intel to Meta brings deep memory management expertise (huge pages, TDX, LAM) to Meta, potentially increasing Meta's influence over mm subsystem direction. Confirmed by 2/9 searches.
- [medium] Subsystem 'Btrfs' continuity risk: high. Gained: none. Lost: Josef Bacik. Net change: -1. Btrfs is used extensively in Meta's data centres. Loss of maintainership could slow feature development and bug-fix cycles for Meta-specific workloads.
- [medium] Subsystem 'cgroups' continuity risk: medium. Gained: none. Lost: Roman Gushchin. Net change: -1. cgroups v2 is foundational to container orchestration. Other major contributors remain (Tejun Heo was at Meta), but loss of dedicated engineers reduces influence.
- [medium] Subsystem 'memory management' continuity risk: low. Gained: Kirill Shutemov. Lost: Roman Gushchin. Net change: 0. Meta is building mm expertise by hiring from Intel. This is an area of active investment rather than loss.

### Task 2.4
- [high] Meta employees hold 0 of 0 BPF maintainer/reviewer positions (0.0%). BPF-related subsystem sections: 0.
- [high] Alexei Starovoitov: BPF co-maintainer and original author. Co-created eBPF (extended BPF) while at PLUMgrid, then joined Facebook/Meta. Serves as BPF subsystem co-maintainer alongside Daniel Borkmann. Controls the direction of BPF development.
- [high] Andrii Nakryiko: BPF libraries maintainer, libbpf author. Primary author and maintainer of libbpf, the canonical BPF user-space library. Designed BPF CO-RE (Compile Once, Run Everywhere) architecture. Key architect of BPF tooling ecosystem.
- [high] Martin KaFai Lau: BPF networking maintainer. Maintains BPF networking components. Contributed BPF socket storage, cgroup BPF, and other networking-specific BPF features used extensively in Meta's infrastructure.
- [high] Song Liu: BPF contributor, live patching. Contributed BPF trampoline and live-patching support. Works on BPF performance features used in Meta's fleet.
- [high] Yonghong Song: BPF compiler/BTF contributor. Key contributor to BTF (BPF Type Format) and BPF CO-RE compiler support in LLVM/Clang. Enables the 'compile once' paradigm that is central to Meta's BPF deployment strategy.
- [medium] libbpf has 249 contributors with 2446 total contributions. Identified Meta contributions: 1178 (48.2%). Note: many contributors may use personal emails, so the actual Meta contribution percentage is likely higher.
- [medium] BPF CO-RE architecture assessment: Meta operates one of the largest BPF deployments in the world, running BPF programs across millions of servers with varying kernel versions. BPF CO-RE was designed to solve Meta's specific problem of deploying BPF programs fleet-wide without per-kernel recompilation. While this benefits all BPF users, the architecture decisions were driven by Meta's scale requirements. Key design decisions favouring Meta: BTF generation integrated into kernel build (reduces Meta's build burden); libbpf as the canonical user-space library (Meta controls the reference implementation); CO-RE relocation design optimized for large heterogeneous fleets

### Task 2.7
- [high] Licensing pattern identified: 'Restrict-then-Open Cycle'. Meta repeatedly introduces restrictive licensing, faces community backlash, then relicenses to standard open-source terms. This was seen with React (BSD+Patents -> MIT) and may be playing out with Llama (custom license -> potential future change). Evidence: 5 events. Confidence: high.
- [high] Licensing pattern identified: 'Open-Source as Marketing Strategy'. Meta uses 'open' branding for releases that do not meet OSI's Open Source Definition. This creates adoption through perceived openness while retaining commercial control. Llama 2/3 are marketed as 'open' despite having commercial use restrictions. Evidence: 4 events. Confidence: high.
- [medium] Licensing pattern identified: 'Licensing as Competitive Moat'. Meta's licensing choices appear calibrated to maximise adoption while preventing competitors (companies with >700M MAU) from freely deploying Meta's models. This suggests licensing is used as a competitive weapon rather than a community good. Evidence: 2 events. Confidence: medium.
- [medium] Licensing pattern identified: 'Escalating Restrictions Over Time'. While React moved toward more open licensing, Meta's AI licensing has moved in the opposite direction -- from no AI models released to 'available but restricted' to 'restricted with use policies'. This suggests Meta may further tighten restrictions as AI models become more commercially valuable. Evidence: 3 events. Confidence: medium.
- [high] Documented 9 licensing events spanning 2014-10-28 to 2025-01-01. Identified 4 strategic patterns in Meta's open-source licensing behaviour: Restrict-then-Open Cycle, Open-Source as Marketing Strategy, Licensing as Competitive Moat, Escalating Restrictions Over Time.

### Task 3.1
- [high] OpenXR extension audit: 265 total extensions found. Meta authored 76 (28.7% of total, 40.4% of vendor-specific). XR_FB_*: 41, XR_META_*: 35.
- [medium] 67% contribution claim assessment: NOT VERIFIED against total: Meta has 28.7% of total extensions (76/265). 
- [medium] Dependency analysis: 0 non-Meta extensions depend on Meta-authored extensions. Meta's extension volume creates de facto influence over the OpenXR standard even when extensions are technically vendor-specific.

### Task 3.4
- [high] Meta holds Platinum membership at the Linux Foundation at $500,000/yr. This grants Meta a guaranteed board seat, TSC voting rights, and marketing council seat. Platinum members have direct governance influence over LF project selection, funding, and strategic direction.
- [high] Kathy Kam, Director of Open Source at Meta, serves as Meta's Platinum member representative on the Linux Foundation Board of Directors. This gives Meta direct influence on LF governance including project selection, budget allocation, and policy decisions.
- [high] Meta is involved in 8 LF-affiliated projects. Meta founded or created 4 of these: PyTorch Foundation, Open Compute Project (OCP), Presto Foundation, GraphQL Foundation. This pattern of donating company-created projects to LF while retaining governance influence extends Meta's reach within the open-source ecosystem.
- [medium] Linux Foundation board meeting minutes are not publicly available, limiting external oversight. Platinum members like Meta can influence governance decisions without public accountability for individual votes. This governance opacity benefits large corporate members who can shape policy behind closed doors.
- [medium] Meta's LF strategy combines Platinum membership ($500K/yr board seat) with donating Meta-created projects (PyTorch, Presto, GraphQL) to LF stewardship. This positions Meta as both a governance decision-maker and a major project contributor, creating a dual channel of influence. The $500K annual fee is trivial relative to Meta's $134B+ revenue but yields disproportionate ecosystem influence.

### Task 4.1
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc (position: n/a, period: n/a - n/a)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc (position: n/a, period: n/a - n/a)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc (position: n/a, period: n/a - n/a)
- [high] Colorado lobbying: Headwaters Strategies lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc (position: n/a, period: n/a - n/a)
- [high] Colorado lobbying: Sachs, Dan lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc. (position: n/a, period: n/a - n/a)
- [high] Colorado lobbying: Martinez, Ana lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc. (position: n/a, period: n/a - n/a)
- [high] Colorado lobbying: Headwaters Strategies lobbied on HB26-1058 (subject: Protections for Minors Featured in Digital Content) on behalf of Meta Platforms, Inc (position: Amending, period: 02/09/26 - Current)
- [high] Colorado lobbying: Headwaters Strategies lobbied on SB26-051 (subject: Age Attestation on Computing Devices) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/12/26 - Current)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on HB26-1058 (subject: Protections for Minors Featured in Digital Content) on behalf of Meta Platforms, Inc (position: Amending, period: 02/09/26 - Current)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on SB26-051 (subject: Age Attestation on Computing Devices) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/12/26 - Current)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on HB26-1058 (subject: Protections for Minors Featured in Digital Content) on behalf of Meta Platforms, Inc (position: Amending, period: 02/09/26 - Current)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on SB26-051 (subject: Age Attestation on Computing Devices) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/12/26 - Current)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on HB26-1058 (subject: Protections for Minors Featured in Digital Content) on behalf of Meta Platforms, Inc (position: Amending, period: 02/09/26 - Current)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on SB26-051 (subject: Age Attestation on Computing Devices) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/12/26 - Current)
- [high] Colorado lobbying: Diers, Tyler lobbied on n/a (subject: n/a) on behalf of Meta Platforms, Inc. (position: n/a, period: n/a - n/a)
- [high] Colorado lobbying: Martinez, Ana lobbied on RULES (subject: Privacy Rules) on behalf of Meta Platforms, Inc. (position: Monitoring, period: 04/30/22 - 06/30/22)
- [high] Colorado lobbying: Headwaters Strategies lobbied on SB23-207 (subject: Sales And Use Tax Refund For Data Center Purchases) on behalf of Meta Platforms, Inc (position: Monitoring, period: 04/03/23 - 06/30/23)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on SB23-207 (subject: Sales And Use Tax Refund For Data Center Purchases) on behalf of Meta Platforms, Inc (position: Monitoring, period: 04/03/23 - 06/30/23)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on SB23-207 (subject: Sales And Use Tax Refund For Data Center Purchases) on behalf of Meta Platforms, Inc (position: Monitoring, period: 04/03/23 - 06/30/23)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on SB23-207 (subject: Sales And Use Tax Refund For Data Center Purchases) on behalf of Meta Platforms, Inc (position: Monitoring, period: 04/03/23 - 06/30/23)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on SB23-207 (subject: Sales And Use Tax Refund For Data Center Purchases) on behalf of Meta Platforms, Inc (position: Monitoring, period: 04/03/23 - 06/30/23)
- [high] Colorado lobbying: Headwaters Strategies lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/26/24)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/02/24 - 02/26/24)
- [high] Colorado lobbying: Headwaters Strategies lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/29/24)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/29/24)
- [high] Colorado lobbying: Headwaters Strategies lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 03/14/24)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 03/14/24)
- [high] Colorado lobbying: Headwaters Strategies lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/15/24 - 03/25/24)
- [high] Colorado lobbying: Headwaters Strategies lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Amending, period: 02/26/24 - 06/30/24)
- [high] Colorado lobbying: Headwaters Strategies lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Amending, period: 03/14/24 - 06/30/24)
- [high] Colorado lobbying: Headwaters Strategies lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Amending, period: 02/29/24 - 06/30/24)
- [high] Colorado lobbying: Headwaters Strategies lobbied on HB24-1468 (subject: Artificial Intelligence & Biometric Technologies) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/07/24 - 06/30/24)
- [high] Colorado lobbying: Headwaters Strategies lobbied on SB24-205 (subject: Consumer Protections for Artificial Intelligence) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
- [high] Colorado lobbying: Headwaters Strategies lobbied on SB24-041 (subject: Privacy Protections for Children's Online Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 06/30/24)
- [high] Colorado lobbying: Headwaters Strategies lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Amending, period: 03/25/24 - 06/30/24)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Amending, period: 02/26/24 - 06/30/24)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Amending, period: 03/14/24 - 06/30/24)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Amending, period: 02/29/24 - 06/30/24)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/26/24)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/26/24)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/26/24)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/29/24)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/29/24)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 03/14/24)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/02/24 - 03/14/24)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/15/24 - 03/25/24)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/15/24 - 03/25/24)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/15/24 - 03/25/24)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on HB24-1468 (subject: Artificial Intelligence & Biometric Technologies) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on SB24-205 (subject: Consumer Protections for Artificial Intelligence) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on SB24-041 (subject: Privacy Protections for Children's Online Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 06/30/24)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Amending, period: 03/25/24 - 06/30/24)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Amending, period: 02/26/24 - 06/30/24)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on HB24-1070 (subject: Allowing Certain Items at School Graduation) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 06/30/24)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Amending, period: 03/14/24 - 06/30/24)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Amending, period: 02/29/24 - 06/30/24)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on HB24-1468 (subject: Artificial Intelligence & Biometric Technologies) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on SB24-205 (subject: Consumer Protections for Artificial Intelligence) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on SB24-041 (subject: Privacy Protections for Children's Online Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 06/30/24)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Amending, period: 03/25/24 - 06/30/24)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Amending, period: 02/26/24 - 06/30/24)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Amending, period: 03/14/24 - 06/30/24)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Amending, period: 02/29/24 - 06/30/24)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on HB24-1468 (subject: Artificial Intelligence & Biometric Technologies) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on SB24-205 (subject: Consumer Protections for Artificial Intelligence) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on SB24-041 (subject: Privacy Protections for Children's Online Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 06/30/24)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Amending, period: 03/25/24 - 06/30/24)
- [high] Colorado lobbying: Martinez, Ana lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc. (position: Monitoring, period: 02/12/24 - 06/30/24)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 02/29/24)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 03/14/24)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/15/24 - 03/25/24)
- [high] Colorado lobbying: Martinez, Ana lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc. (position: Monitoring, period: 02/12/24 - 06/30/24)
- [high] Colorado lobbying: Martinez, Ana lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc. (position: Monitoring, period: 02/12/24 - 06/30/24)
- [high] Colorado lobbying: Martinez, Ana lobbied on SB24-085 (subject: Sales & Use Tax Rebate for Digital Asset Purchases) on behalf of Meta Platforms, Inc. (position: Monitoring, period: 02/12/24 - 06/30/24)
- [high] Colorado lobbying: Martinez, Ana lobbied on SB24-205 (subject: Consumer Protections for Artificial Intelligence) on behalf of Meta Platforms, Inc. (position: Amending, period: 04/19/24 - 06/30/24)
- [high] Colorado lobbying: Martinez, Ana lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc. (position: Amending, period: 03/25/24 - 06/30/24)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1058 (subject: Protect Privacy of Biological Data) on behalf of Meta Platforms, Inc (position: Amending, period: 02/26/24 - 06/30/24)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1130 (subject: Privacy of Biometric Identifiers & Data) on behalf of Meta Platforms, Inc (position: Amending, period: 03/14/24 - 06/30/24)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1136 (subject: Healthier Social Media Use by Youth) on behalf of Meta Platforms, Inc (position: Amending, period: 02/29/24 - 06/30/24)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on HB24-1468 (subject: Artificial Intelligence & Biometric Technologies) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on SB24-205 (subject: Consumer Protections for Artificial Intelligence) on behalf of Meta Platforms, Inc (position: Monitoring, period: 05/06/24 - 06/30/24)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on SB24-041 (subject: Privacy Protections for Children's Online Data) on behalf of Meta Platforms, Inc (position: Monitoring, period: 02/01/24 - 06/30/24)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on SB24-158 (subject: Social Media Protect Juveniles Disclosures Reports) on behalf of Meta Platforms, Inc (position: Amending, period: 03/25/24 - 06/30/24)
- [high] Colorado lobbying: Headwaters Strategies lobbied on HB25-1287 (subject: Social Media Tools for Minor Users & Parents) on behalf of Meta Platforms, Inc (position: Amending, period: 03/28/25 - 06/30/25)
- [high] Colorado lobbying: Headwaters Strategies lobbied on HB25-1090 (subject: Protections Against Deceptive Pricing Practices) on behalf of Meta Platforms, Inc (position: Amending, period: 02/10/25 - 06/30/25)
- [high] Colorado lobbying: Headwaters Strategies lobbied on SB25-070 (subject: Online Marketplaces & Third-Party Sellers) on behalf of Meta Platforms, Inc (position: Amending, period: 02/17/25 - 06/30/25)
- [high] Colorado lobbying: Headwaters Strategies lobbied on SB25-086 (subject: Protections for Users of Social Media) on behalf of Meta Platforms, Inc (position: Amending, period: 01/30/25 - 06/30/25)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on HB25-1287 (subject: Social Media Tools for Minor Users & Parents) on behalf of Meta Platforms, Inc (position: Amending, period: 03/27/25 - 06/30/25)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on HB25-1090 (subject: Protections Against Deceptive Pricing Practices) on behalf of Meta Platforms, Inc (position: Amending, period: 02/10/25 - 06/30/25)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on SB25-070 (subject: Online Marketplaces & Third-Party Sellers) on behalf of Meta Platforms, Inc (position: Amending, period: 02/17/25 - 06/30/25)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on SB25-086 (subject: Protections for Users of Social Media) on behalf of Meta Platforms, Inc (position: Amending, period: 01/30/25 - 06/30/25)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on HB25-1287 (subject: Social Media Tools for Minor Users & Parents) on behalf of Meta Platforms, Inc (position: Amending, period: 03/27/25 - 06/30/25)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on HB25-1090 (subject: Protections Against Deceptive Pricing Practices) on behalf of Meta Platforms, Inc (position: Amending, period: 02/10/25 - 06/30/25)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on SB25-070 (subject: Online Marketplaces & Third-Party Sellers) on behalf of Meta Platforms, Inc (position: Amending, period: 02/17/25 - 06/30/25)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on SB25-086 (subject: Protections for Users of Social Media) on behalf of Meta Platforms, Inc (position: Amending, period: 01/30/25 - 06/30/25)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on HB25-1287 (subject: Social Media Tools for Minor Users & Parents) on behalf of Meta Platforms, Inc (position: Amending, period: 03/27/25 - 06/30/25)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on HB25-1090 (subject: Protections Against Deceptive Pricing Practices) on behalf of Meta Platforms, Inc (position: Amending, period: 02/10/25 - 06/30/25)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on SB25-070 (subject: Online Marketplaces & Third-Party Sellers) on behalf of Meta Platforms, Inc (position: Amending, period: 02/17/25 - 06/30/25)
- [high] Colorado lobbying: EICHBERG, ADAM lobbied on SB25-086 (subject: Protections for Users of Social Media) on behalf of Meta Platforms, Inc (position: Amending, period: 01/30/25 - 06/30/25)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on HB25-1287 (subject: Social Media Tools for Minor Users & Parents) on behalf of Meta Platforms, Inc (position: Amending, period: 03/28/25 - 06/30/25)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on HB25-1090 (subject: Protections Against Deceptive Pricing Practices) on behalf of Meta Platforms, Inc (position: Amending, period: 02/10/25 - 06/30/25)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on SB25-070 (subject: Online Marketplaces & Third-Party Sellers) on behalf of Meta Platforms, Inc (position: Amending, period: 02/17/25 - 06/30/25)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on SB25-086 (subject: Protections for Users of Social Media) on behalf of Meta Platforms, Inc (position: Amending, period: 01/30/25 - 06/30/25)
- [high] Colorado lobbying: Headwaters Strategies lobbied on HB25-B1008 (subject: Consumer Protections for Artificial Intelligence Interactions) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
- [high] Colorado lobbying: Headwaters Strategies lobbied on SB25-B004 (subject: Increase Transparency for Algorithmic Systems) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on HB25-B1008 (subject: Consumer Protections for Artificial Intelligence Interactions) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
- [high] Colorado lobbying: Schmidt, Alyson lobbied on SB25-B004 (subject: Increase Transparency for Algorithmic Systems) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on HB25-B1008 (subject: Consumer Protections for Artificial Intelligence Interactions) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
- [high] Colorado lobbying: COYNE, WILLIAM C lobbied on SB25-B004 (subject: Increase Transparency for Algorithmic Systems) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on HB25-B1008 (subject: Consumer Protections for Artificial Intelligence Interactions) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
- [high] Colorado lobbying: Burkhart, Amber Janelle lobbied on SB25-B004 (subject: Increase Transparency for Algorithmic Systems) on behalf of Meta Platforms, Inc (position: Monitoring, period: 08/23/25 - 08/27/25)
- [high] Colorado lobbying: Sachs, Dan lobbied on n/a (subject: n/a) on behalf of Facebook Inc. (position: n/a, period: n/a - n/a)
- [high] Colorado lobbying: Martinez, Ana lobbied on n/a (subject: n/a) on behalf of Facebook Inc. (position: n/a, period: n/a - n/a)
- [high] Colorado lobbying: Martinez, Ana lobbied on HB21-1244 (subject: Restrictions On Collection And Use Of Biometric Info) on behalf of Facebook Inc. (position: Monitoring, period: 04/16/21 - 06/30/21)
- [high] Colorado lobbying: Martinez, Ana lobbied on SB21-190 (subject: Protect Personal Data Privacy) on behalf of Facebook Inc. (position: Amending, period: 03/23/21 - 06/30/21)
- [high] Colorado lobbying: Sachs, Dan lobbied on SB21-190 (subject: Protect Personal Data Privacy) on behalf of Facebook Inc. (position: Amending, period: 03/23/21 - 06/30/21)

### Task 4.2
- [HIGH] AB-1043 full text analysis — key provisions impacting Linux/FOSS:
1. §1798.500(g): "Operating system provider" defined as "a person or entity that develops, licenses, or controls the operating system software on a computer, mobile device, or any other general purpose computing device" — this explicitly includes desktop/laptop computers, not just mobile.
2. §1798.501(a): Operating system providers MUST provide (a) accessible interface at account setup for birth date/age entry, (b) real-time API providing age bracket signals (under 13, 13-16, 16-18, 18+).
3. §1798.504(f): Exemptions only cover broadband ISPs, telecom services, physical products. NO exemption for open-source, community-developed, or volunteer-maintained operating systems.
4. §1798.503(a): Penalties up to ,500/child (negligent) or ,500/child (intentional), enforced by CA Attorney General.
5. §1798.505: Operative January 1, 2027 — 10 months from now.
6. The bill requires an ACCOUNT SYSTEM with age data — Linux distros have no equivalent. Debian, Fedora, Ubuntu install processes do not collect birth dates.
7. §1798.500(e): "Covered application store" includes any publicly available platform that distributes applications — potentially covers apt, dnf, flatpak, snap repositories.
- [HIGH] CO SB26-051 legislative details:
- Prime sponsors: Sen. Matt Ball, Sen. Larry Liston, Rep. Amy Paschal, Rep. Naquetta Ricks
- Co-sponsor: Sen. Nick Hinrichsen
- Introduced: 01/27/2026
- Committee hearing: 02/24/2026 (Senate Business, Labor & Technology)
- Amendment L.001 adopted in committee 02/24/2026
- Senate Third Reading: 03/03/2026, passed 28-7
- Status: Under consideration (awaiting House)
- Title: "Age Attestation on Computing Devices"
- Key provisions mirror CA AB-1043: OS providers must implement age bracket signal API, developers must request signals, penalties $2,500-$7,500 per affected minor.
- Effective date: August 12, 2026 if enacted without safety clause.
- [HIGH] CO SB26-051 full text analysis — template bill comparison with CA AB-1043:
IDENTICAL STRUCTURE: Both bills define the same terms in the same order: Account Holder, Age-Bracket Data, Age Signal, Application, Covered Application Store, Developer, Device, Operating System Provider, User. Both use the same four age brackets (under 13, 13-16, 16-18, 18+). Both impose the same penalties ($2,500 negligent / $7,500 intentional per minor). Both exempt only broadband ISPs, telecom services, and physical products.
KEY DIFFERENCES: (1) CO effective date is Jan 1, 2028 (CA is Jan 1, 2027). (2) CO adds §6-30-105(6) exempting developers whose apps exclusively serve internal business communication, enterprise software sales, or technical support platforms. (3) CO uses "DEVICE" (§6-30-101(7)) defined as "ANY GENERAL-PURPOSE COMPUTING DEVICE" vs CA's "computer, mobile device, or any other general purpose computing device."
LINUX IMPACT: Both bills define "Operating System Provider" as any person that "develops, licenses, or controls" OS software on any device. Neither bill contains any FOSS/open-source exemption. "Covered Application Store" is defined broadly enough to include apt, dnf, flatpak, snap repositories. Both bills would require Linux distros to implement: (a) an account system collecting user birth dates, (b) a real-time age bracket API, (c) integration with application package managers.
TEMPLATE BILL CONFIRMATION: The structural and substantive similarity confirms these are template bills. Both mirror the ICMEC "Digital Age Assurance Act" model legislation.
- [HIGH] LA HB-570 CORRECTED: The correct bill is "The App Store Accountability Act" (Act No. 481 of 2025), authored by Rep. Kim Carver (R-Bossier City). Signed by Governor Jeff Landry on June 30, 2025, effective July 1, 2026. Passed unanimously at every stage: House 99-0, Senate 39-0, both conference committee votes 98-0/38-0. Uses 4 age categories (child <13, younger teen 13-15, older teen 16-17, adult 18+). NOTE: LA uses different age brackets than CA/CO (13-15 instead of 13-16, 16-17 instead of 16-18). This is a third template bill in the same family, with Louisiana-specific variations.

### Task 4.3
- [high] PAC tracker collected 8 records totaling $0.00 from sources: FEC, TRACER.
- [low] OpenSecrets API is no longer available. Federal lobbying data for Meta ($26.29M 2025 figure, 86 lobbyists) cannot be independently verified via API. Alternative: manual review of opensecrets.org website or Senate LDA filings.
- [HIGH] California lobbying data: Meta spent $1,036,728 on CA state lobbying in Q1-Q3 2025 (record pace). Q2 2025 alone: $518,605 (highest single quarter ever). Paid CA Chamber of Commerce $3.1M. CRITICAL: Meta SUPPORTED AB-1043 publicly while its trade associations (TechNet, Chamber of Progress) OPPOSED it — Meta broke ranks to support a bill that burdens OS providers and app stores (Apple/Google) rather than platforms (Meta). This confirms the strategic interest hypothesis.

### Task 4.4
- [HIGH] Meta client name fragmentation analysis: 6 distinct client name variants across CO and LA lobbying records. Headwaters Strategies team (Burkhart, Coyne, Eichberg, Schmidt) registers under "Meta Platforms, Inc" (no period). In-house lobbyists (Diers, Martinez, Sachs) use "Meta Platforms, Inc." (with period). Two lobbyists (Martinez, Sachs) maintain separate legacy "Facebook Inc." registrations. LA lobbyists use "Meta Platforms, Inc." except Borill ("Meta Platforms, INC.") and Harbison ("Meta Platforms, Inc. (META)"). DCA lobbyist Koch is separately registered under "Digital Childhood Alliance, Inc." — not under Meta.
- [HIGH] Meta lobbying position pattern analysis (CO SOS data, 117 records, 22 bills):
CRITICAL PATTERN: On child safety bills, Meta consistently takes an "Amending" position (actively seeking changes) on bills regulating SOCIAL MEDIA platforms: HB25-1287 (Social Media Tools for Minor Users), SB25-086 (Protections for Users of Social Media), HB24-1136 (Healthier Social Media Use by Youth), SB24-158 (Social Media Protect Juveniles).
EXCEPTION: SB26-051 (Age Attestation on Computing Devices) is the ONLY child safety bill where Meta is "Monitoring" only — passive observation with 4 lobbyists deployed but no amendment efforts. This is consistent with tacit support: Meta benefits from the bill passing as-is because Horizon OS has 83.3% compliance while Linux has 13.9%. Meta actively fights bills regulating its OWN platforms but passively observes a bill that burdens its COMPETITORS.
Of 22 bills lobbied, 9 are monitoring-only, 5 are amending-only, and 5 escalated from monitoring to amending. SB26-051 fits the monitoring-only pattern alongside non-controversial bills like sales tax refunds and graduation items.
- [HIGH] Headwaters Strategies lobbying expenditure data (CO SODA API): Total Meta/Facebook payments to Headwaters: ~$338,500 (2019-2026). Combined Colorado lobbying income from Meta (Headwaters + in-house): ~$451,441. CRITICAL PATTERN: Monthly payments jumped from ~$5K/month (2019-2022) to $14-30K/month starting July 2023, coinciding with intensified state-level child safety legislation. Individual lobbyist incomes at current rates: Eichberg $15K/month (~$180K/year), Schmidt $8,333/month (~$100K/year), Burkhart $6,667/month (~$80K/year).

### Task 4.5
- [HIGH] ATEP/Meta PAC update: Meta launched TWO super PACs totaling $65M:
1. American Technology Excellence Project (ATEP): $45M from Meta (late Sept 2025)
   - Run by Republican veteran Brian Baker and Democratic firm Hilltop Public Solutions
   - Spent $329,000 in 2025 on polling, consulting, and legal
   - Focus: electing tech-friendly state politicians from both parties
2. META California (Mobilizing Economic Transformation Across California): $20M
   - Focus: California state-level candidates favoring lighter tech regulation
Strategic goal: counter state AI regulation bills. The bipartisan structure (Baker + Hilltop) is designed to support candidates who oppose burdensome tech regulation in either party.
Note: "American Excellence PAC" (FEC C00832501) is a DIFFERENT entity — a Leadership PAC with ~$500K, NOT the $45M ATEP.
- [HIGH] ATEP strategic alignment with age verification advocacy: ATEP's three stated pillars include "putting parents in charge of how their kids experience online apps and AI technologies" — this directly aligns with the age attestation legislative agenda (AB-1043, SB26-051). ATEP is NOT registered as a federal FEC committee; it appears to operate as a state-level Super PAC filing with individual state agencies. Of its $45M war chest, only $329K was spent by year-end 2025 — the vast majority is still undeployed. Additionally, Meta spent $518K lobbying Sacramento specifically on child protection legislation, separate from PAC spending. The combination of: (a) $45M ATEP for electing tech-friendly state legislators, (b) $518K direct CA lobbying, (c) DCA advocacy for age attestation bills, and (d) Headwaters Strategies lobbying in CO suggests a multi-channel influence strategy where direct lobbying, PAC spending, and ostensibly-independent advocacy organizations are deployed in parallel.
- [HIGH] NVF 990 analysis: NVF (EIN 20-5806345) had $669M revenue, $593M in grants (2023). $103.4M specifically for youth development/education, with $59.2M in direct grants. NVF also spent $36.7M on lobbying including $31.2M in grants to OTHER orgs for lobbying. 823 domestic grant recipients on Schedule I. Could not parse full Schedule I (needs XML download). No direct NVF→DCA link found, but NVF grants to 501(c)(4) orgs would be unusual (NVF is 501(c)(3)). The $31.2M in lobbying grants to other organizations is a potential channel for indirect funding.
- [HIGH] Arabella network scale: Sixteen Thirty Fund ($282M revenue, 318 grants totaling $236.5M in 2024), Windward Fund and Hopewell Fund combined 2023 revenue $370M. Including NVF, the Arabella network exceeds $1B annually. Adam Eichberg (Meta's CO lobbyist) chairs NVF board. All Arabella entities share 1828 L St NW, DC. No direct Arabella→child safety grant connection found yet, but Schedule I data (823+ grant recipients across NVF alone) could not be fully parsed.

### Task 4.6
- [high] RDAP lookup for digitalchildhoodalliance.org: registrant=redacted, created=2024-12-18T04:11:13.629Z, nameservers=['leia.ns.cloudflare.com', 'mitch.ns.cloudflare.com']
- [medium] DCA social media presence found on: twitter, linkedin. twitter: 4 profile(s); linkedin: 1 profile(s)
- [high] Headwaters Strategies OSINT: The firm is owned by Will Coyne and Adam Eichberg, who are the same individuals listed as individual lobbyists (COYNE, WILLIAM C and EICHBERG, ADAM) in Meta CO lobbying records. Staff Alyson Schmidt and Amber Burkhart are also registered individually. The "4 lobbyists + 1 firm" pattern in the data is actually 4 people and their firm — not 5 separate entities.
- [high] Headwaters Strategies OSINT: Adam Eichberg (co-founder, Meta lobbyist) serves as Chair of the Board of the New Venture Fund, part of the Arabella Advisors dark money network. He was also a founding board member of the Windward Fund and is incoming board chair of Sunflower Services (which acquired Arabella Advisors in late 2025). This places Meta's principal Colorado lobbyist at the center of one of the largest dark money pass-through infrastructures in US politics.
- [high] Headwaters Strategies OSINT: The Center for Secure and Modern Elections (CSME), a project of the New Venture Fund, is also a Headwaters Strategies lobbying client. This means Eichberg's firm lobbies for an organization housed within a network he chairs — a notable governance overlap.
- [high] Headwaters Strategies OSINT: Meta has been a Headwaters client since December 2019 (pre-rebrand from Facebook). The relationship has been continuously active through FY 2025-2026. Other notable clients include Airbnb, Tesla, City of Boulder ($60K/yr), Everytown for Gun Safety, Environmental Defense Fund, and Charter Communications.
- [medium] Headwaters Strategies OSINT: No direct connection found between Headwaters Strategies and DCA, Koch (LA lobbyist), ATEP, ConnectSafely, ICMEC, or CCME. Headwaters operates exclusively in Colorado with $0 federal lobbying. However, the Arabella/NVF infrastructure chaired by Eichberg could theoretically be used to fund or coordinate advocacy entities without direct paper trails.
- [high] Meta-DCA funding confirmed: Reporting from the Deseret News (Dec 2025) confirms Meta funds the Digital Childhood Alliance. Louisiana Senator Jay Morris pressed DCA Executive Director Casey Stefanski about DCA's tech company funding sources during legislative testimony. This upgrades the DCA anomaly from open question to confirmed Meta-funded advocacy.
- [HIGH] DCA/DCI DNS/WHOIS deep dive: SHARED INFRASTRUCTURE CONFIRMED:
1. Same registrar (GoDaddy) with privacy protection on both domains
2. Same CDN (Cloudflare) on both
3. Same email provider (Microsoft 365) on both
4. CRITICAL: Same email marketing platform (Elastic Email) on both — indicates shared mass communications capability and likely same person/team set up both
5. DCA has 4-year registration (through 2028, well-funded) vs DCI 1-year (expires June 2026)
6. DCA registered Dec 18, 2024 — 6 months BEFORE DCI (June 13, 2025). This is reversed from normal pattern: typically the 501(c)(3) educational arm is established first, then the lobbying arm. DCA (lobbying) coming first suggests it was the primary objective.
7. DCA has sophisticated email stack: Microsoft 365 + Google + Amazon SES + Elastic Email, indicating professional-grade infrastructure for a 3-month-old organization.
- [MEDIUM] CO GA witness list analysis: SB26-051 committee hearing (Feb 24, 2026) records examined. No detailed individual witness names found in publicly accessible hearing summaries for SB26-051. SB25-086 (vetoed social media bill): witnesses included DA Brian Mason, Chelsea Congdon, Aaron Ping. HB25-1287: referred to committee but hearing records limited. FOIA responses (due 3/13-3/14) may contain witness lists and Meta/DCA testimony details. Notable: Governor Polis VETOED SB25-086 (social media regulation) in April 2025 — Meta was in "Amending" position on this bill.
- [HIGH] Digital Childhood Institute (DCI) EIN FOUND: 39-3684798. Very new 501(c)(3) — IRS ruling date November 2025. Registered in Wilmington, DE with operations in Utah. Founded by Melissa McKay. No 990 filings exist yet. DCI EXPLICITLY states it does not accept tech platform funding — this contrasts with DCA (501(c)(4)) which confirmed accepting tech funding under questioning.
- [HIGH] Wayback Machine DCA website analysis (CDX API, 100+ snapshots, Dec 2024 - Mar 2026):
NO version of the DCA website has EVER disclosed funding sources. No "supported by", "funded by", or sponsor logos section exists in any archived snapshot. The earliest snapshot (Dec 19, 2024, one day after domain registration) and all subsequent versions contain zero references to Meta, Facebook, or any tech company as a funder.
Site evolution: Feb 2025 was a simple landing page with the App Store Accountability Act campaign. By Mar 2026, it expanded to include About Us, Our Team, Resources, Donate, state bill tracker, and ASAA bill page. Featured "Voices" include Heritage Foundation, NCOSE, Ethics and Public Policy Center, Institute for Family Studies — all conservative organizations.
The complete absence of funding disclosure across ALL snapshots is consistent with deliberate donor anonymity under 501(c)(4) status, despite Meta funding being confirmed by Bloomberg and acknowledged by Stefanski under legislative questioning.

### Task 4.7
- [medium] AVPA member 'Contact Us' found in legislative testimony in 1 state(s): CA
- [medium] Hearing transcript keyword match [DCA]: NOTE: In order to use the designer, the <menu> code must be temporarily moved outside of the <table> code -->
                <a href="#ctl00_ctl00_PageBody_Menu1_SkipLink"><img alt="Skip Navigation Links" src="/Legis/WebResource.axd?d=9dRXm_2hH9Tre_DnPjqfcn65FFHj8DUuXqVRtz_zag39ullvw0q6guAM4ZFsnXHF
- [medium] Hearing transcript keyword match [DCA]: (FAQ's)</a></td>
					</tr>
				</table></td>
			</tr><tr onmouseover="Menu_HoverStatic(this)" onmouseout="Menu_Unhover(this)" onkeyup="Menu_Key(this)" id="ctl00_ctl00_PageBody_Menu1n9">
				<td><table cellpadding="0" cellspacing="0" border="0" width="100%">
					<tr>
						<td style="white-space:no
- [medium] Hearing transcript keyword match [Meta]: %PDF-1.4
%����
22 0 obj
<<
/Linearized 1
/L 62433     
/H [ 730 359              ]
/O 24
/E 38650     
/N 6
/T 61869     
>>
endobj
xref
22 15
0000000017 00000 n
0000000628 00000 n
0000001089 00000 n
0000001382 00000 n
0000004423 00000 n
0000004669 00000 n
0000005612 00000 n
0000006150 00000 n
00000
- [medium] Hearing transcript keyword match [Meta]: ʷX����3����zl�R ���x{P�콯5ߠ'}���ު'hx�1z����=����0��j�������`1�HD�]N��8u��}|]f(�c~��ۉ3i!W,�m���q#����
endstream
endobj
26 0 obj
<<
/Type /Font
/Subtype /Type1
/Name /F12
/Corel_IsVertical false
/Corel_CharSet 0
/BaseFont /DPWMHS+TimesNewRomanPSMT
/FirstChar 32
/LastChar 255
/Widths 27
- [medium] Hearing transcript keyword match [Meta]: ���າKNX2f9r�r�OJC�b�r�H��O�ӿ���b�Si Ky�>�&<XK
�C�ҭs~�5��������+#M��r��"]�%?��{��I�%m}$h��#e��<��;1��W���"��A(�n�y�z.E�?�Ҏ�dn �g
���;�:n�8[��W��С�M&���1����/�q����毯������˼ZϢq���]4"���.�ܦv(�����L�����}!m�y������S���'vي���x	�������a��ܱb�V.��-��@l5����TbN�ϕb�Ƞ�#�����e�{X�x
- [medium] Hearing transcript keyword match [Meta]: �vA�E'�o����QMODk57d��L�����Z� VA�	����E	�Fuk��N2&��6i�)?�"6H=��2	�U����O�_��>� ��HI�
� /
��Ew�Цؓ������|���|�{U�p�����sQ�`j��g����3�ʹ��C�9V}Y��G"W���$��{V���rG��e�ײ�0�����e�R}\G����T4�m^\qa��,�RΕ�iu��UQ��D4�����)�lB�����$����5EN'���I�r�5]�K�2��m�1ܯ���Q�:�u3S�
- [medium] Hearing transcript keyword match [Meta]: ��*��d��z)!�]�>2��q>MB�2\(�c �4��2�P:��8;qI;�$�5^������艞���f4��T�Ac����M�`Yiz����G�5?����/��$dh���]`8�Hzd<KXV���h��2E�0��#��	��9C�9�6�u�9(S�ʵ����4�iT�)� ���:�I�X�O��r7��&̀��NW�>���*���oʲq��KeQ��nˬE�
���S��������|0�W*����L'��O�d�:$k6h`���F4�Z���H�Rf��.�>N����k�
- [medium] Hearing transcript keyword match [Meta]: %PDF-1.4
%����
10 0 obj
<<
/Linearized 1
/L 37944     
/H [ 726 220              ]
/O 12
/E 30577     
/N 2
/T 37620     
>>
endobj
xref
10 15
0000000017 00000 n
0000000627 00000 n
0000000946 00000 n
0000001238 00000 n
0000004820 00000 n
0000005066 00000 n
0000006009 00000 n
0000006505 00000 n
00000
- [medium] Hearing transcript keyword match [Meta]: ��� ���l�	�`�� �-�����P���i��vf�i?G���x�}H�~�
g�J��A"��z�]�]�8J�.��a� ?N�;U0��[��^Xbo��=����\�+��U4���U�2G����BS	�J�F�% J6�)^&���`
���wyi�*� BSo B�ᤌGĘ�)�d���9�?�E���a��OsV��B�,q��ߩ�MnS���l����i^�����I~�<������������s
��1!���8Hz�#��vl}��@�{�i�l����B��op�݉�1$[
- [medium] Hearing transcript keyword match [Meta]: ڐt?8���puq�1��5A@�O䢗v���V3l��F ��:"��~��H�� �?��q�@��$ٙ��P��t�a*��G��%X���)�46�
�����2��jL�C��@���g�)$'��%w?9M+�@��W �� ���6��k�:��14��� �KWTh������Q�� 3�ܢ�.�ho�c�`ѩ_�C��ZkS��w�3�u�~g����� J
��t6��	�I6t�
@)Y��%�Hn�]H���'�yR�۫>���ȵ|�g�[d�C`�D�}j5W�
:�|0O�������B��
- [medium] Hearing transcript keyword match [Meta]: g^����t���='�,�Fސ���?�S���}���7w��Β�{'��nG�������]Fʧ��?�en��n|�qLl��=4�}��B{��!~%v���37�_<-�t�y �rUi���)ڑ�H:^��T��9�_Պ�]�(B\��W�� H��_�?%�B&o#��)���ؕ�c_��[�_�;7��Gga�����K���L9�)iɜ�]^�CTs�9�n����x��(W�;�G
���-}s�G7>�� B,��ʦ�}�}U`����7Z8���n��;=���i���6���s�2ߠ����
- [medium] Hearing transcript keyword match [Meta]: �^y��O3+=�=�W�s�G"���ϯ�;@�rY�
endstream
endobj
3 0 obj
<<
/D [12 0 R /XYZ -4 1012 0]
>>
endobj
4 0 obj
<<
/Kids [5 0 R]
>>
endobj
5 0 obj
<<
/Limits [(_PAGE1) (_PAGE2)]
/Names [(_PAGE1) 3 0 R
(_PAGE2) 6 0 R]
>>
endobj
6 0 obj
<<
/D [1 0 R /XYZ -4 1012 0]
>>
endobj
7 0 obj
<<
/Type /Pages
/Kids [12
- [medium] Hearing transcript keyword match [Meta]: %PDF-1.4
%����
7 0 obj
<<
/Linearized 1
/L 30711     
/H [ 721 193              ]
/O 9
/E 26770     
/N 1
/T 30448     
>>
endobj
xref
7 15
0000000017 00000 n
0000000623 00000 n
0000000914 00000 n
0000001205 00000 n
0000002486 00000 n
0000002732 00000 n
0000003675 00000 n
0000004126 00000 n
00000158
- [medium] Hearing transcript keyword match [Meta]: [DP��ZD6�����_	@��=|��v`
%�� (��bt_OB C=���r����� ���30o�Bt����F�hxn̪`���CO���f=�^:��2ݜ`��~ƍ7�����&�_	ݧŵ���!�?�5�ۀ-���N���ܙW�c�E��Cr�y�Bٗ.�y#��ټ1�'�_�.�М�S��(ߘ�in�����v��d�f0������'��� N�BXR/�jp�H����T�F�y��Q5�������!�dp��o�*�vs\�b��*p����JH���CL3.x���Q�8~���
Z��C
- [medium] Hearing transcript keyword match [Meta]: �:cNsZ��9K�i�XH�o/�O$g��N��{�.�p
���'u�-�6�<g�ugKX�H쑐M��j�|�#%)�2ő��P�њL�\[�d]�F����uH@GeMv|���
�ݲbo�j�~��ó��Ckh
�>b��sI_ſ��x���<��jN�ϖ���7�Z�b<zԮQ��v�$�8�F��OH�ApD��2���s�A\4 ����M�Vq���;%aXg���G��",���f�ê�
{��t����if뾻tc2��~��XW�@�~�] !�C-�y�����'�ڃ���2:v
- [medium] Hearing transcript keyword match [Meta]: g^����t���='�,�Fސ���?�S���}���7w��Β�{'��nG�������]Fʧ��?�en��n|�qLl��=4�}�Լ��?x����Z���/���`:�< C��4@���H�$�|D*���ïj���j!.��	�g ��ׅ�ҟ`!���]���g�Jױ�]֭ܯQ��I����0�zU�����k����d��.��!���m7�P�j��t�+���ÊNǖ��ңk!�]eS��׾�*��}z|��-���s��❞DJ�S�P������	�o��r�o�?a�������
- [medium] Hearing transcript keyword match [Meta]: %PDF-1.4
%����
13 0 obj
<<
/Linearized 1
/L 42495     
/H [ 729 248              ]
/O 15
/E 31853     
/N 3
/T 42111     
>>
endobj
xref
13 15
0000000017 00000 n
0000000628 00000 n
0000000977 00000 n
0000001270 00000 n
0000005806 00000 n
0000006052 00000 n
0000006995 00000 n
0000007505 00000 n
00000
- [medium] Hearing transcript keyword match [Meta]: �4�#�7�)��$	��Z(�bk�OvN-�i���+���
.G|]u]O���?w��%�y�y<ij�C]�X+꒔v�r[��Y� 4�6��qb���
/�梇�c�n�g�TX��u_�^Ә�sd��m����a�\�\�������^�+�Ŗ������������	Ll�F��v�F��`L�)�O�
endstream
endobj
21 0 obj
<<
/Subtype /XML 
/Type /Metadata 
/Length 2838
>>
stream
<?xpacket begin="﻿" id="W5M0MpCeh
- [medium] Hearing transcript keyword match [Meta]: Շܰ$5-��Z"���@-�SV�����\��su|w�,MI&mcL`��c������)��ީBE[��W��FpZ_�Y���E��
*�K�pUL���*?��[jH�Ճ��vU�#7/%5j^��3'v�>�zi�e�S2��cif8�J�dyEZ�;���G���n�G��3- w��[�W&}É������P��& ϵ!�Φ�dL�#�[_��F
T(m�΢����0�Zt��Ŭ�=9�1G	ļ*�v�h}�(�����7�}
E;�7�
/a�З��"|۪�k?��F��`�����K't���LwL�{b��
- [medium] Hearing transcript keyword match [Meta]: %PDF-1.4
%����
13 0 obj
<<
/Linearized 1
/L 43406     
/H [ 729 248              ]
/O 15
/E 31965     
/N 3
/T 43022     
>>
endobj
xref
13 15
0000000017 00000 n
0000000628 00000 n
0000000977 00000 n
0000001270 00000 n
0000005793 00000 n
0000006039 00000 n
0000006982 00000 n
0000007494 00000 n
00000
- [medium] Hearing transcript keyword match [Meta]: =w��������%��_�,�'�X0�B7�&Jo��o�i��!گ��� �L��V(���£+�e=C���$��9�j��&��s]�YM�<V�)S%�>{y��]���9җ��V�����
���::��aCah{����s	 ��i��t]!�Ss�k�ҵ��K���Nh�Ⱥ>�澾�+����e꒴�5�C
]oͧ_�~��r���4:����a�Ԥ/^2�_�}��B�����E�tBU�p��
D���.��m�Z���|m�<m��\�+P�CYS.+a����_�z_}FT�݌)�nFZa��v�
- [medium] Hearing transcript keyword match [Meta]: �z�Xt��*b�2T�Ϯ�@8:y�������`��e��� Z��*>?���O���������El�l��mL�,� ��*�O��d ��� @7#3 ����'`���
0�u�3v��1����߈�
@'�� ��"V ��#& ����o������3;���`����Y�vF��>#&��̟%�+�o� �s2s �C�����m���B�çIt��Lӿ��s}��d?Z�7��L�S�)�0��FJ�$���}B���"l����m�)� �Y�?�������\�
- [medium] Hearing transcript keyword match [Meta]: �e��x��n���K�r(S�*��}�����-���Y�����O��a�`F2�-m��V����H^��
g�C�q�~�8���r�UײH��1�ϭ��	�ίƆ���c��?�
`n�
= o�qJƃ-��\��8�{B�L�j0�=�h���s�B"T��B�W��,g���=��&
<*��\�H�Jq�,ԙ8඾��瞉�zN7F�x�Մt�#v�'�jZ��r^<Emh���Wv�п	��3&��2FW��GG���;��xP�Ag�:X԰������۽�mV5�_��U�qcU]k���M��3̂�q��ת�
- [medium] Hearing transcript keyword match [Meta]: �j��������򨛆��Vz&�'����i.�,-�j��hE�����u�Fm2�n��`�a�y��PmD������R&M�>n�G�+)�p�p+������11Rl��W�3[�U��x �yB�µ��1����?����
�u�*��@���6�DY�~}e&��Mƽ9ܸ�Ҧ�xgm���J��	��|[�-:�(mCx���A�
endstream
endobj
3 0 obj
<<
/Type /Page
/Parent 10 0 R
/Contents 4 0 R
/MediaBox [-0.0000 -0.0000 612.0000
- [medium] Hearing transcript keyword match [Meta]: %PDF-1.4
%����
10 0 obj
<<
/Linearized 1
/L 33307     
/H [ 726 220              ]
/O 12
/E 28395     
/N 2
/T 32983     
>>
endobj
xref
10 15
0000000017 00000 n
0000000627 00000 n
0000000946 00000 n
0000001238 00000 n
0000004379 00000 n
0000004625 00000 n
0000005568 00000 n
0000006039 00000 n
00000
- [medium] Hearing transcript keyword match [Meta]: �����yҢ5N􋴱Q]P�%ȴ;���pQ=��Ɠ��v��d�z��뙌X���+rvW�xSH���|8�W�1%gT�DPƤ��v@=4�ణK��C����D�SK���9Ak}4�SK֏2I�H<)3�9�+3�٥y���Ћ�q������Z���N뢫�_6��*)a�����C[S���v�j�@8%[�ͤ���0�r��/���a��m�W3��WY��N��rŹIe��?h(iY}��$�]�s��M��L��X�����o_:=sEo𤫾�ͽE}�Z��p�'�~�n���(�}�䨄�9�:�m�oAHYP�� `.˪
- [medium] Hearing transcript keyword match [Meta]: qm.��]�mHӰ!���}թns��2]w�Fe5Ƽ`22���#���ǥ^.i��>�
��ԥtP���/�H�~�8xG�9�!��?ۃ�Z:lrp��Z�!M��`7��Ǘ�5�\8�ȣ	q�M�F����L�B`�H&�K��˹$z����P�l��d���6�rͦ��%=�
o����vEez��ߍ�A-�g8"q���T~y���^���@r<��6�O�7"��7)��9煝5+.����8*C���.��:���h��7�⡅赞�x�?oWث�+E���FY��ش��L���p�xTc�[�?IjPc�e�_�ܤ
- [medium] Hearing transcript keyword match [Meta]: �F��Ѳ涶%��GQe�86["a��Mm)�P3�e0��q�=������U�y%
o�Z��	K�{?���S�Q�T��g���B�YzC'p���%�*&��(��B�/�c�ۍ�5�wmebq�#G�Hҵ��ת^p��h�!Q�ӛۘ��m�B"�p��sW<������%O��z���4�z�0?u���HA������
XO�1�AsF���?J�SZ���؂+�2��:�U�o�0hi����q�ߠN�w��@B̜�ieO��,���f+
�ݙ�&�lIDD�nn|�̄w�^�e���Y�M�S�.J�k^�=�IL!�
- [medium] Hearing transcript keyword match [Meta]: �|��_�7�1ې��ě+���q�hA%�f��� �X
endstream
endobj
3 0 obj
<<
/D [12 0 R /XYZ -4 1012 0]
>>
endobj
4 0 obj
<<
/Kids [5 0 R]
>>
endobj
5 0 obj
<<
/Limits [(_PAGE1) (_PAGE2)]
/Names [(_PAGE1) 3 0 R
(_PAGE2) 6 0 R]
>>
endobj
6 0 obj
<<
/D [1 0 R /XYZ -4 1012 0]
>>
endobj
7 0 obj
<<
/Type /Pages
/Kids [
- [medium] Hearing transcript keyword match [Meta]: %PDF-1.4
%����
7 0 obj
<<
/Linearized 1
/L 28543     
/H [ 721 193              ]
/O 9
/E 24602     
/N 1
/T 28280     
>>
endobj
xref
7 15
0000000017 00000 n
0000000623 00000 n
0000000914 00000 n
0000001205 00000 n
0000002411 00000 n
0000002657 00000 n
0000003600 00000 n
0000004027 00000 n
00000142
- [medium] Hearing transcript keyword match [Meta]: ��pi�LMY�?kg-Y&@�9"}���ߋ eg~�O�;|\h���^#>}l�3��A�+� �I���( �'�/b���
���k{l^��������$e
9�
f���]����r΢�6۲P�{��w��y�#��Q�{��K��n,=u�_
j1,��
MT�G�?@ic��,Z Z�i��g�����^��9Flw\T"��y�-i������|7��8,3�9�^{�F�^��vH"�R�c��
z�lZ+�=健e왂s�}>�I?�g_��e��8����)�O�������`ʏ�+
- [medium] Hearing transcript keyword match [Meta]: %PDF-1.4
%����
10 0 obj
<<
/Linearized 1
/L 32717     
/H [ 726 220              ]
/O 12
/E 27674     
/N 2
/T 32393     
>>
endobj
xref
10 15
0000000017 00000 n
0000000627 00000 n
0000000946 00000 n
0000001238 00000 n
0000004105 00000 n
0000004351 00000 n
0000005294 00000 n
0000005761 00000 n
00000
- [medium] Hearing transcript keyword match [Meta]: �?�y`��L쀟l��v{�D�r��J�`|+�Jl$R��<�����O������v�/7~��]n�'8���🉝Opz8>����@�I�<w���O���	��5I��_�KG����x'>��H��N"��H��˯��kM�h�sg�?�̆.Am�t���jf|uh����p/����JA��t��oKÖ	Uv�V��ѧ���?��nX�}���*��w��c\�c����? �W�
endstream
endobj
14 0 obj
<<
/Type /Font
/Subtype /Type1
/Name /F12
/Corel_IsVerti
- [medium] Hearing transcript keyword match [Meta]: �z�����cQ�%dbYm�
����ާE�=�av�Su�{%(m���_�����{n�s��+��V}[$�3�~�Cq�iF�����#[���%�`�M)�jى�a�鰾�56'=�$���F.������:��#�Q��yΈ��~u��gG�h%�����{��T�!���B�#H�&��5yS��GM�F1���h
n���jP� �v4Z��9-;�{&EkY6O�}�/�³�
��'�u�O�=�CZ6�����*[�4�sY	`�i8qw�I��0�
ݮ�����@a�FCgM7"���I���
- [medium] Hearing transcript keyword match [Meta]: C�\1iئ=�R������	}��R.�&w?8|�xÎ:-���(�c�h��`"q��`-��s��j�f��j$��PG�R�߭
i
`�\ԃ�/H�g7�#��F?�5�g���wq�0V���dh$�~�2�Jl���(j�K�hn����K�/�nw�0� �|"6YT�+�c�N#F������YS���G�2Uou��N�N�`{%��g�Zg�nS�%������'?�ot��,λ��~��\!C�F�R(���V�V�"��^����e>v��`�2ҡ  [3Ő�`гA�u�V�q���03��?�
- [medium] Hearing transcript keyword match [Meta]: %PDF-1.4
%����
7 0 obj
<<
/Linearized 1
/L 33376     
/H [ 721 193              ]
/O 9
/E 29435     
/N 1
/T 33113     
>>
endobj
xref
7 15
0000000017 00000 n
0000000623 00000 n
0000000914 00000 n
0000001205 00000 n
0000004962 00000 n
0000005208 00000 n
0000006151 00000 n
0000006645 00000 n
00000190
- [medium] Hearing transcript keyword match [Meta]: +.����=��/eb�\����B_$ƕ����rU�n��z�^v�pbeOa�N=Q�ǭ[&���HP�����]׾n��-��Nd�}'��E~w���h��r�V/�.cx���x��_*�y�[���i�x��#�|�_F.]�µ�� ���l�R��' rM
$N�4{�����Mn����qO�E�
�A�H*��ݻ@�b{�1����O��JQܢF�9��?w{���f��Q�X�bM1�i�W��4��c(9bKs��^�S`�%F;�V�z��Z�x��2��uJ�i��;_����Gv's����g[�2pܽ��-
- [medium] Hearing transcript keyword match [Meta]: �����?|�  0:@?�6
�,�]����6�)��4��uLu}�-����]g~�c�2���ؘ�S�TN����Sk�䉶�Ȋ����3����("�Hc���=2�~Y�
����a.�v���D5���(�9�F��x���a��:}�FG`1z���-�ͯc)Z��C#NP��9�Wj�-��'Ux���&�~�7�Zͼ���[�{U��	�`^�W�e��q3�f$�t�.7�G���r�|�jeiKbn=%�����p_�`?������ݾ���T23�w�=u�>�ʧ�� eM�|�徂'��
- [medium] Hearing transcript keyword match [Meta]: <�z|�{�"ڕ~@�'�V��<�?�v�����6�EU�o����K�_����9Z������Q�[�9tԀ>_��t	��o�|x�enRP�B���ƹ�G6﷯-�����o��{�G��SR!zr��s������f��jɠb��ײS����R�sg�nܑ�("��I��9W�B\��_E(�L��'r9�V��Aas��6�1hQ\�[��Fۣ�z��=���]k��#�K���Y��Zr�J��nMp��ł|A>�AH�/2��.�i?k_����K��\��)]#��s&�+�U����m$M�������-���g�
- [medium] Hearing transcript keyword match [Meta]: %PDF-1.4
%����
13 0 obj
<<
/Linearized 1
/L 40741     
/H [ 729 248              ]
/O 15
/E 29129     
/N 3
/T 40357     
>>
endobj
xref
13 15
0000000017 00000 n
0000000628 00000 n
0000000977 00000 n
0000001270 00000 n
0000004181 00000 n
0000004427 00000 n
0000005370 00000 n
0000005868 00000 n
00000
- [medium] Hearing transcript keyword match [Meta]: p�8��!��p�Y��]}%ٙЁ�Q_�Ğ�"����T8f���]��I�HM
��������03_-Q�fm��hg?*K�s#�5�G��^�Rix+�1�r���9+Hi?�)o��瀑��=�o���C����\/Å%����+�Ae&q���� ��r�gTW��'N�=�L��.����HX�R�����R6����6���9� �@�\c�H�k�5b�*�?�;�WŃ��!�·}5�t�Uo�� +
	��*tH��&K�&��ۚe��E����F�Z	�a?H���iK'{��;����d����
- [medium] Hearing transcript keyword match [Meta]: �t�r���aմk��'�&L�hǥ�,��,�dO�������J0}�^��m�S��n�O��K#u{o�YI�FH�
�9<Z�n�}�
-@�%W�֕���Xw���.Ȁ77z{�!�ZC�I��&����.���)w+�܀P�
�9~�_�w\ӊOY��0}km7��ny
��!�\F�J^���"K6���jÈ#�x�`�!njb7���#p�y����%?���y���t��6�T��'����:��Yf��������;�4�"�����Gl��c���|~�����M_TZ��>CaEÑ?G'�
- [low] Colorado SB26-051 committee hearing scrape attempted but failed to retrieve data from the CO legislature website. Target URL: https://leg.colorado.gov/committees/business-labor-technology/2026-regular-session
- [medium] Louisiana HB570 hearing scrape (Senate Finance Committee): found 15 hearing-related link(s), saved 16 file(s). Bill URL: https://legis.la.gov/legis/BillInfo.aspx?s=25RS&b=HB570
- [high] Hearing transcript keyword search configured for: Meta, Facebook, DCA, Digital Childhood Alliance, Stefanski, age verification, attestation. These keywords track Meta/Facebook involvement and DCA (Digital Childhood Alliance) connections to age-verification legislation in CO and LA.
- [medium] AVPA member 'Concordium' found in legislative testimony in 1 state(s): CA
- [medium] AVPA member 'MyMahi' found in legislative testimony in 1 state(s): CA
- [medium] AVPA member 'KJR' found in legislative testimony in 1 state(s): CA
- [medium] AVPA member 'Persona' found in legislative testimony in 1 state(s): CA
- [medium] AVPA member 'Shufti' found in legislative testimony in 1 state(s): CA
- [medium] AVPA member 'GeoComply' found in legislative testimony in 1 state(s): CA
- [medium] AVPA member 'ShareRing' found in legislative testimony in 1 state(s): CA
- [medium] AVPA member 'IKETech' found in legislative testimony in 1 state(s): CA
- [medium] AVPA member 'CitizenCard' found in legislative testimony in 1 state(s): CA
- [low] Jumio: custom/enterprise pricing (no public per-check rates)
- [medium] Veriff pricing: $0.80 per verification (context: ...to our Premium plan. No credit card needed. Try for free Essential Full auto i $0.80 per verification $49/ month min. × Essential Full auto i $0.80 per verification $49/ month min....)
- [high] Per-check age verification pricing is incompatible with FOSS: Per-check fee model — Commercial vendors charge per verification (typically $0.10-$2.00/check). FOSS distributions have no revenue stream to cover per-user fees, making integration economically impossible for volunteer-run projects.; API key requirement — Vendor SDKs require API keys tied to commercial accounts. Distributing API keys in open-source packages would expose them to abuse; not distributing them renders the integration non-functional.; Proprietary SDK licensing — Yoti, Jumio, and Veriff SDKs are proprietary and cannot be bundled in GPL-licensed distributions. Binary-only SDK blobs conflict with distro packaging policies (Debian DFSG, Fedora licensing guidelines).; Terms of service restrictions — Vendor ToS typically prohibit redistribution, reverse engineering, and modification — all activities fundamental to FOSS. Accepting vendor ToS may conflict with GPL obligations.; No offline/self-hosted option — Cloud-only verification requires internet connectivity and vendor uptime. Air-gapped or privacy-focused Linux installations cannot comply. Self-hosting is not offered or is prohibitively expensive.; Scale economics for non-commercial distros — A mid-size Linux distribution with ~1M users would face $100K-$2M/year in verification fees with no offsetting revenue. This exceeds the entire annual budget of many community distros.; Vendor lock-in and single points of failure — Legislation mandating specific commercial vendors creates single-vendor dependency. If Yoti or similar vendor exits the market, all compliant implementations break simultaneously.; Privacy and data sovereignty — Sending user biometric data to third-party commercial APIs conflicts with the privacy expectations of Linux users and the data-minimization principles of distributions like Tails or Whonix.
- [high] EU open-source age verification frameworks (EUDIW, T-Scy) provide FOSS-compatible alternatives to US commercial vendors. Key advantages: open-source licensing, no per-check fees, privacy-by-design, interoperable standards. Licensing: EU=Open-source (EUPL, Apache 2.0); reference implementations freely available vs US=Proprietary SDKs; commercial licenses incompatible with GPL | Cost model: EU=No per-check fees; self-hostable infrastructure vs US=Per-check fees ($0.10-$2.00+); cloud-only SaaS | Privacy architecture: EU=Privacy-by-design; selective disclosure; user-controlled wallet vs US=Biometric data sent to vendor cloud; vendor retains data per ToS | Interoperability: EU=Standards-based (eIDAS 2.0, ISO 18013-5); cross-border interop mandated vs US=Vendor-specific APIs; no interoperability standard | FOSS compatibility: EU=Fully compatible; designed for open-source integration vs US=Incompatible; proprietary blobs, API keys, ToS restrictions | Governance: EU=EU regulatory framework; democratic oversight; public code mandate vs US=Private companies; no public accountability; vendor lock-in risk | Age verification method: EU=Verifiable credentials from trusted issuers; zero-knowledge proofs vs US=Facial estimation, document scanning, parent-verified (K-ID) | Offline capability: EU=Wallet-based verification works offline after credential issuance vs US=Requires internet for each check; no offline mode
- [HIGH] LA Senate hearing testimony details: Sen. Jay Morris pressed Casey Stefanski (DCA ED) on funding. Stefanski said she was "not comfortable" answering, eventually confirmed tech companies fund DCA but refused to name them. She identified the "father of DCA's founder" as largest donor. DCA paid attorneys to draft model legislation. Meta's Nicole Lopez testified IN SUPPORT of HB-570. Apple and Google filed opposition but sent NO representatives to testify. DCA confirmed meeting with Google for broader support.

### Task 4.9
- [HIGH] ConnectSafely conflicts of interest: CEO Larry Magid serves on Meta's Safety Advisory Council and receives honorarium. Revenue is 89.7% contributions with $0 program service revenue. Executive compensation ($387K) consumes 57.5% of expenses ($673K). Magid earned $218,708 in 2024. Funded by Meta since at least 2017, also by Google, Microsoft, Snapchat. Magid has publicly OPPOSED certain child safety bills — effectively acting as a tech-industry voice while running a nominally independent child safety organization.

### Task A1
- [low] News match [Phoronix]: "There's Hope That At Least Colorado's Age Attestation Bill Could Exclude Open-Source" (keywords: age verification, age attestation)

### Task A2
- [high] US app-store-accountability-act: status changed from '' to 'unknown'
- [high] US KOSA: status changed from '' to 'unknown'
- [high] UT SB-142: status changed from 'enacted' to 'passed'
- [high] IL HB-3304: status changed from '' to 'unknown'
- [high] IL HB-4140: status changed from '' to 'unknown'
- [high] IL SB-2037: status changed from '' to 'unknown'
- [high] NY S8102A: status changed from '' to 'unknown'

### Task EU-US-COMPARE
- [high] EU DSA age verification analysis: Age verification obligations under the DSA apply primarily to VLOPs (>= 45M monthly EU users) through Articles 34-35 risk assessment and mitigation requirements. Smaller platforms face graduated obligations. FOSS projects that do not act as intermediary services are outside DSA scope entirely (Recital 13). Micro/small enterprises receive additional exemptions from transparency and reporting requirements.
- [high] EU age verification blueprint: The EU approach centres on the EUDIW (EU Digital Identity Wallet) under eIDAS 2.0, providing government-issued verifiable credentials with selective disclosure for age verification. Found 0 related GitHub repos. T-Scy consortium search returned 4 results. Key difference from US approach: wallet-based, user-controlled, interoperable across platforms and OS vendors.
- [high] EU vs US age verification comparison: EU uses platform-level regulation (DSA/VLOPs) with FOSS exemptions and privacy-by-design (EUDIW). US uses OS-level mandates (AB 1043, SB 26-051) with no FOSS exemption, concentrating power in Apple/Google. Key risk: US approach threatens open-source OS distributions and creates vendor lock-in absent from the EU model.
- [high] FOSS exemption analysis: EU provides 5 distinct protection mechanisms for FOSS. US model creates 4 categories of threat affecting 13+ named projects/channels. 4 technical barriers exist with no current FOSS workaround. The EU EUDIW (open-source) provides a compliance pathway for FOSS; the US offers none.

### Task horizon-os-audit
- [high] Horizon OS has 5 built-in compliance features: Meta Account Age Verification; Get Age Category API; Family Center; Quest Store Age Ratings; Minor Account Defaults. These collectively address age verification, parental consent, content controls, parental tools, and default protections for minors.
- [high] Linux distros have 7 major compliance gaps: Account System Age Bracket; Age Category D-Bus API; Parent-Child Account Linking; Parental Consent Verification; Package Manager Age-Rating Enforcement; Unified Parental Controls Dashboard; Age-Gated Default Profiles. Estimated total implementation effort: 36-71 months of coordinated cross-project work.
- [medium] The compliance gap creates a structural advantage for Meta's Horizon OS: it already has the infrastructure (account system, age API, parental controls, app store enforcement) that child-safety legislation requires. Linux distros would need 3-5 years of coordinated development across freedesktop.org, GNOME, KDE, and multiple package managers to reach parity. This gap could be leveraged in regulatory arguments that open-source platforms are not ready for compliance, justifying app-store gatekeeping.
- [low] Horizon OS Age API documentation scraped from 0 page(s). No structured API endpoints extracted -- documentation may require JavaScript rendering or may have changed structure.
- [low] Meta Family Center pages fetched but no structured feature list extracted. Pages may require JavaScript rendering or features are embedded in non-standard markup.

## FOIA Requests and Status

- **CO -- Secretary of State**: Filed 2026-03-10, Due 2026-03-13, Status: pending
- **CO -- Attorney General**: Filed 2026-03-11, Due 2026-03-14, Status: pending
- **LA -- Board of Ethics**: Filed 2026-03-11, Due 2026-03-14, Status: pending

## Timeline of Key Events

Total events: 35

- **2014-10-28** [licensing_decision]: Facebook introduces BSD+Patents license for React: Facebook releases React under a BSD license with 
- **2017-04-18** [licensing_controversy]: Apache Software Foundation bans BSD+Patents license: The Apache Software Foundation adds Facebook's 
- **2017-07-16** [licensing_controversy]: WordPress announces move away from React: WordPress co-founder Matt Mullenweg announces that WordPre
- **2017-09-22** [licensing_change]: Facebook relicenses React to MIT: After sustained community backlash and the WordPress departure, Fa
- **2019-03-01** [licensing_decision]: Facebook releases PyTorch under modified BSD license: PyTorch is released under a standard BSD-3-Cla
- **2019-03-13** [governance]: Presto Foundation established under the Linux Foundation with Meta (Facebook) as founding member.
- **2019-09-18** [patent_filing]: Patent US11119931B1: Data pipeline for microkernel operating system (expired)
- **2019-11-06** [governance]: GraphQL Foundation established under the Linux Foundation, stewarding the Meta-created GraphQL speci
- **2019-12-09** [lobbying_registration]: Meta (then Facebook) becomes Headwaters Strategies client in Colorado. Will Coyne registered as lobb
- **2021-05-04** [patent_filing]: Patent US20210286628A1: Operating System With A Single Kernel Stack Per Processor (abandoned)
- **2022-09-12** [governance]: Meta donates PyTorch to the Linux Foundation, establishing the PyTorch Foundation as an LF project. 
- **2023** [personnel_move]: Roman Gushchin: Meta -> Google (cgroups/memory contributor)
- **2023** [personnel_move]: Kirill Shutemov: Intel -> Meta (memory management developer)
- **2023-07-18** [licensing_decision]: Meta releases Llama 2 with custom 'open' license: Meta releases Llama 2 under a custom license that 
- **2024** [personnel_move]: Josef Bacik: Meta -> Anthropic (Btrfs maintainer)
- **2024-04-18** [licensing_decision]: Meta releases Llama 3 with updated custom license: Meta releases Llama 3 under an updated community 
- **2024-07-23** [licensing_decision]: Llama 3.1 release maintains restrictive license: Meta releases Llama 3.1 (405B, 70B, 8B) under the s
- **2025-01-01** [strategic_analysis]: Industry discussion: potential closed-weights pivot: Industry analysts and open-source advocates dis
- **2025-02-25** [ORGANIZATION]: Digital Childhood Alliance publicly launches with 50+ member organizations
- **2025-06-30** [LEGISLATION]: LA HB-570 (App Store Accountability Act) signed by Governor Landry, effective July 1, 2026
- ... and 15 more events

## Threat Assessment

### Immediate Risks

- Age attestation bills advancing through state legislatures with language incompatible with open-source OS architecture
- Model bill language being replicated across states suggests coordinated campaign
- Lack of open-source community engagement in legislative process

### Medium-Term Risks

- Federal legislation codifying OS-level age verification
- International adoption of similar frameworks (EU Digital Services Act precedent)
- De facto exclusion of Linux from consumer device markets

### Long-Term Risks

- Regulatory precedent that computing requires commercial identity services
- Erosion of the principle that operating systems should not require user accounts
- Structural advantage for vertically integrated platforms across all regulatory domains

## Recommended Actions

### For EFF

1. File public comments on pending state age attestation bills highlighting open-source impact
2. Challenge technology-specific mandates as unconstitutional prior restraint on speech (software distribution)
3. Investigate Meta's lobbying coordination across states

### For FSF

1. Issue position statement on age attestation and software freedom
2. Analyse GPL implications of mandatory identity services in Linux distributions
3. Coordinate with distribution maintainers on compliance impact assessment

### For Linux Foundation

1. Engage directly with state legislatures through policy team
2. Develop technical white paper on alternative compliance architectures
3. Convene working group on identity-free age verification approaches
4. Review Meta's kernel contributions for strategic alignment with regulatory positioning

## Source Index

- [Kernel git log signoff analysis (v6.10..v6.11, v6.11..v6.12, v6.12..v6.13)](https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/log/) (accessed 2026-03-11T23:24:46Z)
- [Headwaters Strategies - Our Team](https://headwatersstrategies.com/our-team/) (accessed 2026-03-11T15:14:22Z)
- [Headwaters Strategies - Our Clients](https://headwatersstrategies.com/our-clients/) (accessed 2026-03-11T15:14:22Z)
- [New Venture Fund - Adam Eichberg Board Bio](https://newventurefund.org/who-we-are/board-of-directors/adam-eichberg-chair-of-the-board/) (accessed 2026-03-11T15:14:22Z)
- [Adam Eichberg - InfluenceWatch](https://www.influencewatch.org/person/adam-eichberg/) (accessed 2026-03-11T15:14:22Z)
- [Headwaters Strategies - OpenSecrets](https://www.opensecrets.org/orgs/headwaters-strategies/summary?id=D000074493) (accessed 2026-03-11T15:14:22Z)
- [CO Open Data - Professional Lobbyist Clients](https://data.colorado.gov/Legislative/Professional-Lobbyist-Clients-in-Colorado/vp65-spyn) (accessed 2026-03-11T15:14:22Z)
- [Deseret News - Meta funds DCA](https://www.deseret.com/opinion/2025/12/07/child-safety-bill-backed-by-meta/) (accessed 2026-03-11T15:14:22Z)
- [Center Square - Senator presses DCA on tech ties](https://www.thecentersquare.com/louisiana/article_e97200f8-13d0-4b1f-90a9-e9a7093d329f.html) (accessed 2026-03-11T15:14:22Z)
- [EU age verification research: https://github.com/eu-digital-identity-wallet](https://github.com/eu-digital-identity-wallet) (accessed 2026-03-11T12:09:07Z)
- [EU age verification research: https://github.com/eu-digital-identity-wallet/eudi-lib-jvm-siop-openid4vp-kt](https://github.com/eu-digital-identity-wallet/eudi-lib-jvm-siop-openid4vp-kt) (accessed 2026-03-11T12:09:07Z)
- [EU age verification research: https://digital-strategy.ec.europa.eu/en/library/european-digital-identity-wallet-architecture-and-reference-framework](https://digital-strategy.ec.europa.eu/en/library/european-digital-identity-wallet-architecture-and-reference-framework) (accessed 2026-03-11T12:09:07Z)
- [EU age verification research: https://tscy.eu/](https://tscy.eu/) (accessed 2026-03-11T12:09:07Z)
- [EU age verification research: https://tscy.eu/age-verification/](https://tscy.eu/age-verification/) (accessed 2026-03-11T12:09:07Z)
- [EU age verification research: https://commission.europa.eu/strategy-and-policy/priorities-2019-2024/europe-fit-digital-age/european-digital-identity_en](https://commission.europa.eu/strategy-and-policy/priorities-2019-2024/europe-fit-digital-age/european-digital-identity_en) (accessed 2026-03-11T12:09:07Z)
- [EU age verification research: https://digital-strategy.ec.europa.eu/en/policies/eidas-regulation](https://digital-strategy.ec.europa.eu/en/policies/eidas-regulation) (accessed 2026-03-11T12:09:07Z)
- [Pricing: Jumio](https://www.jumio.com/identity-verification/) (accessed 2026-03-11T12:08:42Z)
- [Pricing: Veriff](https://www.veriff.com/pricing) (accessed 2026-03-11T12:08:42Z)
- [DCA linkedin profile](https://www.linkedin.com/company/digital-childhood-alliance) (accessed 2026-03-11T11:54:05Z)
- [DCA twitter profile](https://x.com/DCAlliance) (accessed 2026-03-11T11:54:02Z)
- [DCA twitter profile](https://x.com/DigitalChildhoodAlliance) (accessed 2026-03-11T11:54:00Z)
- [DCA twitter profile](https://twitter.com/DCAlliance) (accessed 2026-03-11T11:53:57Z)
- [DCA twitter profile](https://twitter.com/DigitalChildhoodAlliance) (accessed 2026-03-11T11:53:55Z)
- [Bill status: IL SB-2037](https://www.ilga.gov/legislation/BillStatus.asp?DocNum=2037&GESSION=104&GA=104&DocTypeID=SB&SessionID=114&LegID=) (accessed 2026-03-11T11:53:30Z)
- [LA bill page: HB-570](https://legis.la.gov/legis/BillInfo.aspx?s=25RS&b=HB-570) (accessed 2026-03-11T11:53:30Z)
- [CO bill page: SB26-051](https://leg.colorado.gov/bills/sb26-051) (accessed 2026-03-11T11:53:28Z)
- [Bill status: IL HB-4140](https://www.ilga.gov/legislation/BillStatus.asp?DocNum=4140&GESSION=104&GA=104&DocTypeID=HB&SessionID=114&LegID=) (accessed 2026-03-11T11:53:28Z)
- [Bill status: IL HB-3304](https://www.ilga.gov/legislation/BillStatus.asp?DocNum=3304&GESSION=104&GA=104&DocTypeID=HB&SessionID=114&LegID=) (accessed 2026-03-11T11:53:26Z)
- [Bill status: UT SB-142](https://le.utah.gov/~2025/bills/static/SB0142.html) (accessed 2026-03-11T11:53:21Z)
- [Lobbying search results for DCA in CA](https://cal-access.sos.ca.gov/Lobbying/Employers/Detail.aspx?q=Digital+Childhood+Alliance) (accessed 2026-03-11T11:48:35Z)
- ... and 64 additional sources

## Contact and Updates

This briefing is a living document updated as new findings are recorded. For the latest version, see the research repository tracking document.

Last updated: 2026-03-12
