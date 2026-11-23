# Milestone 05: AI-Assisted Financial Dashboard Prototype

**Course lab:** Lab 7: AI-built web page  
**Owner:** Braden Stein  
**Completed:** November 22, 2026

## What this milestone does
A working web proof-of-concept of one feature of the executive dashboard we recommend for WOC: comparing capital investment ROI **by location** and checking new purchase requests against past results before they're approved. It was built with an AI coding assistant across three versions, following the Lab 7 process (as-is → improved → innovative).

## Artifact(s) in this folder
| File | Version | What it shows |
|---|---|---|
| `index_v1.html` | v1: As-Is | WOC's current process: one spreadsheet per store, raw numbers, no ROI, no totals |
| `index_v2.html` | v2: Improved | All stores combined, automatic ROI and KPIs, filters, sorting, status flags (Strong / OK / Watch / Underperforming) |
| `index_v3.html` | v3: Executive Dashboard | KPI cards, ROI heatmap (asset type × location), net-profit chart, **"Should we buy this?" evaluator**, underperformer watchlist, auto-drafted executive summary |
| `woc_track_e_finance.csv` | Data | Track E dataset (400 investments, 2025) |
| `screenshot_v1.png` … `screenshot_v3.png` | Evidence | Screenshots of each version |

**To run:** open any `index_v*.html` in a browser. The pages load the CSV from this folder or from GitHub. If neither works, they ask you to pick the file.

## Key finding / decision
**Where an asset goes matters as much as what it is.** E-bikes average **+36% ROI at Downtown SLC** but about **−19% at Park City and Sandy**. High-end skis average **+75% at Park City** but **−33% Downtown**. Guided tour vans and store remodels lose money at every store. Overall, WOC invested **$11.0M** in 2025 and is **down $693K** year-to-date (−6.3% portfolio ROI), with **57%** of investments losing money.
→ WOC should require every capital request to go through a decision-support check like the v3 evaluator, so it buys the right assets for the right store.

## How AI was used
An AI assistant wrote the HTML/JavaScript from our process descriptions in each version. The team checked every figure against the CSV (net profit = revenue − maintenance − cost). The "executive summary" panel is rule-based in this prototype and stands in for an AI-written draft. It's labeled as a draft that the Finance Director must verify.

## Limitations
- Revenue and maintenance are **year-to-date**, so assets bought late in 2025 have had less time to earn back their cost.
- The data covers one year at three stores, so the evaluator shows historical patterns, not guarantees.

## How it connects
This is the live demo on **Slide 10** of the final presentation. It shows the dashboard recommended in Milestone 2 actually working, and the heatmap backs up the Tableau findings from Milestone 1.
