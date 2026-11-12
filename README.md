# TaskRabbit Earnings Analysis: Yield Over Volume

## Project Overview

I've worked as a Tasker in Boston and NYC since 2018. In late 2023 I changed strategy: fewer jobs, higher rates, and a focus on premium services like photography, computer help, and packing. This project uses 3.5 years of my own transaction data to test whether that shift worked, what it cost, and what it suggests TaskRabbit could build.

The analysis led to a product proposal, **TaskRabbit Select**: a premium tier that matches clients with top-rated Taskers automatically, built around the demand patterns found here.

## Key Questions

1. Can a Tasker raise rates without losing demand or client satisfaction?
2. Which categories, locations, and times command premium rates?
3. What does a shift from volume to value do to earnings stability?

## Project Status

Analysis complete. A dashboard is built in Tableau, along with a spinoff deployed app, a review sentiment dashboard which incorporates text mining.

## Data

- **Source:** My own TaskRabbit transaction and review records
- **Time period:** April 2022 to November 2025
- **Transactions:** 488 total, 484 valid after cleaning
- **Markets:** Boston area and NYC
- **Strategy shift:** October 2023, used to split the data into before and after

## Technologies
- Python (Pandas, NumPy, Scikit-learn)
- Jupyter Notebooks
- Tableau Public
- Statistical Analysis & Machine Learning

## Project Structure
```
taskrabbit-analysis/
├── data/
│   ├── raw/              # Original CSV files
│   └── processed/        # Cleaned datasets
├── notebooks/            # Jupyter analysis notebooks
└──visualizations/       # Charts and dashboards
```

## Key Findings

**Data:** 484 valid transactions, April 2022 to November 2025, Boston and NYC. Strategy shift in October 2023: fewer, higher-value jobs instead of maximizing volume.

**Result:** I worked less and earned more. My hourly rate rose 25% with no drop in client satisfaction. Clients pay for trust and reliability, not the lowest price.

| Metric | Before (2022 to Q3 2023) | After (Q4 2023 to 2025) | Change |
|---|---|---|---|
| Average hourly rate | $56 | $70 | +25% |
| Jobs per week | 3.7 | 2.7 | -27% |
| Average weekly earnings | $535 | $561 | +4.8% |
| Weekly earnings volatility (CV) | 68.8% | 72.7% | +3.9 pts |
| Average tip | $26.35 | $38.12 | +45% |
| Median tip % | 20% | 15% | -5 pts |

**Volatility tradeoff:** income became slightly less predictable week to week, because premium jobs are less frequent. I accepted that in exchange for higher earnings per hour worked. Someone who needs steady income would weigh this differently.

**Tip paradox:** tip percentage fell, but tip dollars rose 45%, because the base price was higher. Rates showed no meaningful link to tip % (p = 0.47).

**Where premium demand lives:**
- Category drives most of it (57% of feature importance), then location (28%) and timing (15%)
- Photography was the top service in both markets ($112/hr Boston, $89/hr NYC)
- Boston paid 30% more per hour than NYC overall ($69 vs $53)
- NYC weekends paid 20% more than NYC weekdays

**Product recommendation: "TaskRabbit Select."** A premium tier that automatically matches clients to top-rated Taskers, with pre-screening (parking, pets, schedule, gender preference) instead of browsing and messaging. Proposed pilot: NYC weekends, top 5% of Taskers, 20 to 30% rate premium, measured against a control group on opt-in, booking conversion, satisfaction, and revenue per hour.

📊 [Slide deck](https://data-laur.github.io/taskrabbit-gtm.pdf) · [Tableau dashboard](https://public.tableau.com/app/profile/lauren.chagaris/viz/TaskrabbitAnalysis-SampleFindings/MarketAnalysisDashboard)

**What premium categories share:** they are expertise-driven, trust-dependent, time-sensitive, and costly if done wrong. Clients pay for certainty.

**Product recommendation: "TaskRabbit Select."** A premium tier that matches clients to top-rated Taskers automatically, with pre-screening (parking, pets, schedule, gender preference) instead of browsing profiles and messaging back and forth. Proposed pilot: NYC weekends, top 5% of Taskers, 20 to 30% rate premium, measured on opt-in rate, booking conversion, satisfaction, and revenue per hour against a control group.

📊 [Slide deck](https://data-laur.github.io/taskrabbit-gtm.pdf) · [Tableau dashboard](https://public.tableau.com/app/profile/lauren.chagaris/viz/TaskrabbitAnalysis-SampleFindings/MarketAnalysisDashboard)

## Contact
Lauren Chagaris
www.linkedin.com/in/lchagaris
datalaur@bu.edu

## License
Code is MIT licensed. Data, findings, and slides © 2026 Lauren Chagaris. All rights reserved.
