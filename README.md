# Proposing New Child Care Centers in Pennsylvania

### A data-driven expansion proposal for a childcare franchise, built with Tableau

---

## Overview

This project takes the perspective of an executive at a childcare franchise company building a data-driven case for expanding into the Pennsylvania market. Using federal childcare cost data, the analysis identifies which Pennsylvania counties present the strongest opportunity: places where center-based childcare prices are high, rising fast, and consuming a disproportionate share of household income — exactly the conditions where a competitive new provider has the most to offer.

The analysis surfaces three target counties — **Philadelphia, Mercer, and Centre** — and packages the findings into three deliverables aimed at two different audiences.

Pennsylvania was specifically chosen because its county-level data is unusually complete, with less interpolation than most other states in the National Database of Childcare Prices.

## The Proposal

Center-based childcare costs in Pennsylvania are not only high — they are growing faster than family-based care, and the gap is most severe in select counties:

| County | Why it was selected |
|---|---|
| **Philadelphia** | Highest absolute childcare costs relative to county median income |
| **Mercer** | Steepest price growth (~$5.90/week per year for center-based preschool); affordability under severe pressure |
| **Centre** | Among the highest "% of income needed for childcare" scores statewide |

The core finding driving the recommendation: **center-based preschool prices are rising ~$2.82/week per year statewide** — nearly double the $1.61/week annual increase for family-based care. A franchise entering at 10% below the county median would be well-positioned in each of these markets.

## Deliverables & Audiences

Three outputs were produced for two distinct audiences:

| Deliverable | Audience | Purpose |
|---|---|---|
| **Interactive Dashboard** | Management teams | Explore all Pennsylvania counties; drill into affordability metrics, price trends, and employment context for any county |
| **Presentation** | Executive leadership | Formal proposal naming the three target counties and the data case for each |
| **Infographic Poster** | All employees | Internal announcement generating excitement about the new markets — less technical, more motivational |

## Analytical Approach

| Stage | Description |
|---|---|
| Data Selection | Filtered National Database of Childcare Prices to Pennsylvania for data quality; assessed completeness of county-level records |
| EDA | Compared center-based vs. family-based costs across infant, toddler, and preschool age groups; built "% of household income needed for childcare" as a calculated field with a toggle parameter |
| Trend Analysis | Used Tableau trend lines to quantify annualized price increases (slope × 365); isolated Mercer County as an outlier in price growth |
| LOD Calculations | Replaced manual slope calculations with Fixed Level of Detail expressions for accuracy and repeatability; multiplied weekly slope × 52 for annual figures |
| Recommendation | Ranked counties by affordability pressure and price trajectory; selected three with the strongest case for a competitive new entrant |

## Design Decisions

The dashboard and presentation share a deliberate two-color palette:
- **Red** highlights the selected county name, making it immediately clear which county is in focus as selections change
- **Blue gradients** represent quantitative measures across all other elements

The infographic uses a different palette — **blue + magenta** — because it targets a different audience. Red can read as "error" or "stop," which is the wrong tone for an employee announcement. Magenta carries a hint of urgency (used to flag the high-cost problem) while blue represents the company. The intent is for employees to read the color contrast as: *our company is the solution to the childcare struggles these communities face.*

The same infant, toddler, and preschool icons appear in both the dashboard and the presentation, creating a consistent visual vocabulary across both management-facing materials.

## Project Structure

```
childcare-analysis.twbx              — Tableau packaged workbook (interactive dashboard)
childcare-analysis-presentation.pdf  — Executive proposal presentation (complete, with appendix)
childcare-analysis-infographic.pdf   — Employee announcement infographic
childcare-expansion-whitepaper.pdf   — Written analysis: methodology, assumptions, design rationale
assets/
  infant.svg                         — Icon: infant age group
  toddler.svg                        — Icon: toddler age group
  preschool.svg                      — Icon: preschool age group
README.md
```

## Interactive Dashboard

The final Tableau dashboard is published on Tableau Public:

[View Live Dashboard](https://public.tableau.com/views/ChildCareIncomespendproject/ExpansionDashboard?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Technologies

| Tool | Purpose |
|---|---|
| Tableau Desktop / Tableau Public | Dashboard design, calculated fields, LOD expressions, trend line analysis |
| Microsoft Excel | Data preparation and exploratory mockups |

## Academic Context

Completed as the final project for **DSC 640: Data Visualization** at Bellevue University. The course emphasized translating data into actionable business narratives — moving from descriptive reporting toward analytical storytelling aimed at real decision-makers.

---

*Data science portfolio project by Martin Hoehler — [github.com/mhoehler22](https://github.com/mhoehler22)*
