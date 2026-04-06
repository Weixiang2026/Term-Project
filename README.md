# Canada Energy 2026–2030: Renewables vs Energy Intensity (SDG 7)

## Project Title and Decision Statement

**Decision-maker:** Tim Hodgson, Canada's Minister of Energy and Natural Resources

**Decision:** Should Tim Hodgson, Canada's Minister of Energy and Natural Resources, prioritize expanding renewable energy (SDG 7.2.1) or reducing energy intensity (SDG 7.3.1) in Canada's 2026–2030 federal energy agenda?

---

## Executive Summary

Canada’s 2026–2030 energy agenda must balance affordability, reliability, emissions reduction, and long-term competitiveness. This project evaluates two policy priorities aligned with UN Sustainable Development Goal 7: expanding the renewable share of total final energy consumption (SDG 7.2.1) and reducing energy intensity (SDG 7.3.1), which measures how much energy is used per unit of economic output.

The evidence suggests that both strategies matter, but they affect the system differently. Renewable expansion mainly works through supply-side transformation, while energy intensity reduction acts through demand-side change, efficiency, and cost control. The project uses exploratory analysis, systems thinking, and scenario-based interpretation to examine which option gives the federal government the stronger leverage point between 2026 and 2030.

The main conclusion is that reducing energy intensity should be the primary federal priority for 2026–2030, while renewable expansion should continue in parallel as a complementary long-term strategy. This sequencing is more likely to reduce system pressure, improve affordability, and make renewable integration easier.

---

## Table of Contents

- [Project Title and Decision Statement](#project-title-and-decision-statement)
- [Executive Summary](#executive-summary)
- [Background](#background)
- [Data Sources](#data-sources)
- [Exploratory Findings](#exploratory-findings)
- [System Dynamics](#system-dynamics)
- [Analysis](#analysis)
- [Recommendations](#recommendations)
- [Limitations and Future Work](#limitations-and-future-work)
- [References](#references)
- [Optional Reflection](#optional-reflection)

---

## Background

For full background research, stakeholder analysis, and early decision framing, see [Background.md](./Background.md).

---

## Data Sources

This project uses public World Bank SDG indicator data for Canada:

1. **SDG 7.2.1 – Renewable Energy Share**  
   Indicator Code: `EG.FEC.RNEW.ZS`  
   Unit: `% of total final energy consumption`

2. **SDG 7.3.1 – Energy Intensity**  
   Indicator Code: `EG.EGY.PRIM.PP.KD`  
   Unit: `MJ per constant 2017 PPP GDP`

Cleaned files and documentation are stored in the [`data`](./data) folder.  
Detailed wrangling notes are provided in [Wrangling.md](./Wrangling.md).

---

## Exploratory Findings

### Visualization 1: Renewable Energy Share Trend
![Renewable Trend](./img/viz01_renewables_share_trend_sdg721_2000_2021.png)

Canada’s renewable energy share shows a gradual long-term increase, but the pace is modest rather than transformational. This suggests that renewable expansion is happening, but not yet at a scale that guarantees rapid structural change by 2030.

### Visualization 2: Energy Intensity Trend
![Energy Intensity Trend](./img/viz02_energy_intensity_trend_sdg731_2000_2021.png)

Energy intensity declines much more consistently over time. This indicates that Canada has historically made steadier progress in using less energy per unit of economic output.

### Visualization 3: Dual-Axis Trend Comparison
![Dual-Axis Trend](./img/viz03_dual_axis_trends_sdg721_vs_sdg731_2000_2021.png)

Comparing both indicators on the same timeline shows that renewable share and energy intensity move in different ways. Renewable growth is slower and less even, while energy intensity reduction is more stable. This difference matters for policy sequencing.

### Visualization 4: Relationship Between Renewable Share and Energy Intensity
![Scatter Plot](./img/viz04_scatter_sdg721_vs_sdg731_trendline_2000_2021.png)

The relationship between the two variables appears broadly inverse: higher renewable share tends to align with lower energy intensity. This supports the idea that supply-side and demand-side progress can reinforce one another, even if they do not move in lockstep.

---

## System Dynamics

### Final Causal Loop Diagram
![Final CLD](./img/cld-final.png)

The final causal loop diagram shows why this decision is difficult: both renewable expansion and energy intensity reduction improve the system, but they do so through different feedback structures. The first major loop, **R1: the renewable investment loop**, is reinforcing. More renewable investment increases renewable capacity, which raises the renewable share of energy consumption. As renewable share rises, political and public support for further clean-energy action can also rise, which encourages additional investment. This loop is important because it explains how early renewable success can build momentum over time.

However, the CLD also shows a balancing constraint on this pathway. In **B2: the grid constraint loop**, more renewable capacity increases grid stress and integration needs. That can raise system costs and delays, especially when transmission, storage, and permitting capacity do not expand fast enough. Higher costs and delays can then slow future renewable investment. This means renewable expansion is strategically important, but its short-run performance depends heavily on complementary infrastructure and coordination.

The third major loop is **B1: the efficiency-pressure loop**, which centers on energy intensity. When energy intensity is high, energy demand pressure and system costs tend to be higher. Higher pressure and cost create stronger incentives for efficiency programs, standards, and demand-side management. Those interventions reduce energy intensity, which then lowers demand pressure. This is a balancing loop because it works against system strain and stabilizes the energy system over time.

The leverage point highlighted in the diagram is **efficiency programs and standards**. This point is attractive because it influences multiple parts of the system at once. Lower energy intensity can reduce demand growth, ease pressure on infrastructure, improve affordability, and make renewable integration easier. For the Minister’s 2026–2030 decision, the CLD suggests that reducing energy intensity is the stronger near-term leverage point, while renewable expansion remains essential as a parallel long-term strategy.

---

## Analysis

Detailed Milestone 3 analysis is available in [Analysis.md](./Analysis.md).

The Milestone 3 analysis used the **Foundational (Path A)** approach. It identified two relevant system archetypes: **Growth and Underinvestment** and **Shifting the Burden**. These archetypes explain why renewable expansion can be slowed by grid, storage, and permitting bottlenecks, and why excessive focus on new supply can weaken attention to deeper demand-side solutions.

Three scenarios were developed:

- **Status Quo:** mixed policy continues without a clear priority
- **Intervention A:** prioritize reducing energy intensity
- **Intervention B:** prioritize renewable expansion

Across these scenarios, reducing energy intensity appears to offer the stronger near-term leverage point because it lowers demand pressure, supports affordability, improves competitiveness, and makes renewable integration easier.

---

## Recommendations

**Recommendation:** Tim Hodgson should make **reducing energy intensity** the primary federal energy priority for 2026–2030, while continuing targeted support for renewable expansion as a complementary strategy rather than the single dominant focus.

The main reason is that energy intensity reduction appears to be the more controllable and system-wide leverage point in the short to medium term. In the project data, Canada’s energy intensity improved far more consistently than renewable share expanded. That pattern suggests that demand-side action has historically produced steadier structural change. It also fits the system logic shown in the final CLD: lowering energy intensity reduces demand pressure, eases system costs, improves affordability, and makes renewable integration more manageable. In contrast, renewable expansion remains critical for long-term decarbonization, but it is more exposed to bottlenecks in transmission, storage, grid reliability, and project delivery.

This recommendation does **not** mean renewable energy should be deprioritized in an absolute sense. Instead, it means the federal agenda should sequence its efforts more carefully. If the government first pushes harder on energy efficiency, building retrofits, industrial efficiency, appliance standards, and demand-side management, it can reduce the size of the system problem that new clean supply must solve. A lower-intensity economy is easier and cheaper to decarbonize. It is also more resilient if electricity demand grows quickly because of electrification, population growth, or industrial expansion.

The evidence also supports this sequencing. Natural Resources Canada reports that Canada used 25% less energy per dollar of GDP in 2022 than in 2000, showing meaningful long-run improvement in energy productivity. At the same time, federal clean electricity policy recognizes that demand is growing and that reliability and affordability must be maintained alongside decarbonization. Those facts reinforce the view that a demand-side-first emphasis offers the strongest near-term risk-adjusted payoff.

This recommendation could change under several conditions. If major grid infrastructure, storage, and permitting improvements are implemented faster than expected, renewable expansion may become a stronger near-term priority. Likewise, if provincial policy alignment improves significantly, the federal government may be able to accelerate renewable deployment with fewer system bottlenecks than the current evidence suggests.

The most practical next steps are:
1. expand federal efficiency and retrofit programs for buildings and industry;
2. tighten equipment and performance standards where feasible;
3. support demand-side management and electrification measures that reduce energy use per unit of output;
4. continue renewable investments that are paired with transmission, storage, and grid modernization; and
5. monitor annual movement in both SDG 7.2.1 and SDG 7.3.1 so policy priority can be adjusted if system conditions change.

Additional information that would strengthen this analysis includes province-level data, sector-level energy intensity data, project delivery timelines for grid infrastructure, and more current measures of affordability and reliability impacts.

---

## Limitations and Future Work

This project has several limitations. First, it relies mainly on national-level indicator data, which is useful for strategic comparison but too aggregated to capture important regional differences across Canada. Energy systems are shaped by provincial resource mixes, grid structures, industrial composition, and policy design, so a national average can hide important variation.

Second, the project uses a limited number of variables. That makes the analysis clear and focused, but it cannot fully represent all drivers of energy outcomes, such as fuel prices, provincial regulations, sector mix, trade exposure, or technological learning rates. Third, the evidence is better for identifying broad system patterns than for proving causal effects. The CLD is a decision-support tool, not a causal proof on its own.

Future work should extend the analysis with province-level and sector-level data, especially for electricity demand, building efficiency, industrial energy use, and grid constraints. A stronger version of this project could also include a simple forecast model or policy dashboard to compare scenarios under different assumptions.

---

## References

World Bank. (2024). *Renewable energy consumption (% of total final energy consumption) – Canada (EG.FEC.RNEW.ZS).* World Development Indicators.

World Bank. (2024). *Energy intensity level of primary energy (MJ/$2017 PPP GDP) – Canada (EG.EGY.PRIM.PP.KD).* World Development Indicators.

Government of Canada. (2024). *Clean Electricity Regulations: maintaining reliability.*

Canadian Centre for Energy Information. (2025). *Energy Fact Book, 2025–2026: Energy efficiency.*

Canada Energy Regulator. (2026). *Canada’s Energy Future 2026.*

---

## Optional Reflection

This project showed me that a good analysis is not only about finding trends in data. It is also about helping a real decision-maker choose between competing options under constraints. What surprised me most was that the “better” policy was not simply the one that seemed more ambitious. Renewable expansion is very important, but the system view showed that it can be slowed by infrastructure bottlenecks. Reducing energy intensity looked less dramatic at first, but it turned out to be a strong leverage point because it affects affordability, demand pressure, and implementation difficulty at the same time.

I also learned that a causal loop diagram can make an analysis much more useful. It helped connect the data, the policy tradeoffs, and the final recommendation in one structure. If I had more time, I would improve the project by adding province-level data and a small forecast component. Overall, this project helped me practice systems thinking, policy analysis, data interpretation, and professional repository presentation.
