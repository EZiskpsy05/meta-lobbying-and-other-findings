# AOSP Gerrit Contribution Analysis

*Generated 2026-03-11*
*Updated 2026-03-12 — DATA RETRACTED*

## RETRACTION NOTICE

**This report has been retracted.** The Gerrit REST API queries failed silently, returning zero results for all vendors including Samsung and Qualcomm (who are known major AOSP contributors with thousands of upstream patches). The data below is entirely invalid and should not be cited.

**Root cause:** The `owner:domain:` query syntax either requires authentication or is not supported by the public AOSP Gerrit API. All results reflect API query failures, not actual contribution counts.

**Recommendation:** If AOSP contribution analysis is needed, use the AOSP source tree commit history directly (`git log` on the AOSP mirror repos) rather than the Gerrit REST API.

---

## Original Data (INVALID — DO NOT CITE)

The data below was generated from failed API queries and is preserved only for audit trail purposes.

| Entity | Domain | Total | Merged | Open | Abandoned |
|--------|--------|------:|-------:|-----:|----------:|
| Meta (facebook.com) | facebook.com | 0 | 0 | 0 | 0 |
| Meta (meta.com) | meta.com | 0 | 0 | 0 | 0 |
| Meta (oculus.com) | oculus.com | 0 | 0 | 0 | 0 |
| Samsung | samsung.com | 0 | 0 | 0 | 0 |
| Qualcomm | quicinc.com | 0 | 0 | 0 | 0 |
| Google | google.com | 1 | 0 | 0 | 1 |
