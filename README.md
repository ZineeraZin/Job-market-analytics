# Job Market Analysis in India and the USA

**Analyzing job market trends, in-demand skills, advertised salaries, experience requirements, and remote-work opportunities to support data-driven career decisions.**

## Project Overview

The job market is constantly changing as employers seek different skills, qualifications, and levels of experience. Job seekers often find it difficult to understand which skills are most in demand, what salaries are advertised for different roles, and how employment opportunities vary between countries.

This project explores real-world job postings from India and the United States to understand job market patterns, skill requirements, advertised salary trends, and working arrangements.

Using the *Job Postings 2026: India and United States* dataset, the project aims to identify patterns across job titles, companies, professional roles, seniority levels, locations, required skills, experience, education, and salary information.

The goal is to transform a large collection of job advertisements into meaningful analytical insights that can help job seekers understand employer requirements and make more informed career and skill-development decisions.

## Business Problem

Job seekers may struggle to identify the skills employers are looking for, understand advertised salary differences across roles, and compare employment opportunities between India and the USA. Employers and career advisors may also benefit from understanding the characteristics of advertised positions across different locations and professional categories.

This project addresses the following question:

**What patterns can be identified in job opportunities, skill demand, advertised salaries, experience requirements, and remote-work arrangements in India and the USA?**

The analysis will compare the available job postings to identify trends and differences that may help people better understand the job market. The findings will be interpreted carefully, recognizing that job advertisements do not necessarily represent actual hires or the entire employment market.

## Project Objectives

- Analyze the distribution of job postings across India and the USA.
- Identify the most frequently requested skills in the available job advertisements.
- Explore job opportunities across professional roles, industries, companies, and locations.
- Compare advertised salaries across countries, roles, and experience levels where sufficient salary data is available.
- Examine the experience and education requirements specified in job postings.
- Investigate the distribution of on-site, remote, and hybrid opportunities where work-mode information is available.
- Explore the skills and qualifications requested in Data Analyst and related analytics positions.
- Develop interactive visualizations and dashboards to communicate findings.
- Provide evidence-based recommendations for job seekers planning their skill development.

## Dataset Information

| Attribute           | Details                                          |
| ------------------- | ------------------------------------------------ |
| Dataset             | Job Postings 2026: India and United States       |
| Source              | Fliar BI                                         |
| File format         | CSV                                              |
| Number of records   | 100,009                                          |
| Number of columns   | 17                                               |
| Countries covered   | India and the USA                                |
| Posting period      | January–June 2026                                |
| Unit of observation | Job posting                                      |
| Domain              | Human Resources Analytics / Job Market Analytics |

**Dataset source:** [https://fliarbi.com/datasets/job-postings-2026/](https://fliarbi.com/datasets/job-postings-2026/)

The dataset contains 100,009 job postings, including 19,994 records from India and 80,015 from the USA. Each row represents a job posting rather than a confirmed appointment or successful hire.

The dataset includes job titles, company names, locations, professional roles, seniority levels, required skills, experience requirements, education information, work arrangements, and advertised annual salary information where available.

### Key Fields

The following fields are relevant to the project:

- `posting_id` – Unique identifier for a job posting.
- `posted_date` – Date the job posting was published.
- `title` – Advertised job title.
- `company` – Name of the hiring company or organisation.
- `role` – Professional role category, where available.
- `seniority` – Seniority level, where available.
- `category` – Job category, where available.
- `city` – City associated with the posting.
- `region` – State or region associated with the posting.
- `country` – Country associated with the job posting.
- Work Mode – Recorded work arrangement, such as on-site, remote, or hybrid.
- `experience_years` – Experience requirement, where available.
- `education` – Education requirement, where available.
- `skills` – Skills mentioned in the job posting, where available.
- `salary_annual_usd` – Annual salary value expressed in US dollars, where available.
- `company_domain` – Company website domain, where available.
- `fliar_profile_url` – Associated company profile URL, where available.

## Tools and Technologies

- **Microsoft Excel** – Initial data inspection, cleaning, sorting, filtering, and summary analysis.
- **SQL (MySQL)** – Data querying, grouping, aggregation, and comparisons across roles, countries, and locations.
- **Python** – Exploratory data analysis, data cleaning, statistical summaries, and skill analysis.
- **Pandas** – Dataset loading, transformation, and tabular analysis.
- **NumPy** – Numerical operations and calculations.
- **Matplotlib** – Data visualization.
- **Power BI** – Interactive dashboards, KPIs, and comparative visualizations.
- **Jupyter Notebook** – Documentation of the Python analysis.
- **GitHub** – Version control and project presentation.

## Project Workflow

The project will follow a structured data analytics workflow:

1. **Understand the data:** Load the dataset and inspect its dimensions, column names, data types, sample records, and country distribution.
2. **Data quality assessment:** Identify missing values, duplicate postings, inconsistent formats, and potential data-quality issues.
3. **Data cleaning and preparation:** Handle missing values appropriately, standardize relevant fields, validate data types, and prepare the skills field for analysis.
4. **Exploratory data analysis:** Examine job counts, professional roles, locations, experience requirements, and advertised salary distributions.
5. **Skill demand analysis:** Identify frequently mentioned skills and compare skill requirements across selected job roles and countries.
6. **Comparative analysis:** Compare India and the USA using clearly defined metrics and account for differences in the number of postings and data completeness.
7. **Visualization and dashboard development:** Build charts and interactive Power BI reports to communicate important patterns.
8. **Interpretation and recommendations:** Summarize the findings, explain limitations, and suggest practical insights for job seekers.

## Planned Analysis

| Analysis Area              | Key Questions                                                                   |
| -------------------------- | ------------------------------------------------------------------------------- |
| Job market distribution    | How many postings are available for India and the USA?                          |
| Job roles                  | Which professional roles appear most frequently?                                |
| Skill demand               | Which skills are mentioned most often, overall and within analytics roles?      |
| Salary analysis            | How do available advertised salary values vary by role, country, and seniority? |
| Experience requirements    | What experience levels are requested for different roles?                       |
| Education requirements     | What education requirements are recorded in the available postings?             |
| Location analysis          | Which cities and regions have the most postings in this dataset?                |
| Work arrangements          | How are on-site, remote, and hybrid postings distributed?                       |
| Data Analyst opportunities | Which skills and qualifications appear in postings relevant to data analytics?  |

## Expected Business Value

The project aims to demonstrate how job posting data can be used to:

- Understand the skills employers request most frequently.
- Compare advertised job opportunities between India and the USA.
- Explore salary differences across selected professional roles.
- Understand experience and education requirements associated with different jobs.
- Identify job postings that mention remote and hybrid working arrangements.
- Support career planning and prioritization of relevant technical skills.
- Present job market information through accessible, interactive dashboards.

The analysis will provide descriptive insights into the available job postings. It will not establish actual hiring rates, guarantee salary outcomes, or prove that a particular skill causes higher earnings.

## Repository Structure

The repository will be organized as follows:

```text
Job-Market-Analysis-India-USA/
│
├── data/
│   └── job_postings_2026_sample.csv
│
├── notebooks/
│   └── Job_Market_Analysis.ipynb
│
├── sql/
│   └── job_market_analysis.sql
│
├── powerbi/
│   └── Job_Market_Dashboard.pbix
│
├── reports/
│   └── Project_Report.docx
│
└── README.md
```

- `data/job_postings_2026_sample.csv` – The dataset used for the project.
- `notebooks/Job_Market_Analysis.ipynb` – Python-based data inspection, cleaning, analysis, and visualizations.
- `sql/job_market_analysis.sql` – SQL queries used to investigate job market patterns.
- `powerbi/Job_Market_Dashboard.pbix` – Interactive dashboard containing key findings and comparisons.
- `reports/Project_Report.docx` – Final project report documenting the methodology, results, and recommendations.
- `README.md` – Project overview, dataset source, workflow, and findings.

## Scope and Limitations

- The dataset covers postings published from January through June 2026 and does not represent every job available in either country.
- The dataset contains more USA postings than India postings, so country comparisons must account for this imbalance.
- Salary information is missing from most records. Salary analysis will use only appropriate available records and report the sample size.
- Skills, experience, education, role, and work-mode information are missing from many records. Findings based on these fields may not represent all postings.
- Salary values are expressed in US dollars. Any comparison with local Indian salary levels must account for currency conversion, differences in cost of living, and the limitations of the dataset.
- Advertised salaries may not equal final compensation or actual salaries received by employees.
- Job postings do not necessarily correspond to unique vacancies, successful hires, or unique employers.
- The analysis is descriptive and cannot establish that particular skills or qualifications cause higher salaries or better employment outcomes.
- The dataset's documented collection and processing methods should be reviewed before interpreting derived or standardized fields.

## Project Status

**Phase 1 – Project Proposal and Initial Dataset Inspection**

The project title, business problem, objectives, dataset source, and planned analysis have been defined. The uploaded dataset has been inspected and confirmed to contain 100,009 rows and 17 columns, covering India and the USA.

The next phase will involve data quality assessment, cleaning, exploratory analysis, SQL querying, Python analysis, Power BI dashboard development, and documentation of evidence-based findings.

