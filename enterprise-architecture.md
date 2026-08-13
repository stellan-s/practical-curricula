# Practical Enterprise Architecture

> This curriculum was developed with AI assistance and has not been independently validated.

**Goal:** Produce a defensible, portfolio-quality enterprise architecture for an anonymized 25-person SaaS company—not merely learn enterprise-architecture vocabulary.

**Time:** Approximately 29 hours. Complete the modules in order. Use one continuous case throughout: a SaaS company with CRM, billing, customer onboarding, analytics, several third-party integrations, and growing operational risk.

## Selected channels

- [Fragile to Agile](https://www.youtube.com/@FragiletoAgile) — strongest practical strategy-to-roadmap spine.
- [The Open Group](https://www.youtube.com/@theopengroup) — authoritative TOGAF and ArchiMate context.
- [Karl Stanley: Enterprise Architecture, Tools, Tips and Training](https://www.youtube.com/@KarlStanley) — concrete enterprise-architecture artifacts and modeling practice.
- [SAP LeanIX / SAP Community](https://www.youtube.com/@SAPCommunity) — useful portfolio, data, and decision-management demonstrations; treat the product as an example, not the method.
- [Enterprise Architecture in Practice](https://www.youtube.com/@EnterpriseArchitectureInPractice) — unusually concrete governance implementation.

## 1. Frame the architecture problem — 2.5 h

**Watch**

1. Fragile to Agile — [The Difference Between Enterprise Architecture and Solution Architecture](https://www.youtube.com/watch?v=ttxFpQ2dq38)
2. Fragile to Agile — [Introduction to Digital Transformation Roadmaps](https://www.youtube.com/watch?v=-Xsr5qaA_ek)
3. The Open Group — [The TOGAF Standard, 10th Edition and the Certification Portfolio](https://www.youtube.com/watch?v=uh36bZ7bWPI) — watch for framework literacy; ignore certification detail.

**Exercise:** Write a one-page architecture mandate: business trigger, three outcomes, scope, five stakeholders, constraints, decisions enterprise architecture must enable, and explicit non-goals.

## 2. Translate strategy into capabilities — 3.5 h

**Watch**

1. Fragile to Agile — [Establishing Business Intent and Outcomes](https://www.youtube.com/watch?v=wBHO2TM0-Rs)
2. Fragile to Agile — [Creating a Business Capability Model](https://www.youtube.com/watch?v=MmrLmoa50a0)
3. Fragile to Agile — [Capability Standardization](https://www.youtube.com/watch?v=xF_qAHc-AKA)

**Exercise:** Create a capability map with no more than eight level-1 and 25 level-2 capabilities; score each for strategic importance, current maturity, and target maturity, then highlight the five largest justified gaps.

## 3. Build a useful current-state repository — 4 h

**Watch**

1. Fragile to Agile — [How to Assess the Current State for a Technology Roadmap](https://www.youtube.com/watch?v=kqVwByO5AHw)
2. Karl Stanley — [Creating Current and Future State Application Portfolio Artefacts](https://www.youtube.com/watch?v=Rsujg_6b4-s)

**Exercise:** Inventory 12–20 applications and platforms with owner, lifecycle, cost band, technical risk, supported capabilities, critical data, system-of-record status, and dependencies; then draw one dependency landscape that answers a real question.

## 4. Model only the views people need — 4 h

**Watch**

1. The Open Group / Bizzdesign — [ArchiMate 3.0 in Practice: Introduction](https://www.youtube.com/watch?v=_kmYkxKb_-o)
2. The Open Group — [Introduction to ArchiMate: Motivation and Strategy](https://www.youtube.com/watch?v=JgwXcMES3F8)
3. The Open Group / Bizzdesign — [ArchiMate in Practice: Digital Transformation](https://www.youtube.com/watch?v=3tUSDoMx4YE)

**Tool:** Install [Archi, the free ArchiMate 3.2 modeling tool](https://www.archimatetool.com/download/). The videos use 3.0, but the core concepts used here remain applicable.

**Exercise:** Build three linked views in one Archi model: motivation, capability-to-application realization, and application/data/technology dependencies. Limit each view to one stakeholder question and roughly 20 visible elements.

## 5. Analyse application and data portfolios — 5 h

**Watch**

1. SAP Community / LeanIX — [Optimizing IT Spending Through Application Rationalization](https://www.youtube.com/watch?v=VxCEeWnp4nk)
2. SAP Community / LeanIX — [Your Guide to Data Architecture Using SAP LeanIX](https://www.youtube.com/watch?v=PTh5fO-_mYo)

**Reference:** Use the [TIME model](https://www.leanix.net/en/wiki/apm/gartner-time-model) for consistent portfolio decisions.

**Exercise:** Score ten applications for functional fit, technical fit, cost, and risk; assign Tolerate/Invest/Migrate/Eliminate; then map five data domains, their owners, systems of record, and three critical cross-system flows. Challenge every proposed elimination against dependencies and migration cost.

## 6. Design the target state and record decisions — 4 h

**Watch**

1. Fragile to Agile — [How to Determine Your Target State Architecture](https://www.youtube.com/watch?v=rFoNgBcEKqM)
2. SAP LeanIX — [Architecture Decisions in SAP LeanIX](https://www.youtube.com/watch?v=j2U6FKu8Br4)

**Tool:** Use the free [Markdown Architectural Decision Record template](https://github.com/adr/madr).

**Exercise:** Define three materially different target-state options, compare them against outcomes, cost, risk, reversibility, and capability gaps, select one, create the target ArchiMate view, and write two ADRs—including rejected alternatives and consequences.

## 7. Turn architecture into governed change — 6 h

**Watch**

1. GCC Transformation at Scale — [How to Create an Architecture Roadmap](https://www.youtube.com/watch?v=48CykVGJlfA)
2. Enterprise Architecture in Practice — [EA Governance Foundation: Operating Model](https://www.youtube.com/watch?v=YuF9ehxAeB0)
3. Enterprise Architecture in Practice — [EA Governance Foundation: Standards and Principles](https://www.youtube.com/watch?v=CslknutEUuk)

**Exercise:** Convert gaps into a three-horizon roadmap with dependencies, transition states, owners, decision points, and measurable outcomes; add five architecture principles, a lightweight review/exception flow, and a one-page executive view. Record a ten-minute briefing defending priorities and trade-offs.

## Completion standard

You are finished when the artifacts form one traceable chain:

`business outcomes → capabilities → current landscape → gaps → target decisions → roadmap → governance`

Do **not** add more frameworks or notation until a stakeholder question cannot be answered from that chain. The finished case is more valuable for your career than a TOGAF study notebook.
