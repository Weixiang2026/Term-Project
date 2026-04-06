# Milestone 3: Analysis (Path A — Foundational)

## Why Path A Fits This Project

This project is fundamentally a decision-support exercise rather than a purely predictive one. The central question is not only which indicator changed faster in the past, but which policy priority is more likely to produce a stronger and more manageable system response between 2026 and 2030. Because Milestone 2 already established key feedback loops through the Causal Loop Diagram (CLD), the Foundational path is the strongest fit. It allows the analysis to build directly on the project’s existing strengths: systems thinking, trade-off analysis, and policy relevance.

Milestone 2 showed three important patterns. First, Canada’s renewable energy share increased only modestly over the long run, rising from 22.6% in 1990 to 23.8% in 2021. Second, energy intensity declined much more consistently, from 8.3 MJ per unit of GDP in 1990 to about 6.0 in 2022. Third, the project’s exploratory analysis suggests that rising renewable share and falling energy intensity are related, but not perfectly, which implies that policy sequencing and implementation capacity matter.

These findings support a systems-focused analysis. The issue is not whether renewables or efficiency matter—they both do. The question is where the federal government can intervene for the greatest near-term leverage while still supporting long-term decarbonization. Path A is therefore appropriate because it helps explain why the system may resist change, where bottlenecks appear, and how different policy priorities could produce different medium-term trajectories.

---

## System Archetype Analysis

### Archetype 1: Growth and Underinvestment

The most visible system archetype in this decision context is **Growth and Underinvestment**. In this structure, growth begins, but the supporting capacity required to sustain it is not expanded quickly enough. Performance then weakens, not because the original strategy is wrong, but because complementary investment lags behind demand.

In Canada’s energy system, the growth process is renewable deployment. More renewable investment increases renewable capacity, which can increase renewable share, lower emissions intensity, and build additional political support for clean electricity. However, this growth loop is constrained by underinvestment in transmission, storage, grid modernization, interprovincial coordination, and permitting capacity. When those enabling systems lag, renewable expansion becomes slower, more expensive, and more politically contested.

This archetype maps closely to the project’s CLD. The reinforcing loop is:

**Renewable Investment -> Renewable Capacity -> Renewable Share -> Political Support -> Renewable Investment**

The balancing constraint is:

**Renewable Capacity -> Grid Stress / Infrastructure Bottlenecks -> System Costs and Delays -> Slower Renewable Expansion**

The pattern is supported by both project evidence and current policy context. The project’s renewable trend shows only modest long-run growth rather than a sharp acceleration. World Bank data show Canada’s renewable energy share rising from 22.6% in 1990 to 23.8% in 2021, an increase of only 1.2 percentage points over three decades. At the same time, the Government of Canada states that the Clean Electricity Regulations are intended to meet growing electricity demand while preserving affordability and reliability, and that they provide a market signal for investment in renewable energy, smart grids, distributed systems, and storage. That policy language strongly implies that generation growth alone is insufficient without enabling infrastructure.

### Generic Archetype Diagram

```mermaid
flowchart LR
    A[Growth Engine] --> B[System Growth]
    B --> C[Need for Supporting Capacity]
    C --> D[Investment in Capacity]
    D --> E[Available Capacity]
    E --> B
    B --> F[Strain on Capacity]
    F --> G[Delays / Costs / Bottlenecks]
    G --> B
