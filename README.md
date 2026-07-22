# Fuel Queue & Price Tracker

**Status:** 🚧 In Progress — real data collection ongoing

## Problem
Fuel queues are a daily reality in Nigeria, but there's no public, structured data on patterns — when they're worst, which stations are more reliable, or how price relates to queue length. This project fills that gap with self-collected, real-world field data from Abraka, Delta State.

## Method
- Real observations logged via a Google Form by me and a small group of contributors, collected over several weeks
- While real data collection is ongoing, the analysis pipeline (cleaning, exploration, dashboard) is being built and tested on a clearly-labeled **synthetic dataset** so the project isn't blocked waiting on data volume
- Once enough real entries are collected, the synthetic file is swapped for the real dataset and the analysis is rerun

## Tools
Google Sheet → Python (pandas) → Power BI

## Repo Structure
```
fuel-queue-tracker/
├── README.md
├── .gitignore
├── data/
│   ├── SYNTHETIC_fuel_queue_data.csv   ← placeholder data for pipeline testing, NOT real
│   └── fuel_queue_observations.csv      ← real collected data (added once ready)
├── notebooks/
│   └── analysis.ipynb                   ← pandas cleaning + exploration
├── dashboard/
│   └── fuel_queue_dashboard.pbix        ← Power BI file (added once built)
└── src/
    └── clean_data.py                    ← reusable cleaning script
```

## Key Finding
*(to be added once analysis on real data is complete)*

## What's Next
- Continue real data collection
- Swap synthetic data for real data once volume is sufficient
- Build out Power BI dashboard
- Publish key finding + dashboard screenshot here
