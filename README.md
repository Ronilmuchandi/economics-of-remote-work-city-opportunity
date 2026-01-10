The Economics of Remote Work: City-Level Opportunity & Fragility (U.S.)
Executive Summary

Remote work has reshaped where people live and work—but growth in remote jobs does not always translate into sustainable city-level opportunity.
This project analyzes U.S. metropolitan areas (MSAs) to distinguish true opportunity from structural fragility, combining labor demand, migration flows, and cost-of-living pressures into interpretable economic indicators.

The key contribution is the Remote Work Fragility Index (RWFI), which flags cities experiencing rapid growth paired with rising costs and unstable migration—separating hype from long-term viability.

Problem Statement

Most discussions around “best cities for remote work” rely on rankings or demand alone, ignoring affordability and migration stability.

This project answers:

Which U.S. cities offer sustainable remote-work opportunity, not just short-term growth?

Where is remote-work growth structurally fragile due to cost pressure and mobility volatility?

How do opportunity patterns differ regionally and structurally, not just city-by-city?

Data Sources

City- and metro-level datasets were aggregated and standardized, including:

Remote job postings and labor demand

In-migration and out-migration flows

Cost-of-living components (housing, food, transportation, taxes, etc.)

Median family income

All datasets were cleaned, merged, and locked prior to analysis to ensure reproducibility.

Methodology (End-to-End Pipeline)

Step 1–2: Data loading, cleaning, aggregation
Step 3: Exploratory Data Analysis (EDA)
Step 4: Feature engineering (economic indices)
Step 5: Modeling & structural analysis
Step 6: Validation, robustness checks, regime classification

Each step is implemented in a dedicated notebook to maintain clarity and auditability.

Key Indices (Core Contributions)

Remote Work Demand Index (RWDI)
Measures relative intensity of remote job demand by city.

Cost-Adjusted Attractiveness Score
Evaluates opportunity after accounting for cost-of-living pressure.

Mobility Intensity Score (MIS)
Captures migration churn and population movement dynamics.

Remote Work Opportunity Index (RWOI)
Composite indicator of demand and affordability.

⭐ Remote Work Fragility Index (RWFI) (Signature Feature)
Identifies cities with:

Fast demand growth

Rising cost pressure

Unstable migration patterns

RWFI highlights where growth may be unsustainable, even when demand appears strong.

Key Findings

Remote work demand alone is a weak signal without affordability and migration context.

Several high-growth MSAs show elevated fragility, driven by housing costs outpacing income growth.

Some mid-tier cities exhibit lower hype but higher sustainability, offering more resilient opportunity.

State-level aggregation reveals regional regimes, not a uniform national pattern.

Visual Evidence

This repository includes static visualizations illustrating:

Opportunity vs. Fragility trade-offs across MSAs

State-level regime classifications (Stable / Neutral / Fragile)

Cluster-based city archetypes

These visuals support decision-oriented interpretation, not rankings.

Why This Project Matters

This analysis reframes remote work from a ranking problem to a sustainability problem.

Use cases:

Job seekers: identify cities with durable opportunity, not just short-term hype

Employers: understand labor-market risk when expanding remote hiring

Policy analysts: detect regions vulnerable to cost-driven displacement

The framework translates economic theory into measurable decision metrics.

Limitations & Next Steps

Analysis is limited to available job posting and migration data windows.

Time-series depth can be expanded for stronger causal inference.

Future work could integrate wage distributions, firm-level data, or zoning constraints.

Repository Structure
economics-of-remote-work-city-opportunity/
│
├── 00_project_notes.ipynb
├── 01_data_loading.ipynb
├── 02_eda.ipynb
├── 03_feature_engineering.ipynb
├── 04_modeling_analysis.ipynb
├── 05_evaluation_validation.ipynb
│
├── data/
│   ├── raw/
│   └── processed/
│
└── visuals/

Skills Demonstrated

Economic feature engineering

City-level labor market analysis

Migration & cost-pressure modeling

Interpretable index design

Executive-ready analytical communication

✅ Project Status

Analysis complete. Dataset locked. Results validated.
