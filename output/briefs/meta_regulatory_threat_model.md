# Threat Model: Meta's Ideal Regulatory Outcome

*Generated 2026-03-12*

## Executive Summary

This threat model documents the scenario in which age attestation mandates effectively require commercial operating system services for consumer device compliance. We analyse how this regulatory outcome would marginalise Linux for consumer use and map Meta's competitive advantage through Horizon OS.

**Date:** 2026-03-12

**Classification:** Threat Model -- Task 5.3

## Threat Scenario: Mandatory Commercial OS Services

### Scenario Description

State legislatures pass age attestation requirements that mandate OS-level identity verification for minors' access to online services. The technical compliance path requires:

1. A platform-level identity service (verified account system)
2. An age verification API accessible to applications
3. Hardware attestation binding (TPM/Secure Enclave)
4. A liable legal entity operating the verification service

### Impact on Linux

Linux distributions cannot satisfy requirements (1), (2), or (4) without fundamental restructuring. Community distributions have no legal entity to operate verification services, no account infrastructure, and no mechanism to mandate identity verification before granting system access.

**Result:** Linux-based consumer devices become non-compliant. Schools, libraries, and consumer electronics manufacturers would be forced to use commercial operating systems exclusively.

## Linux Marginalisation for Consumer Use

### Affected Use Cases

- **Education:** Chromebooks (ChromeOS/Linux) in schools would need to route all age verification through Google's account system, eliminating any Linux-native alternative
- **Libraries:** Public-access terminals running Linux would need commercial identity services, contradicting patron privacy mandates
- **Consumer Electronics:** IoT devices, media centres, and embedded Linux systems used by minors would need commercial verification services
- **Developing Nations:** Linux adoption in regions without commercial account infrastructure would be legally foreclosed

### Technical Barriers to Linux Compliance

- No standard age attestation D-Bus service
- No centralised identity provider
- Package managers (apt, dnf, pacman) have no age-gating mechanism
- The Linux kernel has no concept of 'user age' at the kernel level
- Implementing these features would require a fundamental architectural change incompatible with Linux's design philosophy

## Meta's Competitive Advantage via Horizon OS

### Horizon OS Architecture

Meta's Horizon OS (the operating system powering Quest VR headsets) is a vertically integrated platform:

- Mandatory Meta account required for device activation
- Built-in age verification at account creation
- App store with content rating enforcement
- Full control over system-level APIs
- Hardware attestation via platform security

### Regulatory Advantage

If age attestation becomes mandatory, Horizon OS is already compliant by design. Meta gains:

1. **Competitive moat:** Open-source XR platforms (Monado, etc.) cannot compete because they lack the identity infrastructure
2. **Market lock-in:** Developers must target Horizon OS for compliant XR applications
3. **Data advantage:** All age verification flows through Meta's systems, providing additional user data
4. **Lobbying ROI:** The cost of lobbying for these mandates is far less than the competitive advantage gained

### Age Verification Vendor Ecosystem

Tracked vendors: Yoti, Jumio, Veriff, AgeKey/K-ID, Concordium, MyMahi, KJR, Persona, Shufti, GeoComply, ShareRing, IKETech, CitizenCard, Centrebound Limited, Netsweeper, Ondato, Veratad, NEEDEMAND, BT Group, Incode, IDVerse, Envoc, OpenAge, Luciditi, Kids Web Services, Fujitsu, BlueCheck, FaceTec, PRIVO, Innovative Technology, Privately, Age Check Certification Scheme, Serve Legal, OneID, yoti, Verifymy, Experian, AgeChecked

These vendors provide the technical layer that makes compliance possible for commercial platforms while remaining inaccessible to community-maintained systems.

## Lobbying and Influence Map

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

### Influence Timeline

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

## Supporting Evidence

### High-Confidence Research Findings

- **Task horizon-os-audit:** Horizon OS has 5 built-in compliance features: Meta Account Age Verification; Get Age Category API; Family Center; Quest Store Age Ratings; Minor Account Defaults. These collectively address age verification, parental consent, content controls, parental tools, and default protections for minors.

- **Task horizon-os-audit:** Linux distros have 7 major compliance gaps: Account System Age Bracket; Age Category D-Bus API; Parent-Child Account Linking; Parental Consent Verification; Package Manager Age-Rating Enforcement; Unified Parental Controls Dashboard; Age-Gated Default Profiles. Estimated total implementation effort: 36-71 months of coordinated cross-project work.

- **Task 2.1:** Meta employees hold 0 maintainer and 0 reviewer positions across 0 kernel subsystems (kernel mainline HEAD). 0 unique individuals identified.

- **Task 2.4:** Meta employees hold 0 of 0 BPF maintainer/reviewer positions (0.0%). BPF-related subsystem sections: 0.

- **Task 2.4:** Alexei Starovoitov: BPF co-maintainer and original author. Co-created eBPF (extended BPF) while at PLUMgrid, then joined Facebook/Meta. Serves as BPF subsystem co-maintainer alongside Daniel Borkmann. Controls the direction of BPF development.

- **Task 2.4:** Andrii Nakryiko: BPF libraries maintainer, libbpf author. Primary author and maintainer of libbpf, the canonical BPF user-space library. Designed BPF CO-RE (Compile Once, Run Everywhere) architecture. Key architect of BPF tooling ecosystem.

- **Task 2.4:** Martin KaFai Lau: BPF networking maintainer. Maintains BPF networking components. Contributed BPF socket storage, cgroup BPF, and other networking-specific BPF features used extensively in Meta's infrastructure.

- **Task 2.4:** Song Liu: BPF contributor, live patching. Contributed BPF trampoline and live-patching support. Works on BPF performance features used in Meta's fleet.

- **Task 2.4:** Yonghong Song: BPF compiler/BTF contributor. Key contributor to BTF (BPF Type Format) and BPF CO-RE compiler support in LLVM/Clang. Enables the 'compile once' paradigm that is central to Meta's BPF deployment strategy.

- **Task 2.7:** Licensing pattern identified: 'Restrict-then-Open Cycle'. Meta repeatedly introduces restrictive licensing, faces community backlash, then relicenses to standard open-source terms. This was seen with React (BSD+Patents -> MIT) and may be playing out with Llama (custom license -> potential future change). Evidence: 5 events. Confidence: high.

- **Task 2.7:** Licensing pattern identified: 'Open-Source as Marketing Strategy'. Meta uses 'open' branding for releases that do not meet OSI's Open Source Definition. This creates adoption through perceived openness while retaining commercial control. Llama 2/3 are marketed as 'open' despite having commercial use restrictions. Evidence: 4 events. Confidence: high.

- **Task 2.7:** Documented 9 licensing events spanning 2014-10-28 to 2025-01-01. Identified 4 strategic patterns in Meta's open-source licensing behaviour: Restrict-then-Open Cycle, Open-Source as Marketing Strategy, Licensing as Competitive Moat, Escalating Restrictions Over Time.

- **Task 3.1:** OpenXR extension audit: 265 total extensions found. Meta authored 76 (28.7% of total, 40.4% of vendor-specific). XR_FB_*: 41, XR_META_*: 35.

- **Task 3.4:** Meta holds Platinum membership at the Linux Foundation at $500,000/yr. This grants Meta a guaranteed board seat, TSC voting rights, and marketing council seat. Platinum members have direct governance influence over LF project selection, funding, and strategic direction.

- **Task 3.4:** Kathy Kam, Director of Open Source at Meta, serves as Meta's Platinum member representative on the Linux Foundation Board of Directors. This gives Meta direct influence on LF governance including project selection, budget allocation, and policy decisions.

## Risk Assessment

| Risk Factor | Likelihood | Impact | Notes |
|-------------|------------|--------|-------|
| Age attestation mandates pass in 5+ states | HIGH | HIGH | Multiple bills already introduced |
| Mandates require OS-level implementation | MEDIUM | HIGH | Technical requirements in current drafts imply this |
| Linux distributions cannot comply | HIGH | CRITICAL | Fundamental architectural incompatibility |
| Meta lobbying accelerates adoption | MEDIUM | HIGH | Known lobbying activity in multiple states |
| Open-source XR platforms foreclosed | HIGH | HIGH | Horizon OS is only compliant XR platform |
| Federal preemption codifies requirements | LOW | CRITICAL | Would affect all states simultaneously |

## Recommendations

1. **Engage state legislatures** during comment periods to highlight open-source impact
2. **Propose technology-neutral language** that does not assume commercial identity infrastructure
3. **Document the compliance gap** between commercial and community operating systems
4. **Build coalition** with EFF, FSF, Linux Foundation, and Software Freedom Conservancy
5. **Monitor Meta lobbying disclosures** for coordinated legislative campaigns
6. **Develop alternative compliance frameworks** that respect open-source architecture (e.g., browser-level rather than OS-level attestation)
