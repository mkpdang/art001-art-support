# Estimate — TT-AIM-SPRINT-8C (20h Technical Analysis)

**Project:** TT-AIM-SPRINT-8C
**Based on:** Estimate-TankTerminals-TT-AIM-SPRINT-8C-v1.xlsx
**Scope:** Technical analysis & discovery (20 hours)
**Date:** 2026-03-17

---

## Summary

This is a 20-hour technical analysis estimate for the TT-AIM-SPRINT-8C sprint, which covers 8 tickets across the TankTerminals platform. The original sprint estimate is 162 implementation hours over 5 weeks with a team of 7 (React JS, PHP backend, Python, QA, DevOps, PM).

The purpose of this 20h engagement is to perform a structured technical analysis before development begins, following the Syntograde discovery process.

---

## Sprint Tickets Overview

| # | Ticket | Title | Original Est. |
|---|--------|-------|---------------|
| 1 | TT-2436 | Implement measures AI misuse | 12h |
| 2 | TT-2439 | Improvement LPB for BargeInsights: Tanker Type specific LPB stats | 20h |
| 3 | TT-2434 | Split Logistical Benchmarking (Non-Stripe subscriptions) | 3.5h |
| 4 | TT-2423 | Logical Checks Dashboard | 58.5h |
| 5 | TT-2444 | Rhine CPP: Low and High, make available in API | 4h |
| 6 | TT-2435 | Improvement on Ship and Terminal Modal | 64h |
| 7 | TT-2443 | Process Historical Waiting Times Data | TBD |
| | | **Total development hours** | **162h** |

---

## 20-Hour Technical Analysis Breakdown

### Phase 1. Environment Setup — 4h

| Task | Hours |
|------|-------|
| Access and review source code (PHP backend, React frontend, Python LPB app) | 1.0 |
| Set up local dev environment (PHP/Slim API, React JS, Python services) | 1.5 |
| Restore database snapshot and connect services | 1.0 |
| Verify system starts and key workflows function | 0.5 |

---

### Phase 2. Code & Architecture Review — 7h

| Task | Hours |
|------|-------|
| Review PHP/Slim API codebase structure and patterns | 1.5 |
| Review React JS frontend architecture | 1.0 |
| Review Python LPB application and data pipeline | 1.0 |
| Database schema analysis (terminals, ships, subscriptions, benchmarking data) | 1.5 |
| Map external integrations (Stripe subscriptions, ReCaptcha, APIs, email) | 1.0 |
| Infrastructure & deployment review (staging/production, DevOps setup) | 1.0 |

---

### Phase 3. Feature Strategy Evaluation — 5h

Evaluate implementation approach for each ticket group:

| Task | Hours |
|------|-------|
| **Security & anti-abuse** (TT-2436): Review login tracking, CSRF, ReCaptcha integration points | 0.5 |
| **LPB / Python pipeline** (TT-2439): Assess berth data function, asset class extensibility | 0.75 |
| **Subscription splitting** (TT-2434): Map Stripe vs non-Stripe logic, data migration needs | 0.5 |
| **Logical Checks Dashboard** (TT-2423): Evaluate 30 rules engine, dashboard architecture, tab layout complexity | 1.25 |
| **Rhine CPP API** (TT-2444): Review back-office gasoil/gasoline data flow and API exposure | 0.25 |
| **Ship & Terminal Modal** (TT-2435): Assess factsheet UI, map integration, berth widget, responsive constraints | 1.0 |
| **Historical Waiting Times** (TT-2443): Evaluate data processing pipeline requirements | 0.25 |
| Cross-ticket dependency analysis and strategy recommendation | 0.5 |

---

### Phase 4. Risk Assessment & Mitigation — 2.5h

| Task | Hours |
|------|-------|
| Identify risks: Stripe integration complexity, subscription data migration | 0.5 |
| Identify risks: 30-rule engine scalability, dashboard performance (TT-2423) | 0.5 |
| Identify risks: Python LPB pipeline changes impacting existing data (TT-2439) | 0.25 |
| Identify risks: Security implementation gaps (CSRF, ReCaptcha, abuse detection) | 0.25 |
| Identify risks: Mobile/responsive UI constraints (TT-2435) | 0.25 |
| Define mitigation strategies and testing approach | 0.75 |

---

### Reporting — 1.5h

| Task | Hours |
|------|-------|
| Compile findings into technical analysis report | 0.75 |
| Prepare prioritized implementation roadmap with dependencies | 0.5 |
| Review and finalize deliverables | 0.25 |

---

## Hour Summary

| Phase | Hours |
|-------|-------|
| 1. Environment Setup | 4.0 |
| 2. Code & Architecture Review | 7.0 |
| 3. Feature Strategy Evaluation | 5.0 |
| 4. Risk Assessment & Mitigation | 2.5 |
| Reporting | 1.5 |
| **Total** | **20.0** |

---

## Technology Stack (from estimate)

- **Frontend:** React JS
- **Backend:** PHP (Slim API framework)
- **Data/Analytics:** Python (LPB application)
- **Payments:** Stripe integration
- **Infrastructure:** Staging + Production environments

## Team Structure (original sprint)

| Role | Count |
|------|-------|
| React JS Developer | 1 |
| PHP Backend Developer | 2 |
| Python Developer | 1 |
| QA | 1 |
| DevOps | 1 |
| Project Manager | 1 |

---

## Deliverables

1. Working local development environment
2. Architecture overview (codebase, database, infrastructure, integrations)
3. Per-ticket implementation strategy recommendation
4. Risk register with mitigation strategies
5. Prioritized implementation roadmap

## Assumptions

- Source code access (Git), database snapshot, and staging environment are provided
- Original estimate and ticket descriptions are accurate and current
- The 20h analysis covers discovery only — implementation is scoped separately at 162h+ per the original estimate
