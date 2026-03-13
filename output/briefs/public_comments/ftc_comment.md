# Public Comment -- FTC: Age Verification and Open-Source Impact

*Generated 2026-03-12*

## RE: Age Verification and Online Safety -- Impact on Open-Source Software

**Date:** 2026-03-12

**Submitted to:** Federal Trade Commission

**Subject:** Comment on Proposed Age Verification Requirements and Their Impact on Open-Source Operating Systems and Free Software

## Summary of Position

We write to bring to the Commission's attention a significant unintended consequence of proposed age verification and attestation mandates: the structural exclusion of open-source operating systems from consumer markets.

While the goal of protecting minors online is laudable and important, the technical implementation path assumed by current proposals -- OS-level identity verification -- is incompatible with the architecture of Linux and other community-maintained operating systems. This creates an asymmetric regulatory burden that advantages large technology companies with vertically integrated platforms.

## Background: Open-Source Operating Systems

Linux-based operating systems power approximately 96% of the world's top web servers, the majority of smartphones (via Android), and an increasing share of consumer desktop and embedded devices. Unlike commercial operating systems (Windows, macOS, iOS), Linux distributions are:

- Maintained by volunteer communities and nonprofit foundations
- Distributed without mandatory user accounts
- Designed without centralised identity infrastructure
- Licensed under terms (GPL, MIT, Apache) that guarantee user freedom

These properties are features, not bugs. They are the foundation of digital privacy, security research, and technological self-determination.

## The Technical Problem

Age attestation mandates, as drafted in multiple state bills, require:

1. A platform-level identity verification service
2. An API for applications to query verified age status
3. A liable legal entity operating the verification

Linux distributions satisfy none of these requirements and cannot reasonably be modified to do so without abandoning their fundamental design principles.

### State Legislative Activity

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

## Competitive Distortion

We note that several technology companies that benefit from age attestation mandates -- including Meta Platforms -- are actively lobbying for these requirements across multiple states. Companies with existing account infrastructure and identity services face minimal compliance costs, while open-source alternatives face existential barriers.

This dynamic warrants Commission scrutiny under Section 5 of the FTC Act, as it may constitute an unfair method of competition: using regulatory capture to disadvantage competitors who cannot replicate closed-platform identity infrastructure.

## Research Evidence

Our research has identified the following relevant findings:

- Task horizon-os-audit: Horizon OS has 5 built-in compliance features: Meta Account Age Verification; Get Age Category API; Family Center; Quest
- Task horizon-os-audit: Linux distros have 7 major compliance gaps: Account System Age Bracket; Age Category D-Bus API; Parent-Child Account Lin
- Task 2.1: Meta employees hold 0 maintainer and 0 reviewer positions across 0 kernel subsystems (kernel mainline HEAD). 0 unique in
- Task 2.4: Meta employees hold 0 of 0 BPF maintainer/reviewer positions (0.0%). BPF-related subsystem sections: 0.
- Task 2.4: Alexei Starovoitov: BPF co-maintainer and original author. Co-created eBPF (extended BPF) while at PLUMgrid, then joined
- Task 2.4: Andrii Nakryiko: BPF libraries maintainer, libbpf author. Primary author and maintainer of libbpf, the canonical BPF use
- Task 2.4: Martin KaFai Lau: BPF networking maintainer. Maintains BPF networking components. Contributed BPF socket storage, cgroup
- Task 2.4: Song Liu: BPF contributor, live patching. Contributed BPF trampoline and live-patching support. Works on BPF performance
- Task 2.4: Yonghong Song: BPF compiler/BTF contributor. Key contributor to BTF (BPF Type Format) and BPF CO-RE compiler support in 
- Task 2.7: Licensing pattern identified: 'Restrict-then-Open Cycle'. Meta repeatedly introduces restrictive licensing, faces commun

## Requested Commission Action

We respectfully request that the Commission:

1. **Study the impact** of age verification mandates on open-source software before endorsing any technical standards
2. **Require technology neutrality** in any age verification framework, ensuring compliance paths exist for non-commercial platforms
3. **Investigate potential anticompetitive effects** of corporate lobbying for OS-level age attestation mandates
4. **Engage open-source stakeholders** (Linux Foundation, FSF, EFF, Apache Foundation) in policy development
5. **Consider browser-level alternatives** to OS-level attestation that do not discriminate against open platforms
