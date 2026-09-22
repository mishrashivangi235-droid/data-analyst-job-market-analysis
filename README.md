# Data Analyst Job Market Analysis

## Project Overview

This project analyzes Data Analyst job postings to identify patterns in skill demand, job levels, work types, geographic distribution, skill combinations, and job-description keywords.

The analysis uses Python, Pandas, NumPy, Matplotlib, Seaborn, and SQLite to clean, analyze, visualize, and query the job-posting dataset.

The project was developed as part of an IBM SkillsBuild Data Analytics with AI Internship project.

## Objectives

The main objectives of this project are to:

- Identify frequently demanded skills for Data Analyst roles.
- Analyze the demand for core skills such as SQL, Python, Excel, Power BI, and Tableau.
- Identify skills that frequently occur together.
- Analyze job postings by job level.
- Compare skill requirements across job levels.
- Analyze Onsite, Hybrid, and Remote work arrangements.
- Explore the geographic distribution of job postings.
- Compare work types across major search locations.
- Identify frequently occurring keywords in job descriptions.

## Dataset

The project uses a Kaggle dataset containing Data Analyst job postings.

The dataset contains **12,894 job postings** and includes information such as:

- Job title
- Company
- Job location
- First seen date
- Search city
- Search country
- Job level
- Job type
- Job summary
- Job skills

The dataset represents a **single-date snapshot from December 20, 2023** and contains postings from four countries: United States, United Kingdom, Canada, and Australia.

## Research Questions

The project addresses the following questions:

1. Which skills are most frequently demanded in Data Analyst job postings?
2. How frequently are core skills such as SQL, Python, Excel, Power BI, and Tableau mentioned?
3. Which skills commonly occur together?
4. What is the distribution of job postings across job levels?
5. How do skill requirements vary by job level?
6. What is the distribution of Onsite, Hybrid, and Remote work arrangements?
7. Do skill requirements vary by work type?
8. Which countries and search locations have the most postings?
9. How does work type vary across major search locations?
10. Which important keywords are most frequent in job descriptions?

## Tools and Technologies

- **Python** — Data analysis and preprocessing
- **Pandas** — Data manipulation and analysis
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Seaborn** — Statistical visualization
- **SQLite** — SQL-based data analysis
- **Jupyter Notebook** — Analysis workflow and documentation
- **Git & GitHub** — Version control and project sharing

## Project Structure

```text
data-analyst-job-market-analysis/
│
├── data/
│   ├── raw/
│   │   └── postings.csv
│   └── processed/
│       └── cleaned_postings.csv
│
├── notebooks/
│   └── 01_data_analysis.ipynb
│
├── src/
│
├── outputs/
│
├── requirements.txt
└── README.md
```

### Folder Description

- `data/raw/` — Original dataset
- `data/processed/` — Cleaned dataset generated during the analysis
- `notebooks/` — Jupyter Notebook containing the complete analysis
- `src/` — Space for reusable Python scripts
- `outputs/` — Space for generated charts or other project outputs
- `requirements.txt` — Python dependencies required to run the project
- `README.md` — Project documentation

## Analysis Workflow

The project follows the following data analysis workflow:

1. **Data Loading**
   - Load the raw CSV dataset using Pandas.

2. **Data Inspection**
   - Examine dataset dimensions, column names, data types, missing values, duplicates, and descriptive statistics.

3. **Data Cleaning**
   - Standardize column names.
   - Handle missing values in text fields.
   - Remove unnecessary whitespace.
   - Convert the date field into a proper datetime format.
   - Create year, month, and month-name features.
   - Validate the cleaned dataset.

4. **Exploratory Data Analysis**
   - Analyze job levels and work types.
   - Explore geographic distributions.
   - Analyze frequently demanded skills.
   - Compare core skills across job levels and work types.
   - Analyze skill co-occurrence.
   - Extract frequently occurring keywords from job descriptions.

5. **SQL Analysis**
   - Load the cleaned dataset into a SQLite database.
   - Use SQL queries to analyze job levels, work types, countries, locations, and skill patterns.

6. **Visualization**
   - Create charts using Matplotlib and Seaborn to communicate important findings.

7. **Interpretation**
   - Summarize the main findings and document limitations of the dataset.

## Key Findings

The analysis produced the following key findings:

- Data Analysis and SQL are among the most frequently mentioned skills in the dataset.
- Among the selected core skills, SQL has the highest normalized skill count, followed by Tableau, Excel, Python, and Power BI.
- Data Analysis + SQL is the most frequently occurring skill pair, followed by Python + SQL and SQL + Tableau.
- Mid-senior positions account for 75.16% of the job postings, while Associate positions account for 24.84%.
- Onsite postings represent 51.73% of the dataset, followed by Hybrid at 33.65% and Remote at 14.62%.
- The United States accounts for 80.55% of the postings, followed by the United Kingdom, Canada, and Australia.
- Work-type distributions vary across countries and major search locations.
- Frequently occurring job-description keywords include data, business, management, support, analysis, analyst, information, systems, and technical.

## Limitations

- The dataset is a single-date snapshot from December 20, 2023.
- The dataset contains postings from only four countries.
- The dataset may not represent the complete global Data Analyst job market.
- The `search_city` field contains both cities and broader geographic areas.
- Keyword counts represent word occurrences rather than unique job postings.
- Different representations of similar skills may appear as separate skill terms.
- SQL skill counts using text matching may differ from normalized Python-based skill counts.

## How to Run the Project

### 1. Clone the repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd data-analyst-job-market-analysis
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Open the Jupyter Notebook

```bash
jupyter notebook
```

Then open:

```text
notebooks/01_data_analysis.ipynb
```

### 4. Run the notebook

Run the notebook cells from top to bottom to reproduce the data cleaning, exploratory analysis, visualizations, and SQL analysis.

## Project Outputs

The project produces:

- Cleaned job-posting dataset
- Exploratory data analysis
- Data visualizations
- Skill demand analysis
- Skill co-occurrence analysis
- Geographic analysis
- Job-description keyword analysis
- SQLite database and SQL analysis
- Key findings and documented limitations

## Author

This project was developed as part of the IBM SkillsBuild Data Analytics with AI Internship (2026 Cohort).

The project demonstrates practical skills in data cleaning, exploratory data analysis, visualization, SQL analysis, and data interpretation using a real-world job-posting dataset.