# Smart Engineering Innovation Hub — Project Documentation

**Course:** Project Management and Economics for Engineering (ECON3372)  
**Institution:** Birzeit University — Department of Computer Engineering  
**Team:** Aya Abdullah (1220782) · Lana Daramna (1220588) · Haneen Qaisi (1220201)  
**Instructor:** Sana' Atari

---

## Overview

This repository contains the full project management plan and supporting research paper for the **Smart Engineering Innovation Hub with Integrated Digital Management System** — a six-month initiative designed to support engineering students in completing academic and practical projects more efficiently.

The project addresses three core challenges in engineering education:
- Limited access to electronic components and shared tools
- Lack of organized, well-managed workspaces
- Weak coordination between students, resources, and mentors

The solution combines a **centralized physical hub** with a **digital management system** covering user registration, workspace scheduling, inventory tracking, and operational reporting.

---

## Repository Contents

```
├── README.md                          — this file
├── project_management_final.pdf       — full project management plan (Phases 1–3)
├── research_management.pdf            — research paper: Risk Management Using Fuel Price Forecasting
```

---

## Project Management Plan

### Phase 1 — Initiation & Strategic Foundation

Defines the project's purpose, objectives, scope, and stakeholder landscape.

**Project Charter Highlights**
- Title: *Smart Engineering Innovation Hub with Integrated Digital Management System*
- Duration: 6 months (24 weeks)
- Budget Ceiling: $37,400 USD (estimated)
- Scope: Planning and management activities only — excludes physical construction and full system deployment

**Key Stakeholders**

| Stakeholder | Role | Impact |
|---|---|---|
| Engineering Students | Primary users | High |
| University Administration | Sponsor & oversight | High |
| Technical Mentors | Guidance & consultation | High |
| Project Management Team | Planning & control | High |
| Electronic Component Suppliers | Procurement partners | Medium |

**Feasibility Summary**
- Technical: Feasible — relies on commonly available resources and established technologies
- Financial: Feasible — focused on planning activities within a controlled budget
- Operational: Feasible — aligns with existing institutional structures and processes

---

### Phase 2 — Planning & Technical Structure

#### Work Breakdown Structure (WBS)

Six main work areas, each broken into packages:

1. **Physical Setup** — site selection, layout design, workspace setup, infrastructure planning
2. **Digital System Development** — requirements, architecture, UI/UX wireframes, data security
3. **Staffing** — role definition, recruitment, training
4. **Procurement** — supplier identification, RFQ, delivery and inventory intake
5. **Testing** — physical readiness checks, digital UAT, user feedback
6. **Launch** — soft opening, full launch, KPI monitoring

#### Schedule — Key Milestones

| Milestone | Week | Description |
|---|---|---|
| M1 | 2 | Site finalized and lease signed |
| M2 | 8 | Digital system design approved |
| M3 | 10 | All equipment and furniture delivered |
| M4 | 12 | Staff hired and trained |
| M5 | 22 | UAT completed, system ready |
| M6 | 24 | Hub officially launched |

#### Budget Summary

| Category | Estimated Cost (USD) |
|---|---|
| Equipment | $8,500 |
| Furniture | $5,200 |
| Software Development | $6,000 |
| Salaries (6 months) | $12,000 |
| Miscellaneous | $2,300 |
| Contingency Reserve (10%) | $3,400 |
| **Total** | **$37,400** |

#### Technology Stack

- **Frontend:** React.js + Bootstrap
- **Backend:** Node.js + Express
- **Database:** PostgreSQL
- **Hosting:** AWS / Azure
- **Version Control:** GitHub
- **Project Management:** Trello + Google Workspace

#### Procurement Strategy

- Supplier shortlisting (minimum 3 per category)
- Evaluation matrix: cost 30% · quality 25% · delivery 20% · warranty 15% · reputation 10%
- Contract types: fixed-price for furniture/kits, unit-price for components, service agreements for staff

---

### Phase 3 — Execution, Monitoring & Control

#### Organizational Structure

The project uses a **functional–project hybrid** structure:
- **Project Sponsor** (University Administration) — strategic oversight and major approvals
- **Project Manager** — coordination, schedule, cost, risk, and communication
- **Technical Lead** — digital system design and validation
- **Procurement Lead** — supplier coordination and delivery
- **Hub Supervisor** — physical hub operations and safety compliance
- **Technical Mentors** — guidance and UAT support
- **IT Support Coordinator** — infrastructure and compatibility

#### RACI Summary

| Activity | Sponsor | PM | Tech Lead | Procurement | Hub Supervisor |
|---|---|---|---|---|---|
| Project Charter | A | R | C | C | C |
| Budget Approval | A | R | C | C | I |
| Digital System Design | C | A | R | I | I |
| Procurement | C | A | C | R | I |
| Staff Recruitment | C | A | C | C | R |
| System Testing | I | A | R | I | C |
| Launch Approval | A | R | C | C | C |

#### Risk Register (Top Risks)

| Risk | Probability | Impact | Mitigation |
|---|---|---|---|
| Digital system development delay | Medium | High | Modular milestones; simplified soft-launch fallback |
| Budget overrun (equipment costs) | Medium | High | Fixed-price contracts; contingency reserve |
| Equipment delivery delay | Medium | Medium | Early procurement; schedule buffer |
| Insufficient qualified mentors | Low | High | Early recruitment with defined criteria |
| Low pilot user adoption | Medium | Medium | Awareness campaign; extended pilot period |
| Safety compliance issues | Low | High | Safety inspection checklist before opening |

#### Key Performance Indicators

- Schedule Performance: % of tasks completed on time
- Budget Performance: % variance from planned cost
- Procurement Efficiency: delivery within agreed timeline
- System Readiness: completion of defined test cases
- Pilot Usage Rate: % of workstations booked during pilot
- Inventory Accuracy Rate: recorded vs. actual inventory alignment

#### Change Management

- Minor changes (no cost/schedule impact) → Project Manager approval
- Moderate changes → Sponsor review
- Major changes (significant scope/cost/schedule) → Sponsor approval required
- All changes documented via Change Request Form and tracked in Change Log

---

## Research Paper — Risk Management in Energy Projects Using Fuel Price Forecasting

### Abstract

This paper examines how fuel price forecasting can be integrated into energy project risk management frameworks. Using historical Brent crude oil data from FRED and the World Bank Commodity Price Database, an ARIMA(1,1,1) model was applied to generate short-term price forecasts. The study focuses on translating forecasting outputs into actionable management decisions rather than maximizing predictive accuracy.

### Key Findings

**Forecasting Performance**
- Model: ARIMA(1,1,1) on monthly Brent crude oil data
- Validation period: most recent 12 months held out
- MAE: ~$7.79 USD · MAPE: ~11.79%
- 6-month base forecast: ~$67 USD/barrel (stable near-term outlook)

**Scenario Construction**

| Scenario | Adjustment | Monthly Cost (10,000 bbl) |
|---|---|---|
| Base | ARIMA forecast | $670,000 |
| High (adverse) | +15% | $770,000 |
| Low (favorable) | −10% | $603,000 |

Over a 6-month project, the gap between base and high scenarios totals **$600,000** — the quantitative basis for contingency reserve sizing.

### Four Risk Management Applications

1. **Contingency Reserve Allocation** — Scenario spread provides an objective, market-linked basis for determining reserve adequacy rather than using arbitrary percentages.

2. **Procurement Strategy Optimization** — Stable forecasts favor spot purchasing; rising forecasts favor forward contracts or price-ceiling clauses in supplier agreements.

3. **Scenario-Based Budget Development** — Replaces single-point cost estimates with a price envelope (e.g., "$670K base / $603K–$770K range") that improves stakeholder transparency.

4. **Cost Control & Performance Monitoring** — Forecast scenarios serve as quantitative benchmarks; deviations trigger management reviews and continuous model refinement.

### Limitations

- ARIMA assumes future behavior follows historical patterns — may break during structural market shifts
- Scenario boundaries (+15% / −10%) are grounded in observed volatility but remain somewhat arbitrary
- Brent crude is used as a proxy — may not fully represent gas, coal, or renewable fuel dynamics

### References

Key sources cited in the paper:
- Wei, Wei & Huang (2016) — crude oil price volatility and value-at-risk
- Kumar & Sharma (2021) — ARIMA, GARCH, and hybrid ML forecasting comparison
- Wang, Wu & Yang (2019) — oil price forecasting in the era of big data
- Al-Shammari & Hassan (2023) — AI-based market risk prediction in oil markets
- Zhang & Chen (2024) — GARCH and machine learning for energy market volatility
- Paltsev (2017), Ringland (1998), Amer et al. (2013) — scenario planning methodology

---

## How to Navigate This Documentation

Start with the **Project Charter** (Section 1.1) for a one-page summary of goals and constraints, then review the **WBS** (Section 2.1) and **Gantt chart** (Section 2.2) for the execution roadmap. The **Risk Register** (Section 3.5.3) and **RACI Matrix** (Section 3.2.3) are the most frequently referenced sections during execution. The **research paper** provides the theoretical and analytical foundation for the risk management approach applied in the project plan.
