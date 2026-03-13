# Horizon OS vs Linux Distro: Compliance Readiness Comparison

*Generated 2026-03-11*

## Overview

This report compares Meta Horizon OS and generic Linux distributions
against the child-safety requirements of **California AB 1043** and
**Colorado SB 26-051**.  Each requirement is scored 0-3:

| Score | Meaning |
|-------|---------|
| 3 | Fully ready -- feature exists and meets requirement |
| 2 | Mostly ready -- feature exists with gaps |
| 1 | Partial -- some capability exists, significant work needed |
| 0 | Absent -- no capability, must be built from scratch |

## Aggregate Scores

| Platform | Score | Max | Readiness |
|----------|-------|-----|-----------|
| Horizon OS | 30 | 36 | 83.3% |
| Linux Distro | 5 | 36 | 13.9% |

**Gap:** +25 points in favor of Horizon OS

## Detailed Comparison: AB 1043 (California)

| Req ID | Category | Requirement | Horizon OS | Score | Linux Distro | Score |
|--------|----------|-------------|------------|-------|--------------|-------|
| AB1043-1 | Age Verification | Determine whether a user is a minor before allowing access t | Built-in Get Age Category API (ovr_AgeCategory_Get | 3/3 | No standard age-verification API. AccountsService  | 0/3 |
| AB1043-2 | Parental Consent | Obtain verifiable parental consent before allowing minors to | Family Center provides parent-child account linkin | 3/3 | No built-in parental-consent mechanism. GNOME/KDE  | 0/3 |
| AB1043-3 | Data Handling | Limit collection and retention of minors' personal informati | Meta Privacy Center governs data practices. Child  | 2/3 | Linux does not track/share user data centrally --  | 1/3 |
| AB1043-4 | Content Controls | Provide age-appropriate default settings for minor accounts | Age-gated app ratings in Quest Store. Family Cente | 3/3 | Flatpak/Snap have OARS age-rating metadata. GNOME  | 1/3 |
| AB1043-5 | Transparency | Publish annual transparency report on minor-safety measures | Meta publishes transparency reports (community sta | 1/3 | Not applicable at OS level -- distros don't operat | 0/3 |
| AB1043-6 | App Store Duty | App distribution platform must enforce age-rating metadata | Quest Store requires IARC age ratings for all apps | 3/3 | Flathub has OARS content ratings. Package managers | 1/3 |

## Detailed Comparison: SB 26-051 (Colorado)

| Req ID | Category | Requirement | Horizon OS | Score | Linux Distro | Score |
|--------|----------|-------------|------------|-------|--------------|-------|
| SB051-1 | Age Verification | Covered platform must reasonably determine user age before p | Built-in Get Age Category API (ovr_AgeCategory_Get | 3/3 | No standard age-verification API. AccountsService  | 0/3 |
| SB051-2 | Parental Consent | Parental or guardian consent required for users under 16 | Family Center provides parent-child account linkin | 3/3 | No built-in parental-consent mechanism. GNOME/KDE  | 0/3 |
| SB051-3 | Data Handling | Prohibit sale or sharing of minors' personal data | Meta Privacy Center governs data practices. Child  | 2/3 | Linux does not track/share user data centrally --  | 1/3 |
| SB051-4 | Duty of Care | Platforms must exercise reasonable care to prevent harm to m | Horizon OS has built-in personal-boundary system,  | 2/3 | No OS-level duty-of-care features. Individual apps | 0/3 |
| SB051-5 | Parental Tools | Provide parents with supervision and monitoring tools | Family Center: screen time limits, app approval, a | 3/3 | GNOME has malcontent (app restrictions, usage limi | 1/3 |
| SB051-6 | Default Protections | Enable strongest privacy and safety settings by default for  | Minor accounts default to restricted social featur | 2/3 | No concept of minor-account defaults in standard L | 0/3 |

## Key Findings

### What Horizon OS has built-in

- **Account system with age verification:** Meta accounts store age at sign-up; Get Age Category API exposes age bracket to all apps.
- **Parental consent flow:** Family Center requires parent to create/approve child accounts.
- **App store with age ratings:** Quest Store enforces IARC ratings; parent can approve/block apps via Family Center.
- **Comprehensive parental tools:** Screen time, activity reports, friend oversight, purchase controls.
- **Default protections for minors:** Private-by-default, restricted social features, limited discoverability.

### What Linux distros would need to build

- **Account infrastructure:** Age-bracket field in AccountsService or systemd-homed; D-Bus API for apps to query user age category.
- **Parental consent system:** Parent-child account linking with verified guardian authentication.
- **Package manager changes:** Enforce OARS age ratings across apt/dnf/pacman; block installation of unrated packages for minor accounts.
- **D-Bus APIs for parental controls:** Standardized interface for screen time, app restrictions, and activity reporting across DEs.
- **Default profile system:** Age-gated default configurations that apply privacy and safety settings based on account age bracket.

### Implementation complexity for Linux

| Component | Complexity | Estimated Effort |
|-----------|------------|------------------|
| Age-bracket field in AccountsService | Medium | 2-3 months |
| D-Bus Age Category API | Medium | 1-2 months |
| Parent-child account linking | High | 6-12 months |
| Parental consent verification | High | 6-12 months |
| Package manager age-rating enforcement | High | 6-12 months per PM |
| Unified parental controls (cross-DE) | Very High | 12-24 months |
| Age-gated default profiles | Medium | 3-6 months |
| Transparency reporting framework | Low | 1-2 months |

**Total estimated effort:** 3-5 years of coordinated cross-project work (freedesktop.org, GNOME, KDE, package managers, distro maintainers).

---

*This report is generated by horizon_os_audit.py as part of the meta-linux-research project.*
