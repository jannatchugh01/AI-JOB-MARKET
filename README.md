# AI Job Market Analysis, 2025–2026

Everyone has an opinion on which AI roles are hot, what skills to learn, and whether AI jobs really pay more. I wanted to see what job-posting data actually says, so I analyzed 1,500 AI job postings in Python and wrote up what I found, including the places where the data didn't behave.

---

## Questions I set out to answer

1. How much does experience level affect salary?
2. Do LLM-focused roles pay more than other AI roles?
3. Does remote work change compensation?
4. Which skills show up most often in postings?
5. Which roles and industries stand out on demand and pay?
6. Is AI hiring still growing?

---

## Dataset

- **Source:** [AI Jobs Market 2025–2026 (Kaggle, by alitaqishah)](https://www.kaggle.com/datasets/alitaqishah/ai-jobs-market-2025-2026-salaries)
- **Size:** 1,500 postings across 25 AI job titles
- **Time span:** January–December 2025 (624 postings) and January–March 2026 (876 postings)
- **Fields include:** job title, annual salary (USD), experience level, education, country, company size, industry, work arrangement, LLM-role flag, demand score, benefits score, required skills, posting month and year

The Kaggle page doesn't explain how the postings were collected, so I ran some consistency checks before analyzing anything (see [Data quality notes](#data-quality-notes)).

---

## How I approached it

Load → check data quality → explore → compare segments → visualize → interpret.

I used **Python, pandas, NumPy, Matplotlib, and Seaborn** in a Jupyter notebook. The analysis covers salary by experience, education, country, company size, and work arrangement, LLM vs non-LLM roles, skill frequency (parsed from the skills column), hiring trends by month, and correlations between the numeric fields.

---

## What I found

**Experience is the biggest salary driver I could see.**
Median pay rises steadily with experience, from roughly $145K for entry-level roles to roughly $238K for lead roles.

**Location and company size matter a lot too.**
Average salary is highest in the USA (about $226K) and lowest in India (about $133K). Big Tech postings average about $238K, compared with about $168K at startups.

**Python is in nearly two-thirds of postings.**
Python appears in 942 of 1,500 postings (63%), followed by SQL (452, 30%) and cloud skills (429, 29%). Statistics and PyTorch also rank in the top 12. "Machine learning" did not appear as a separate skill tag in the top 20.

**No single job title dominates.**
LLM Engineer is the most-posted title with 75 postings (5% of the data), and Computer Vision Engineer is the least with 46. Demand is spread fairly evenly across the 25 titles.

**LLM roles vs other AI roles.**
LLM roles offer a median annual salary of $191,000 compared to $180,000 for other AI roles, representing an 6.11% salary premium ($11,000).

**Hiring trend: I'm cautious about this one.**
The dataset has 876 postings for January–March 2026 versus 148 for January–March 2025. That looks like a huge jump, but 2026 covers only three months and its volume is far above the 2025 monthly average of about 52 postings. I read this as a feature of how the dataset was assembled, not as evidence that hiring grew sixfold, so I don't draw a growth conclusion from it.

---

## Limitations

- The results describe **patterns within this dataset**, not the global AI job market or verified salary benchmarks.
- The dataset documentation doesn't say how postings were sourced or how fields like demand score and benefits score were calculated.
- 2026 contains only three months of data, so year-over-year comparisons are limited.
- Salaries are listed in USD for every country, so cross-country comparisons say little about local purchasing power or local market norms.

---

## Repository contents

```text
AI-JOB-MARKET/
├── AI_Job_Market.ipynb
├── ai_jobs_market_2025_2026.csv
├── requirements.txt
└── README.md
```

## Running it

```bash
git clone https://github.com/jannatchugh01/AI-JOB-MARKET.git
cd AI-JOB-MARKET
pip install -r requirements.txt
jupyter notebook AI_Job_Market.ipynb
```

---

## Author

**Jannat Chugh** — B.Tech ECE (AI), aspiring data analyst
[GitHub](https://github.com/jannatchugh01) · [Portfolio](https://jannatchugh01.github.io/)
