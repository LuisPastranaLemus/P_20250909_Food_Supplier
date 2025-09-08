# 🧭 Project Analysis

This project analyzes user behavior for a food-tech startup’s application. The first part explores the sales funnel, identifying how users progress through each stage, where they drop off, and how many ultimately reach the purchase stage. The second part focuses on an A/A/B test designed to evaluate a potential font change in the app. By comparing two control groups (with the old fonts) and one test group (with the new fonts), the analysis determines whether the design update impacts user behavior and ensures reliability by validating the similarity between control groups.

---

## 🔍 Project Overview (P-20250909_Food_Supplier)

Project Overview

Key questions:

1. Sales Funnel Analysis

    - How do users progress through the sales funnel?
    - How many users actually reach the purchase stage?
    - At which stages do users get stuck or drop off?
    - Which specific stages show the highest user drop-off rates?

2. A/A/B Test Evaluation

    - Do users respond differently to the new font design compared to the old one?
    - Are the two control groups (A1 and A2) statistically similar, ensuring test reliability?
    - Which font style (old vs. new) produces better user engagement or conversions?
    - What insights can be drawn from comparing control groups for future experiment design?

Project Info explanation

__Note__: 

- Same dataset for both parts → The sales funnel analysis and the A/A/B test are based on the same dataset. This reinforces data consistency.
- Dual control groups (A/A/B) → Having two control groups (A1 & A2) is crucial. It ensures reliability, since significant differences between them could reveal external factors biasing the experiment.
- Experimentation mindset → In real-world scenarios, experiments like this are continuous. The project mimics how analysts repeatedly test and validate app quality with different datasets and designs.
- Decision-making focus → The ultimate goal is guiding product decisions (whether to adopt the new font design) using statistical evidence, not intuition.
- Quality of data → Validating that both control groups are similar provides insight into how much time and data are needed to run reliable tests in the future.

---

## 🧮 Data Dictionary

This project has N different tables.

- `logs_exp_us.csv` (user event information)
    `EventName`: Name of the event.
    `DeviceIDHash`: unique user identifier.
    `EventTimestamp`: event time.
    `ExpId`: Experiment number. 246 and 247 are the control groups, and 248 is the test group.
  
---

## 📚 Guided Foundations (Historical Context)

The notebook `00-guided-analysis_foundations.ipynb` reflects an early stage of my data analysis learning journey, guided by TripleTen. It includes data cleaning, basic EDA, and early feature exploration, serving as a foundational block before implementing the improved structure and methodology found in the main analysis.

---

## 📂 Project Structure

```bash
├── data/
│   ├── raw/              # Original dataset(s) in CSV format
│   ├── interim/          # Intermediate cleaned versions
│   └── processed/        # Final, ready-to-analyze dataset
│
├── notebooks/
│   ├── 00-guided-analysis_foundations.ipynb     ← Initial guided project (TripleTen)
│   ├── 01_cleaning.ipynb                        ← Custom cleaning 
│   ├── 02_feature_engineering.ipynb             ← Custom feature engineering
│   ├── 03_eda_and_insights.ipynb                ← Exploratory Data Analysis & visual storytelling
│   └── 04-sda_hypotheses.ipynb                  ← Business insights and hypothesis testing
│
├── src/
│   ├── init.py              # Initialization for reusable functions
│   ├── data_cleaning.py     # Data cleaning and preprocessing functions
│   ├── data_loader.py       # Loader for raw datasets
│   ├── eda.py               # Exploratory data analysis functions
│   ├── features.py          # Creation and transformation functions for new variables to support modeling and EDA
│   └── utils.py             # General utility functions for reusable helpers
│
├── outputs/
│   └── figures/          # Generated plots and visuals
│
├── requirements/
│   └── requirements.txt      # Required Python packages
│
├── .gitignore            # Files and folders to be ignored by Git
└── README.md             # This file
```
---

🛠️ Tools & Libraries

- Python 3.11
- os, pathlib, sys, pandas, NumPy, Matplotlib, seaborn, IPython.display, scipy.stats
- Jupyter Notebook
- Git & GitHub for version control
-

---

## 📌 Notes

This project is part of a personal learning portfolio focused on developing strong skills in data analysis, statistical thinking, and communication of insights. Constructive feedback is welcome.

---

## 👤 Author   
##### Luis Sergio Pastrana Lemus   
##### Engineer pivoting into Data Science | Passionate about insights, structure, and solving real-world problems with data.   
##### [GitHub Profile](https://github.com/LuisPastranaLemus)   
##### 📍 Querétaro, México     
##### 📧 Contact: luis.pastrana.lemus@engineer.com   
---

