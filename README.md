# AI Job Market Analysis — 2025–2026

The AI job market changes quickly, and there are plenty of opinions about which roles are growing, what skills employers want, and whether AI jobs actually pay more.

Instead of relying on headlines, I wanted to look at the job-posting data and see what patterns were actually visible.

This project uses **Python and exploratory data analysis** to examine salary, experience, skills, job type, remote work, LLM-focused roles, company characteristics, and hiring trends across AI job postings from **2025 and 2026**.

---

## Questions I Wanted to Answer

The analysis was built around a few practical questions:

* Which AI roles are hiring the most?
* How strongly does experience level affect salary?
* Do LLM-focused roles actually pay more?
* Does remote work affect compensation?
* Which technical skills appear most often in job postings?
* Which roles are growing fastest?
* Which industries offer stronger compensation and benefits?
* Is AI hiring still growing year over year?

---

## Dataset

The dataset contains AI job postings from **2025 and 2026** and includes information about:

* Job title
* Annual salary
* Experience level
* Education requirement
* Country
* Company size
* Industry
* Remote / hybrid / on-site work
* LLM role indicator
* Hiring demand score
* Benefits score
* Year-over-year demand growth
* Required skills
* Posting month and year

The dataset is included in the repository as:

`ai_jobs_market_2025_2026.csv`

---

## Tools Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**

---

# Analysis Workflow

I worked through the analysis in a fairly straightforward sequence:

**Load Data → Validate → Clean → Explore → Compare → Visualize → Interpret**

### 1. Data Validation

Before looking for patterns, I checked the structure and quality of the dataset.

This included:

* Reviewing column types
* Checking missing values
* Checking duplicate records
* Inspecting categorical values
* Looking at numerical distributions

The goal was to make sure the later comparisons were based on a dataset that had been properly understood first.

---

### 2. Exploratory Data Analysis

I explored both numerical and categorical variables to understand how the AI job market is distributed across:

* Job roles
* Experience levels
* Countries
* Industries
* Company sizes
* Work arrangements
* LLM vs non-LLM roles

---

### 3. Salary Analysis

Salary was one of the main parts of the analysis.

I compared compensation across:

* Job titles
* Experience levels
* Countries
* Education levels
* Company sizes
* Remote / hybrid / on-site roles
* LLM vs non-LLM positions

One of the clearest patterns was the difference in compensation between experience levels.

---

### 4. LLM vs Non-LLM Roles

With LLM-specific roles becoming increasingly common, I wanted to see whether there was a measurable salary difference.

I compared LLM and non-LLM positions across experience levels rather than looking only at their overall averages.

The analysis showed a **consistent salary premium for LLM-focused roles in this dataset**.

---

### 5. Remote Work Analysis

I compared salaries across:

* Remote
* Hybrid
* On-site

roles.

The results challenged the assumption that remote AI positions necessarily come with lower compensation.

In this dataset, remote roles remained salary-competitive with on-site positions.

---

### 6. Skill Demand

I extracted and analyzed the skills listed in job postings to identify the most frequently requested technical skills.

The analysis highlighted **Python, machine learning, and cloud technologies** among the most common requirements.

This was particularly useful from a career perspective because it connects job-market data with practical decisions about what skills to prioritize.

---

### 7. Hiring Growth

I compared job-posting activity between 2025 and 2026 to understand whether hiring demand was increasing or slowing down.

The monthly comparison showed that posting volumes in 2026 were higher across most months represented in the dataset.

---

### 8. Fastest-Growing Roles

I also compared year-over-year demand growth to identify roles experiencing stronger increases in hiring activity.

This helped distinguish between:

**roles with high current demand**

and

**roles whose demand is growing quickly.**

Those are not necessarily the same thing.

---

# Key Findings

### Experience remains a major salary factor

Experience level showed one of the strongest relationships with compensation. Senior and executive roles consistently earned more than entry-level positions across the job titles examined.

### LLM-focused roles command a premium

LLM-focused positions showed higher compensation than comparable non-LLM AI roles across experience levels in this dataset.

This suggests that specialized LLM skills were being rewarded in the sampled job market.

### Python, ML and cloud skills are highly requested

These skills appeared repeatedly across job postings and can be considered core requirements rather than niche differentiators for many AI roles.

### Remote work is not automatically associated with lower pay

Remote roles remained competitive with on-site positions in the dataset.

The difference appears to be influenced by the types of companies and roles represented in the data rather than remote work alone.

### AI hiring continued to grow in the dataset

Job-posting volumes increased across most comparable months between 2025 and 2026, suggesting continued hiring activity rather than a clear market slowdown.

---

# Analysis Sections

| Section              | Purpose                                           |
| -------------------- | ------------------------------------------------- |
| Data Validation      | Understand data quality and structure             |
| EDA                  | Explore distributions and patterns                |
| KPI Analysis         | Summarize the overall job market                  |
| Job Title Analysis   | Identify frequently posted roles                  |
| Salary Analysis      | Compare compensation                              |
| Salary Drivers       | Examine factors associated with pay               |
| Work Arrangement     | Compare remote, hybrid and on-site roles          |
| LLM Analysis         | Compare LLM and non-LLM positions                 |
| Skill Analysis       | Find frequently requested skills                  |
| Demand Analysis      | Compare hiring demand                             |
| Growth Analysis      | Identify fast-growing roles                       |
| Industry Analysis    | Compare industries                                |
| Correlation Analysis | Examine relationships between numerical variables |

---

# What This Project Shows

Beyond the charts, this project helped me practice the process of taking a relatively messy business question and turning it into a structured analysis.

The main skills I worked on were:

* Data validation and cleaning
* Pandas-based data manipulation
* Grouping and aggregation
* Working with categorical and numerical variables
* Extracting information from text-like skill fields
* Comparing multiple segments
* Building analytical visualizations
* Interpreting correlations carefully
* Turning EDA findings into practical conclusions

---

# Important Limitation

This analysis should not be treated as a complete representation of the global AI job market.

The results depend on the **job postings included in the dataset**, the countries and companies represented, and the way variables such as demand score and benefits score were defined.

In particular, salary comparisons should be interpreted as **patterns within this dataset**, not as universal salary benchmarks.

That distinction is important when using job-posting data to make career or hiring decisions.

---

# Repository Structure

```text
AI-JOB-MARKET/
│
├── AI_Job_Market.ipynb
├── ai_jobs_market_2025_2026.csv
└── README.md
```

---

## How to Run

Clone the repository and open:

```text
AI_Job_Market.ipynb
```

The notebook can be run using Jupyter Notebook or JupyterLab.

Required libraries:

```text
pandas
numpy
matplotlib
seaborn
jupyter
```

---

## Skills Demonstrated

**Python • Pandas • NumPy • Exploratory Data Analysis • Data Cleaning • Data Visualization • Statistical Exploration • Feature Analysis • Business Analysis**

---

## Author

**Jannat Chugh**

B.Tech ECE-AI | Data Analytics & Data Science

[GitHub](https://github.com/jannatchugh01) • [Portfolio](https://jannatchugh01.github.io/)
