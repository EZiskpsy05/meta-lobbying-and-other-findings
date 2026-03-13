# DCA & DCI DNS/WHOIS Deep Dive

**Research Date:** 2026-03-12
**Domains Analyzed:** digitalchildhoodalliance.org, digitalchildhoodinstitute.org

---

## 1. WHOIS Comparison

| Field | DCA (digitalchildhoodalliance.org) | DCI (digitalchildhoodinstitute.org) |
|-------|-----|-----|
| **Registrar** | GoDaddy.com, LLC | GoDaddy.com, LLC |
| **Created** | 2024-12-18T04:11:13Z | 2025-06-13T16:59:23Z |
| **Updated** | 2025-11-23T19:23:18Z | 2025-07-31T16:56:26Z |
| **Expires** | 2028-12-18 (4-year registration) | 2026-06-13 (1-year registration) |
| **Privacy** | GoDaddy privacy (registrant REDACTED) | GoDaddy privacy (registrant REDACTED) |
| **Nameservers** | Cloudflare (leia, mitch) | Cloudflare (macy, santino) |

### Key Observations
- **Same registrar (GoDaddy)** and same privacy protection for both domains
- DCA has a **4-year registration** (paid through 2028) suggesting long-term commitment/funding
- DCI has only a **1-year registration** (expires June 2026) suggesting limited resources
- Both use **Cloudflare** DNS/CDN but on **different nameserver pairs** (leia/mitch vs macy/santino)
- DCA was registered **6 months before** DCI — despite DCI's founder (McKay) being the more established figure

---

## 2. DNS Analysis

### MX Records (Email)
| Domain | MX Record | Provider |
|--------|-----------|----------|
| DCA | `digitalchildhoodalliance-org.mail.protection.outlook.com` | **Microsoft 365** |
| DCI | `digitalchildhoodinstitute-org.mail.protection.outlook.com` | **Microsoft 365** |

**SHARED INFRASTRUCTURE:** Both organizations use Microsoft 365 (Outlook) for email. The MX record naming convention (`{domain}-org.mail.protection.outlook.com`) indicates paid Microsoft 365 Business subscriptions, not free email.

### TXT Records (SPF/Authentication)
**DCA SPF record:**
```
v=spf1 mx include:_spf.elasticemail.com include:_spf.google.com include:amazonses.com include:spf.protection.outlook.com ~all
```

**DCI SPF record:**
```
v=spf1 include:spf.protection.outlook.com include:_spf.elasticemail.com -all
```

### SPF Comparison

| SPF Include | DCA | DCI | Significance |
|-------------|-----|-----|-------------|
| `spf.protection.outlook.com` | Yes | Yes | Microsoft 365 email |
| `_spf.elasticemail.com` | Yes | Yes | **Shared email marketing platform** |
| `_spf.google.com` | Yes | No | Google Workspace (DCA also uses Google) |
| `amazonses.com` | Yes | No | Amazon SES (transactional email) |

**KEY FINDING:** Both DCA and DCI use **Elastic Email** (`_spf.elasticemail.com`) for email marketing/mass communications. This shared infrastructure suggests either:
1. The same person/team set up both organizations' email systems
2. A shared service provider configured both domains
3. Coordinated operations between the two entities

DCA has a more sophisticated email infrastructure (Microsoft 365 + Google + Amazon SES + Elastic Email) compared to DCI (Microsoft 365 + Elastic Email only), consistent with DCA having significantly more funding.

### Google Site Verification
Both domains have Google site verification TXT records, indicating both have been verified with Google (for Search Console, Analytics, etc.):
- DCA: Two verification codes (suggesting multiple Google accounts or re-verification)
- DCI: One verification code

### Microsoft Verification
Both have `MS=` verification records for Microsoft 365:
- DCA: `MS=ms94509368`
- DCI: `MS=ms49512351` and `MS=ms89712736` (two records — possibly re-verified)

### A Records (Hosting)
| Domain | IP Addresses | Provider |
|--------|-------------|----------|
| DCA | 172.67.74.77, 104.26.11.53, 104.26.10.53 | Cloudflare CDN |
| DCI | 172.67.69.219, 104.26.3.135, 104.26.2.135 | Cloudflare CDN |

Both are behind Cloudflare CDN. The `104.26.x.x` IPs are Cloudflare shared hosting IPs, so the actual origin servers are hidden.

---

## 3. Infrastructure Summary

### Shared Infrastructure Between DCA and DCI
1. **Same registrar:** GoDaddy
2. **Same privacy service:** GoDaddy Domain Privacy
3. **Same CDN/DNS provider:** Cloudflare
4. **Same email provider:** Microsoft 365
5. **Same email marketing platform:** Elastic Email
6. **Both verified with Google:** Google Search Console

### Differences
1. Different Cloudflare nameserver pairs (normal for separate accounts)
2. DCA has additional email infrastructure (Google, Amazon SES)
3. DCA has 4-year domain registration vs DCI's 1-year
4. DCA was registered 6 months before DCI

---

## 4. Significance

The extensive shared infrastructure strongly suggests that DCA and DCI were set up by the same person or team, or share operational resources. The shared use of Elastic Email (an email marketing platform) is particularly notable — it suggests coordinated mass communications capability.

The DCA domain's 4-year registration (through 2028) and more sophisticated email setup (Microsoft 365 + Google + Amazon SES + Elastic Email) suggests significantly more funding and operational planning compared to DCI's minimal 1-year registration.

The fact that DCA (the 501(c)(4) lobbying arm) was registered 6 months before DCI (the 501(c)(3) research arm) is notable — typically the educational arm is established first to build credibility before the lobbying arm. The reverse order suggests DCA was the primary objective, with DCI added later as a supporting entity.
