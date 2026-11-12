# TaskRabbit Earnings Analysis

## Project Overview
Analysis of 4 years of personal TaskRabbit earnings data to optimize gig economy performance and provide insights for platform improvement.

## Key Questions
1. How can TaskRabbit reduce earnings volatility to improve tasker retention?
2. What pricing and client selection strategies maximize gig economy profitability?

## Project Status
Analysis complete. Review sentiment dashboard, which is a spinoff project, is now built.

## Data
- **Time Period:** 2022-2025
- **Total Transactions:** ~488 (484 are valid)
- **Markets:** NYC and Boston

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
├── visualizations/       # Charts and dashboards
└── presentations/        # Slide decks
```

**Result:** Raising my hourly rate 25% did not reduce client satisfaction. Clients are paying for trust and reliability, not the lowest price.

| Finding | Evidence |
|---|---|
| Yield over volume works | +25% hourly rate after shifting from job count to $/hour |
| Higher rates did not hurt satisfaction | No link between rate and tip % (p = 0.47) |
| Premium demand is predictable | Category explains 57% of feature importance, location 28%, timing 15% |
| Best premium categories | Packing, Photography, Computer Help |
| Best premium windows | NYC weekends (+20%), Boston Mondays and Tuesdays |

**What premium categories share:** they are expertise-driven, trust-dependent, time-sensitive, and costly if done wrong. Clients pay for certainty.

**Product recommendation: "TaskRabbit Select."** A premium tier that matches clients to top-rated Taskers automatically, with pre-screening (parking, pets, schedule, gender preference) instead of browsing profiles and messaging back and forth. Proposed pilot: NYC weekends, top 5% of Taskers, 20 to 30% rate premium, measured on opt-in rate, booking conversion, satisfaction, and revenue per hour against a control group.

📊 [Slide deck](https://data-laur.github.io/taskrabbit-gtm.pdf) · [Tableau dashboard](https://public.tableau.com/app/profile/lauren.chagaris/viz/TaskrabbitAnalysis-SampleFindings/MarketAnalysisDashboard)

## Contact
Lauren Chagaris
www.linkedin.com/in/lchagaris
datalaur@bu.edu
