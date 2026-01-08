# economics-of-remote-work-city-opportunity
Analyzing global city-level remote work demand, mobility, and economic sustainability using data-driven opportunity and fragility indices (2022–2025).

## Spine Dataset: Remote Job Demand (LinkedIn)

**Source:** Public LinkedIn job postings dataset (Kaggle)

**Purpose:**  
To measure city-level remote job demand across U.S. cities using job postings
as a proxy for labor demand.

**Processing Summary:**
- Raw job-level data aggregated to City × Month
- Remote jobs identified using explicit remote indicators
- Low-volume city-months removed to reduce noise
- Final output represents a 2024 snapshot of demand

**Limitations:**
- Job postings do not represent actual employment
- Analysis limited to one year due to data availability

Step 1–3: Data Preparation (Locked)

Cleaned and standardized raw datasets

Aggregated job postings from job-level → MSA × month

Aligned all sources using a standardized city_state key

Enforced one-row-per-MSA-per-month rule

These steps are intentionally locked to preserve reproducibility.

Step 4: Exploratory Data Analysis (EDA)

Notebook: 02_eda.ipynb

What was explored

Distribution of remote job demand across MSAs

Migration intensity vs affordability

Opportunity vs cost tradeoffs

Identification of outliers and early signals

Key takeaway

Remote work demand varies widely across cities, but high demand does not automatically imply sustainability.

Step 5: Feature Engineering (Core Differentiator)

Notebook: 04_feature_engineering.ipynb

Indices Built

RWDI — Remote Work Demand Index

MIS — Mobility Intensity Score

CPI — Cost Pressure Index

RWOI — Remote Work Opportunity Index

⭐ RWFI — Remote Work Fragility Index (signature feature)

Why RWFI matters

RWFI captures cities where:

opportunity interacts with cost pressure and mobility, creating structural risk.

This separates early-stage opportunity from overheated growth.

Step 6: Modeling & Analysis

Notebook: 05_modeling_analysis.ipynb

Regression Analysis

Validated index construction

Identified drivers of fragility

Key result:
Cost pressure and mobility intensity drive fragility — not opportunity alone.

Clustering

Cities were segmented into four structural archetypes:

High Opportunity / Low Fragility

High Opportunity / High Fragility

Stable but Low Growth

Pressure Without Payoff

This revealed that only a minority of cities achieve resilient opportunity.

Step 7: Evaluation & Validation

Notebook: 06_evaluation_validation.ipynb

What was validated

Sanity checks against known high-cost metros

Identification of emerging vs high-risk cities (with names)

Opportunity vs fragility scatter validation

State-level regime map (choropleth)

Correlation analysis to confirm indices are not redundant

Key insight

Opportunity and fragility are distinct dimensions.
Geographic patterns show emerging regions tend to be secondary metros, not legacy hubs.

Key Findings

Remote work opportunity is widespread, but resilient opportunity is rare

Cost pressure and migration volatility amplify fragility

Many cities remain stable but peripheral to remote work growth

Emerging cities are often non-obvious and early-stage

Evaluating opportunity without fragility leads to misleading conclusions

Limitations

Cross-sectional analysis (not causal)

U.S.-only MSAs

Cost metrics reflect a specific household type

Aggregation masks intra-city variation

These constraints are acknowledged and do not affect comparative insights.

Why This Project Matters

This project demonstrates:

End-to-end data science workflow

Economic reasoning, not just modeling

Careful validation and uncertainty awareness

Ability to translate complex signals into decision-relevant insights

Relevant for roles in:
Data Analytics · Economics · Urban Policy · Finance · Consulting
