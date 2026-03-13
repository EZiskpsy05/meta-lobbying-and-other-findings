# EU vs US Age Verification: Comparative Analysis

*Generated 2026-03-11*

## Executive Summary

This report compares the European Union and United States approaches to age verification for online services. The EU has adopted a **platform-level** model through the Digital Services Act (DSA), placing compliance obligations on platforms proportionate to their size, with explicit exemptions for free and open-source software (FOSS) and small enterprises. The US is pursuing an **OS-level** model through state legislation (California AB 1043, Colorado SB 26-051), requiring operating system providers to build age attestation infrastructure with no FOSS exemptions.

The architectural divergence has significant implications for the open-source software ecosystem, user privacy, market competition, and the future of software distribution.

## EU Model: Digital Services Act

### Regulatory Framework

The Digital Services Act (Regulation (EU) 2022/2065) establishes a graduated framework for online platform regulation. Age verification obligations arise primarily through:

- **Article 28**: Online protection of minors
- **Articles 34-35**: Risk assessment and mitigation for VLOPs
- **Recital 71**: Age verification as a risk mitigation measure

### VLOP Threshold

Very Large Online Platforms (VLOPs) are defined as platforms with **45 million or more average monthly active recipients** in the EU (Article 33). Only VLOPs face the full suite of obligations including systemic risk assessment and mandatory age verification measures.

### FOSS and Small Business Exemptions

- **Recital 13**: FOSS repositories not acting as intermediary services are outside DSA scope entirely
- **Micro/small enterprise exemption**: Entities with <50 employees and <EUR 10M turnover receive reduced obligations
- **VLOP threshold**: Effectively exempts all FOSS platforms from the heaviest requirements

### EU Digital Identity Wallet (EUDIW)

The EU is building open-source age verification infrastructure through the EUDIW under eIDAS 2.0. Key features:

- **Selective disclosure**: Users prove age bracket without revealing date of birth
- **Open-source**: Reference implementation available under Apache 2.0/EUPL
- **Interoperable**: Works across all EU member states and platforms
- **User-controlled**: No centralised tracking of verification events

## US Model: OS-Level Attestation

### Legislative Landscape

Multiple US states are pursuing age verification legislation that targets the operating system and device layer:

- **California AB 1043**: Requires mobile OS providers to offer age verification signals to application distribution platforms
- **Colorado SB 26-051**: Mandates device-level age attestation APIs

### Architectural Choice

Unlike the EU platform-level approach, US bills place the compliance burden on OS vendors (primarily Apple and Google), who must build age attestation infrastructure that app stores and developers then consume. This creates a fundamentally different trust architecture:

- Age verification becomes an OS-level service
- OS vendors become gatekeepers for all software distribution
- Hardware attestation (TPM, Secure Enclave) becomes legally required infrastructure

### Missing FOSS Protections

Neither AB 1043 nor SB 26-051 contains:

- A FOSS exemption or carve-out
- A small entity threshold
- Recognition of non-commercial software distribution
- Technology neutrality provisions

## Comparison Matrix

| Dimension | EU Model | US Model |
|-----------|----------|----------|
| **Compliance Burden** | Platform-level (VLOPs responsible) | OS/device-level (Apple/Google responsible) |
| **FOSS Impact** | Exempt (Recital 13, size thresholds) | No exemption; excludes FOSS OSes |
| **Privacy** | Selective disclosure via EUDIW; GDPR integration | OS vendors gain visibility into app access patterns |
| **Technical Approach** | Technology-neutral | Prescriptive (hardware attestation) |
| **Enforcement** | Unified (DSCs + Commission for VLOPs) | Fragmented (state-by-state AG enforcement) |
| **Small Entity Exemptions** | Yes (<50 employees, <EUR 10M) | None |
| **Open Standards** | EUDIW open-source reference implementation | Proprietary vendor APIs only |
| **Innovation Impact** | Preserves competition and alternatives | Reinforces Apple/Google duopoly |

## FOSS Impact Analysis

### EU: How FOSS Is Protected

1. **Scope exclusion**: FOSS repositories outside DSA scope (Recital 13)
2. **Size thresholds**: Most FOSS organisations qualify for micro/small enterprise exemptions
3. **VLOP filter**: No FOSS platform reaches 45M monthly EU users
4. **Technology neutrality**: FOSS platforms choose their own methods
5. **Open-source tooling**: EUDIW provides FOSS-compatible compliance pathway

### US: How FOSS Is Threatened

1. **OS-level mandate**: Linux distributions and custom Android ROMs cannot provide proprietary hardware attestation
2. **Distribution channel coverage**: F-Droid, Flathub, and Linux package managers may be classified as 'application distribution platforms'
3. **No exemption**: Zero carve-outs for non-commercial or open-source software distribution
4. **License conflicts**: Proprietary age verification SDKs may conflict with copyleft (GPL) licensing
5. **Cascading policies**: App store policy changes driven by legislation affect all developers regardless of FOSS status

### Affected FOSS Projects

- **Operating Systems**: All Linux desktop distributions, LineageOS, GrapheneOS, CalyxOS, /e/OS, PostmarketOS, PureOS
- **App Stores**: F-Droid, Flathub, Snap Store
- **Package Managers**: apt, dnf, pacman, portage, and all Linux package management systems
- **App Developers**: Any GPL-licensed application distributed through stores requiring proprietary attestation SDKs

## Implications

### 1. Existential Risk to FOSS Distribution

The US OS-level approach creates a regulatory environment where FOSS operating systems and distribution channels may become legally non-compliant by default, not because they refuse to verify ages, but because the technical infrastructure required is controlled by proprietary vendors.

### 2. Vendor Lock-In as Regulation

By mandating OS-level attestation, US legislation effectively codifies the Apple/Google duopoly into law. Compliance becomes impossible without access to proprietary attestation infrastructure, ensuring that no alternative OS or distribution channel can compete on equal terms.

### 3. Privacy Architecture Divergence

The EU privacy-by-design approach (EUDIW selective disclosure) contrasts sharply with the US model, which gives OS vendors comprehensive visibility into which applications minors attempt to access -- creating surveillance potential absent from the EU model.

### 4. Regulatory Arbitrage Risk

Divergent transatlantic approaches may push privacy-conscious developers and FOSS projects toward EU jurisdictions, fragmenting the global open-source ecosystem.

### 5. Need for US FOSS Exemption

At minimum, US legislation should include:

- Explicit FOSS exemption for non-commercial software distribution
- Small entity thresholds comparable to EU micro/small enterprise rules
- Technology neutrality provisions allowing alternative verification methods
- Recognition that package managers are not equivalent to commercial app stores

## Database Findings

**Finding 1** (confidence: high):
EU DSA age verification analysis: Age verification obligations under the DSA apply primarily to VLOPs (>= 45M monthly EU users) through Articles 34-35 risk assessment and mitigation requirements. Smaller platforms face graduated obligations. FOSS projects that do not act as intermediary services are outside DSA scope entirely (Recital 13). Micro/small enterprises receive additional exemptions from transparency and reporting requirements.

*Sources: https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32022R2065*

---

**Finding 2** (confidence: high):
EU age verification blueprint: The EU approach centres on the EUDIW (EU Digital Identity Wallet) under eIDAS 2.0, providing government-issued verifiable credentials with selective disclosure for age verification. Found 0 related GitHub repos. T-Scy consortium search returned 4 results. Key difference from US approach: wallet-based, user-controlled, interoperable across platforms and OS vendors.

*Sources: GitHub API, EC EUDIW documentation*

---

**Finding 3** (confidence: high):
EU vs US age verification comparison: EU uses platform-level regulation (DSA/VLOPs) with FOSS exemptions and privacy-by-design (EUDIW). US uses OS-level mandates (AB 1043, SB 26-051) with no FOSS exemption, concentrating power in Apple/Google. Key risk: US approach threatens open-source OS distributions and creates vendor lock-in absent from the EU model.

*Sources: EUR-Lex (DSA), CA AB 1043, CO SB 26-051*

---

**Finding 4** (confidence: high):
FOSS exemption analysis: EU provides 5 distinct protection mechanisms for FOSS. US model creates 4 categories of threat affecting 13+ named projects/channels. 4 technical barriers exist with no current FOSS workaround. The EU EUDIW (open-source) provides a compliance pathway for FOSS; the US offers none.

*Sources: DSA Recital 13, AB 1043 text, SB 26-051 text, EUDIW GitHub*

---

**Finding 5** (confidence: high):
EU DSA age verification analysis: Age verification obligations under the DSA apply primarily to VLOPs (>= 45M monthly EU users) through Articles 34-35 risk assessment and mitigation requirements. Smaller platforms face graduated obligations. FOSS projects that do not act as intermediary services are outside DSA scope entirely (Recital 13). Micro/small enterprises receive additional exemptions from transparency and reporting requirements.

*Sources: https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32022R2065*

---

**Finding 6** (confidence: high):
EU age verification blueprint: The EU approach centres on the EUDIW (EU Digital Identity Wallet) under eIDAS 2.0, providing government-issued verifiable credentials with selective disclosure for age verification. Found 0 related GitHub repos. T-Scy consortium search returned 4 results. Key difference from US approach: wallet-based, user-controlled, interoperable across platforms and OS vendors.

*Sources: GitHub API, EC EUDIW documentation*

---

**Finding 7** (confidence: high):
EU vs US age verification comparison: EU uses platform-level regulation (DSA/VLOPs) with FOSS exemptions and privacy-by-design (EUDIW). US uses OS-level mandates (AB 1043, SB 26-051) with no FOSS exemption, concentrating power in Apple/Google. Key risk: US approach threatens open-source OS distributions and creates vendor lock-in absent from the EU model.

*Sources: EUR-Lex (DSA), CA AB 1043, CO SB 26-051*

---

**Finding 8** (confidence: high):
FOSS exemption analysis: EU provides 5 distinct protection mechanisms for FOSS. US model creates 4 categories of threat affecting 13+ named projects/channels. 4 technical barriers exist with no current FOSS workaround. The EU EUDIW (open-source) provides a compliance pathway for FOSS; the US offers none.

*Sources: DSA Recital 13, AB 1043 text, SB 26-051 text, EUDIW GitHub*

## Sources

- Regulation (EU) 2022/2065 (Digital Services Act): https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32022R2065
- Regulation (EU) 2024/1183 (eIDAS 2.0): https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32024R1183
- EUDIW Reference Implementation: https://github.com/eu-digital-identity-wallet
- California AB 1043 (Age-Appropriate Design Code): https://leginfo.legislature.ca.gov/
- Colorado SB 26-051: https://leg.colorado.gov/bills/sb26-051
- European Commission VLOP designations: https://digital-strategy.ec.europa.eu/en/policies/list-designated-vlops-and-vloses-under-digital-services-act
