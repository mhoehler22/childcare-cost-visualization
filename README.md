# Childcare Cost & Market Analysis — Pennsylvania

### Data visualization project analyzing childcare affordability across Pennsylvania counties to inform franchise expansion strategy

---

## Overview

This project uses federal childcare cost data to analyze where childcare prices represent a disproportionately high share of household income across Pennsylvania counties. The analysis supports a hypothetical business expansion strategy for a childcare franchise evaluating new markets. Deliverables include an interactive Tableau dashboard, an executive presentation, and an infographic poster.

Pennsylvania was selected because it has unusually complete county-level data in the National Database of Childcare Prices — less interpolation and better coverage than most other states.

## Methodology

| Stage | Description |
|---|---|
| Data Selection | Filtered National Database of Childcare Prices to Pennsylvania; assessed data completeness across counties and care types |
| Exploratory Analysis | Examined county-level cost distributions for center-based vs. family-based care across infant, toddler, and preschool age groups |
| Dashboard Design | Built Tableau dashboards with calculated fields (% of income spent on childcare), toggle parameters, LOD expressions for annualized price trends, and employment context |
| Storytelling | Synthesized findings into a county-specific expansion recommendation supported by trend analysis and affordability metrics |

## Key Findings

- **Center-based care is consistently more expensive** than family-based care across all age groups and counties.
- **Center-based prices are rising faster**: center-based preschool costs increase ~$2.82/week per year vs. ~$1.61 for family-based care.
- Counties where childcare consumes the highest share of household income:
  - **Philadelphia County**
  - **Mercer County**
  - **Centre County**
- Mercer County shows particularly steep price growth (~$5.90/week per year), amplifying affordability pressure.
- These markets represent strong demand signals for a lower-cost childcare provider.

## Interactive Dashboard

The final Tableau dashboard is published on Tableau Public:

[View Live Dashboard](https://public.tableau.com/views/ChildCareIncomespendproject/ExpansionDashboard?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Project Structure

```
childcare-analysis.twbx              — Tableau packaged workbook (final dashboard)
childcare-analysis-presentation.pdf  — Final presentation slides (complete)
childcare-analysis-infographic.pdf   — Infographic poster
assets/
  infant.svg                         — Icon: infant age group
  toddler.svg                        — Icon: toddler age group
  preschool.svg                      — Icon: preschool age group
README.md
```

## Technologies

| Tool | Purpose |
|---|---|
| Tableau Desktop / Tableau Public | Interactive dashboards, calculated fields, LOD expressions, trend lines |
| Microsoft Excel | Data preparation and exploratory mockups |

## Academic Context

Completed as the final project for **DSC 640: Data Visualization** at Bellevue University. The course emphasized data storytelling, dashboard design, and communicating analytical findings to business audiences.

---

*Data science portfolio project by Martin Hoehler — [github.com/mhoehler22](https://github.com/mhoehler22)*
