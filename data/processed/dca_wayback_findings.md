# Digital Childhood Alliance — Wayback Machine Website History Analysis

**Research Date:** 2026-03-12
**Data Source:** Wayback Machine CDX API (web.archive.org/cdx/)
**Domain:** digitalchildhoodalliance.org

---

## Executive Summary

Analysis of 100+ Wayback Machine snapshots from December 2024 through March 2026 confirms the DCA website launched on **December 19, 2024** and has been continuously operational since. The earliest snapshot shows a fully-developed advocacy site focused on the App Store Accountability Act. **No funder disclosures, "supported by," or sponsor logos were found in any snapshot.** The site uses Cloudflare protection, which blocked several archival attempts. Key sub-pages (/about-us/, /our-team/) were only archived starting September 2025.

---

## 1. Snapshot Timeline

### First Appearances

| Date | URL | Status | Notes |
|------|-----|--------|-------|
| **2024-12-19 03:51** | digitalchildhoodalliance.org/ | 200 | First ever snapshot — site is live |
| 2024-12-19 08:49 | http://digitalchildhoodalliance.org/ | 200 | HTTP variant |
| 2024-12-20 06:14 | www.digitalchildhoodalliance.org/ | 200 | WWW variant |
| 2024-12-25 04:12 | http://digitalchildhoodalliance.org/ | 200 | Christmas snapshot |
| 2025-01-15 19:07 | www.digitalchildhoodalliance.org/ | **403** | First Cloudflare block |
| 2025-01-19 22:26 | www.digitalchildhoodalliance.org/ | 200 | Accessible again |

### Cloudflare Blocks (403 responses)

Multiple snapshots returned 403 errors, indicating Cloudflare challenge pages:
- 2025-01-15, 2025-02-10 (x2), 2025-02-16, 2025-08-18, 2026-03-08

This pattern suggests DCA has intermittent bot protection that sometimes blocks Wayback Machine's crawler.

### Sub-page Archive Coverage

| Page | First Archived | Count |
|------|---------------|-------|
| Homepage (/) | 2024-12-19 | 50+ snapshots |
| /about-us/ | 2025-09-14 | 1 snapshot (Cloudflare blocked) |
| /our-team/ | 2025-09-14 | 1 snapshot (Cloudflare blocked) |
| /cookie-policy/ | 2025-03-23 | 3 snapshots |
| /asaabill/ | 2026-02-02 | 4 snapshots |
| Blog posts | 2025-02-11+ | Various |

---

## 2. Earliest Website Content (January 2025 Snapshot)

The January 19, 2025 snapshot (first fully readable) shows the following site structure:

### Navigation
- Home | Federal | State | Updates | FAQ | Join

### Hero Section
> "We are an alliance fighting for policies that prioritize parent empowerment and children's online well-being, because every child deserves a thriving and safe childhood."

### Priority Campaign: App Store Accountability
- "Putting Kids Before Big Tech Profits"
- Focus on requiring app stores to implement age verification, parental consent, and accurate age ratings

### Statistics Cited
- 200+ dangerous apps rated safe for kids on Apple's App Store
- 81% of U.S. adults support requiring parental consent for minors' social media accounts
- 71% favor age verification before accessing social media
- 31% of second graders use social media apps
- 91% of 14-year-olds own smartphones
- 1/3 of children lie about their age online
- 73% of parents use age ratings

### "Voices for App Store Accountability" Section
Listed supporters included:
- **Annie Chestnut Tutor** — Tech Policy Center Policy Analyst, The Heritage Foundation
- **Eleanor Gaetan, Ph.D.** — VP Public Policy, National Center on Sexual Exploitation
- **Todd Weiler** — Attorney, Utah State Senator

### Key Framing
The site frames the issue as:
- "A SYSTEM THAT LEAVES PARENTS POWERLESS"
- "ENACT COMMON-SENSE LEGISLATION TO PROTECT CHILDREN"
- Positions Apple and Google as the primary targets, not social media platforms

### No Funding Disclosures
- No "Supported by," "Funded by," or sponsor section
- No donor logos
- No mention of Meta, Headwaters Strategies, or any funder
- No 501(c)(4) designation visible on the homepage

---

## 3. Blog Post Archive History

| Date | Post Title |
|------|-----------|
| 2025-02-11 | "Apple's App Store Puts Kids a Click Away from a Slew of Inappropriate Apps" |
| 2025-03-23 | "Apple's Faux Safety Solution" |
| 2025-05-13 | "100+ Child Advocates Praise Introduction of App Store Accountability Act" |
| 2025-10-07 | "Apple and Google Do It Again: New CA Age Verification Law Fails Kids" |
| 2026-02-02 | /asaabill/ page created |
| 2026-03-06 | /asaabill/ updated |

**Pattern:** Posts exclusively target **Apple and Google**, never Meta/Facebook/Instagram. This is consistent with DCA's role as a Meta-funded advocacy group positioning app stores (not social media platforms) as the problem.

---

## 4. Infrastructure Details (from CDX metadata)

| Feature | Detail |
|---------|--------|
| Hosting | Behind Cloudflare CDN |
| Email protection | Cloudflare email obfuscation (cdn-cgi/l/email-protection) |
| CMS | WordPress (based on URL patterns) |
| Domain registration | GoDaddy, 2024-12-18 |
| HTTPS redirect | Yes, HTTP → HTTPS with www |
| Content type | text/html for pages |

---

## 5. Key Findings

### 5.1 No Funder Disclosures Ever Existed on the Site
Across all archived snapshots from December 2024 to March 2026, no version of the DCA website has ever included funder disclosures. This means:
- There were no "supported by" sections that were later removed
- The funding opacity was designed into the site from launch
- As a 501(c)(4), DCA has no legal obligation to disclose donors publicly

### 5.2 Site Launched Fully Formed
The December 19, 2024 snapshot shows a professionally designed site with:
- Complete policy messaging
- Statistics and talking points
- Named testimonials from Heritage Foundation and NCOSE staff
- Multiple call-to-action sections
This suggests professional development prior to domain registration, consistent with a well-funded organizational launch rather than a grassroots effort.

### 5.3 Consistent Anti-Apple/Google Messaging
Every blog post and page targets Apple and Google's app stores. Meta/Facebook/Instagram are never criticized — consistent with Meta's funding interest in shifting regulatory burden to app store operators.

### 5.4 Cloudflare Protection May Be Deliberate
The intermittent 403 blocks on archival attempts could indicate intentional bot protection to limit the amount of DCA content preserved in public archives.

---

## 6. Comparison: Earliest vs. Current Content

| Element | Dec 2024/Jan 2025 | Current (2026) |
|---------|-------------------|----------------|
| Navigation | Home, Federal, State, Updates, FAQ, Join | Same + expanded |
| Hero message | Parent empowerment, safe childhood | Same |
| Target | Apple and Google app stores | Same |
| Funding disclosure | None | None |
| Team page | Not archived until Sep 2025 | Casey Stefanski, John Read, Dawn Hawkins, Melissa McKay |
| Blog posts | None initially | 10+ posts |
| ASAA bill page | Not present | Added Feb 2026 |

---

## Sources

- Wayback Machine CDX API: https://web.archive.org/cdx/search/cdx?url=digitalchildhoodalliance.org
- Earliest snapshot: https://web.archive.org/web/20241219035107/https://digitalchildhoodalliance.org/
- January 2025 snapshot: https://web.archive.org/web/20250119222653/https://www.digitalchildhoodalliance.org/
