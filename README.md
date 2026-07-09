# AI Job Market Analysis (2025–2026)

An exploratory data analysis of AI job postings across multiple countries, industries, and role types — built to understand what's actually happening in the AI hiring market right now, not just what the headlines say.

---

## What this is

I put this together after noticing a lot of conflicting takes on the AI job market — some saying demand is exploding, others saying it's cooling. Rather than guess, I figured I'd look at the data.

The notebook walks through salary drivers, skill requirements, remote work trends, and the growing premium on LLM-specific roles. It's not meant to be a definitive study, but it surfaces some patterns worth knowing about if you're hiring, job hunting, or just curious about where the market is heading.

---

## What's inside

```
ai-job-market-analysis/
│
├── AI_Job_Market.ipynb              # Main analysis notebook
├── ai_jobs_market_2025_2026.csv     # Dataset 
└── README.md
```

---

## Key findings

A few things stood out from the analysis:

- **Experience level is the biggest salary driver** — bigger than country, company size, or education level. The gap between entry-level and senior roles is substantial across every job title.
- **LLM roles pay more, consistently** — not by a small margin either. Roles focused on large language models (fine-tuning, RLHF, prompt engineering at scale) show a clear salary premium over comparable non-LLM AI roles at every experience level.
- **Remote doesn't mean a pay cut** — fully remote AI roles are salary-competitive with on-site positions in this dataset. The assumption that remote work comes with a pay penalty doesn't hold here, likely because remote AI roles skew toward larger, better-funded companies.
- **Python, ML, and cloud are table-stakes** — they appear in more postings than any other skills by a wide margin. If you're upskilling, those three are the floor, not a differentiator.
- **Hiring is still growing year-over-year** — posting volumes in 2026 are up across most months compared to 2025. The market hasn't plateaued.

---

## Analysis sections

| Section | What it covers |
|---|---|
| Data loading & validation | Schema review, null checks, duplicate detection |
| EDA | Distributions across numeric and categorical columns |
| KPI dashboard | Headline metrics — total postings, avg/median salary, remote %, LLM role % |
| Job title distribution | Which roles are hiring most |
| Salary by job title | Average compensation per role |
| Salary drivers | Experience, education, country, and company size compared |
| Work arrangement | Remote vs hybrid vs on-site salary comparison |
| LLM vs non-LLM roles | Salary premium for LLM-focused positions |
| Demand score | Which roles and industries are most actively competing for talent |
| Fastest-growing roles | Top 10 by year-over-year posting growth |
| Benefits by industry | Which sectors offer the strongest total compensation packages |
| Job posting trend | Month-by-month comparison: 2025 vs 2026 |
| In-demand skills | Top 20 skills across all postings |
| Correlation analysis | Relationships between salary, demand, benefits, and role type |

---

## Requirements

```
pandas
numpy
matplotlib
seaborn
jupyter
```

---

## Dataset

Source: Kaggle
The dataset (`ai_jobs_market_2025_2026.csv`) covers AI job postings from 2025 and 2026 and includes the following columns:

| Column | Description |
|---|---|
| `job_title` | Role name |
| `annual_salary_usd` | Advertised annual salary in USD |
| `experience_level` | Entry / Mid / Senior / Executive |
| `education_required` | Minimum education requirement |
| `country` | Country of the posting |
| `company_size` | Small / Medium / Large |
| `industry` | Industry sector |
| `remote_work` | Remote / Hybrid / On-site |
| `is_llm_role` | 1 if role is primarily LLM-focused, 0 otherwise |
| `demand_score` | Composite hiring demand index (0–10) |
| `benefits_score_10` | Employer benefits quality score (0–10) |
| `demand_growth_yoy_pct` | Year-over-year % change in postings for that role |
| `required_skills` | Pipe-delimited list of required skills |
| `posting_month` | Month of posting |
| `posting_year` | Year of posting (2025 or 2026) |

---

## Tools used

- **pandas** — data wrangling and aggregations
- **numpy** — numerical operations
- **matplotlib** — charts and subplots
- **seaborn** — statistical visualisations and the correlation heatmap

---


## Contributing

If you spot something off, have a better way to approach part of the analysis, or want to add a section — open an issue or submit a PR. Happy to review.

---
