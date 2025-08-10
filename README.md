# Project Risk Analysis

This repository contains a **synthetic dataset** and an accompanying Jupyter notebook for analyzing project risk. The goal is to demonstrate data‐driven decision making that would be relevant to roles such as Business Analyst, Program Manager and Data Analyst.

## Project Overview

Modern organizations run numerous projects with varying budgets, team sizes and priorities. Understanding how these factors relate to project risk helps leaders allocate resources, set realistic expectations and mitigate potential issues.

The synthetic dataset in this repository simulates 1,000 projects across multiple business domains and includes variables such as manager experience, team size, budget, duration, domain and priority. Each project is assigned a **risk score** and categorized as _On Schedule_, _At Risk_ or _Delayed_.

In the accompanying Jupyter notebook, we perform exploratory data analysis (EDA) with visualizations and build predictive models to estimate risk and classify project status. The analysis progresses from simple descriptive statistics to baseline linear regression and more sophisticated models like random forest regression/classification.

## Contents

- `synthetic_project_data.csv` – the synthetic dataset used in this project.
- `project_risk_analysis.ipynb` – a Jupyter notebook that loads the dataset, explores the data, visualizes key relationships and builds predictive models.
- `requirements.txt` – a list of Python dependencies needed to run the notebook.

## Dataset Description

| Column | Description |
| --- | --- |
| `Project_ID` | Unique identifier for each project |
| `Manager_Experience` | Years of experience of the project manager |
| `Team_Size` | Number of people on the project team |
| `Budget_kUSD` | Budget allocated to the project (in thousands of USD) |
| `Duration_days` | Planned duration of the project in days |
| `Domain` | Business domain (IT, Finance, Marketing, Operations or HR) |
| `Priority` | Project priority (High, Medium or Low) |
| `Risk_Score` | Calculated risk score between 0 and 100 |
| `Status` | Project status classification derived from the risk score (On Schedule, At Risk, Delayed) |

The synthetic data were generated programmatically with plausible relationships: higher budgets, longer durations and larger teams tend to increase risk; greater manager experience and higher priority reduce risk. Random noise ensures variability.

## Getting Started

1. **Clone or download this repository** to your local machine.
2. **Install the required dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

3. **Open the Jupyter notebook** `project_risk_analysis.ipynb` in Jupyter Lab, Jupyter Notebook or VS Code and run the cells in order. The notebook will load the dataset, perform exploratory analysis and build predictive models.

4. **Experiment further**: adjust hyperparameters, try different algorithms, add new features or visualize other relationships to deepen your understanding.

## Potential Extensions

- **Feature engineering**: derive new variables such as budget per team member or experience per team member.
- **Time series analysis**: add temporal dimensions to simulate changes over time.
- **Domain‐specific analyses**: explore patterns within each business domain or priority level.
- **Visualization dashboards**: create interactive dashboards using tools like Plotly or Tableau to communicate insights.

## License

This project is released under the MIT License. See the [LICENSE](LICENSE) file for details.

---

This project was generated as a demonstration for portfolio building. You can customize the dataset generation logic and analysis to suit your interests and showcase your analytical skills.
