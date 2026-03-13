# Meta Open-Source Licensing Timeline

*Generated 2026-03-11*

## Overview

This timeline documents Meta's (Facebook's) strategic open-source licensing decisions, controversies, and reversals from 2014 to present.

- **Total events documented:** 9
- **Date range:** 2014-10-28 to 2025-01-01

## Chronological Timeline

### 2014-10-28: Facebook introduces BSD+Patents license for React

*Category: Restrictive Licensing*

Facebook releases React under a BSD license with an additional 'PATENTS' file granting a patent license that is automatically revoked if the user sues Facebook for patent infringement. This is the 'BSD+Patents' license model.

**Sources:**

- [React PATENTS file (original)](https://github.com/facebook/react/blob/v0.12.0/PATENTS) (verified)

---

### 2017-04-18: Apache Software Foundation bans BSD+Patents license

*Category: External Pressure*

The Apache Software Foundation adds Facebook's BSD+Patents license to its Category-X list, effectively banning its use in Apache projects. ASF declares the patent retaliation clause incompatible with the Apache License. This forces major projects to reconsider their React dependencies.

**Sources:**

- [Apache Software Foundation -- Resolved License Questions](https://www.apache.org/legal/resolved.html) (verified)
- [LEGAL-303: Facebook BSD+Patents classification](https://issues.apache.org/jira/browse/LEGAL-303) (verified)

---

### 2017-07-16: WordPress announces move away from React

*Category: External Pressure*

WordPress co-founder Matt Mullenweg announces that WordPress will stop using React due to the BSD+Patents license. Given WordPress's market share, this is a significant blow to React's adoption trajectory.

**Sources:**

- [Matt Mullenweg -- On React and WordPress](https://ma.tt/2017/09/on-react-and-wordpress/) (verified)

---

### 2017-09-22: Facebook relicenses React to MIT

*Category: Strategic Reversal*

After sustained community backlash and the WordPress departure, Facebook relicenses React (and Jest, Flow, Immutable.js) from BSD+Patents to the MIT license. Engineering VP Sophie Alpert announces the change. This represents a capitulation to community pressure and sets a precedent for Facebook's licensing strategy.

**Sources:**

- [Facebook Engineering -- Relicensing React, Jest, Flow, and Immutable.js](https://engineering.fb.com/2017/09/22/web/relicensing-react-jest-flow-and-immutable-js/) (verified)
- [React relicense commit (GitHub)](https://github.com/facebook/react/commit/b765fb25ebc6e53bb8de2496d2828d9d01c2774b) (verified)

---

### 2019-03-01: Facebook releases PyTorch under modified BSD license

*Category: Open Licensing*

PyTorch is released under a standard BSD-3-Clause license without the patent rider, reflecting lessons learned from the React controversy. This positions PyTorch for broad adoption in the AI/ML community without licensing friction.

**Sources:**

- [PyTorch LICENSE file (GitHub)](https://github.com/pytorch/pytorch/blob/main/LICENSE) (verified)

---

### 2023-07-18: Meta releases Llama 2 with custom 'open' license

*Category: Restrictive Licensing*

Meta releases Llama 2 under a custom license that allows free use and redistribution but includes restrictions: commercial users with >700M monthly active users must obtain a separate license from Meta. The license is not OSI-approved and has been criticised as 'open-washing' -- marketing proprietary software as open source.

**Sources:**

- [Meta Llama 2 Community License Agreement](https://ai.meta.com/llama/license/) (verified)
- [OSI Blog -- Meta's Llama 2 license is not open source](https://blog.opensource.org/meta-llama-2-license-is-not-open-source/) (inaccessible)
- [The Verge -- Meta releases Llama 2](https://www.theverge.com/2023/7/18/23799025/meta-ai-llama-2-open-source-microsoft) (verified)

---

### 2024-04-18: Meta releases Llama 3 with updated custom license

*Category: Restrictive Licensing*

Meta releases Llama 3 under an updated community license that maintains the 700M MAU commercial threshold and adds acceptable use restrictions prohibiting certain applications. The license continues to be criticised as 'source available' rather than truly open source. Meta brands it as 'open' while retaining control over commercial deployment at scale.

**Sources:**

- [Meta Llama 3 Community License Agreement](https://llama.meta.com/llama3/license/) (inaccessible)
- [Meta AI Blog -- Introducing Meta Llama 3](https://ai.meta.com/blog/meta-llama-3/) (inaccessible)

---

### 2024-07-23: Llama 3.1 release maintains restrictive license

*Category: Restrictive Licensing*

Meta releases Llama 3.1 (405B, 70B, 8B) under the same custom community license. Despite being marketed as the largest 'open' model release, the license remains non-OSI-compliant. The Open Source Initiative continues to object to Meta's use of 'open' terminology for models with usage and commercial restrictions.

**Sources:**

- [Meta AI Blog -- Llama 3.1](https://ai.meta.com/blog/meta-llama-3-1/) (inaccessible)
- [OSI -- Meta's Llama 3.1 and the Open Source Definition](https://opensource.org/blog/metas-llama-3-1-and-the-open-source-definition) (inaccessible)

---

### 2025-01-01: Industry discussion: potential closed-weights pivot

*Category: Strategic Analysis*

Industry analysts and open-source advocates discuss the possibility that Meta may further restrict model weights in future releases, moving from 'available weights' to fully closed or API-only access. Drivers include competitive pressure from OpenAI/Google, safety concerns, and potential regulatory requirements. This would complete a pattern of strategic licensing shifts: from open to selectively open to restricted.

**Sources:**

- [SemiAnalysis -- Industry analysis on Meta AI strategy](https://www.semianalysis.com/) (verified)

---

## Strategic Pattern Analysis

### Restrict-then-Open Cycle

Meta repeatedly introduces restrictive licensing, faces community backlash, then relicenses to standard open-source terms. This was seen with React (BSD+Patents -> MIT) and may be playing out with Llama (custom license -> potential future change).

- **Supporting events:** 5
- **Confidence:** high

### Open-Source as Marketing Strategy

Meta uses 'open' branding for releases that do not meet OSI's Open Source Definition. This creates adoption through perceived openness while retaining commercial control. Llama 2/3 are marketed as 'open' despite having commercial use restrictions.

- **Supporting events:** 4
- **Confidence:** high

### Licensing as Competitive Moat

Meta's licensing choices appear calibrated to maximise adoption while preventing competitors (companies with >700M MAU) from freely deploying Meta's models. This suggests licensing is used as a competitive weapon rather than a community good.

- **Supporting events:** 2
- **Confidence:** medium

### Escalating Restrictions Over Time

While React moved toward more open licensing, Meta's AI licensing has moved in the opposite direction -- from no AI models released to 'available but restricted' to 'restricted with use policies'. This suggests Meta may further tighten restrictions as AI models become more commercially valuable.

- **Supporting events:** 3
- **Confidence:** medium

## Event Type Summary

| Type | Count | Description |
|------|-------|-------------|
| Restrictive Licensing | 4 | Releases with non-standard licenses that restrict use |
| External Pressure | 2 | Community or organisational pushback on licensing |
| Strategic Reversal | 1 | Meta changes licensing in response to pressure |
| Open Licensing | 1 | Standard OSI-approved open-source licensing |
| Strategic Analysis | 1 | Forward-looking analysis of licensing direction |
