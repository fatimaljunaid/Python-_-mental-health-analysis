# Student Mental Health Analysis

A data analysis project exploring factors affecting students' mental health 
using Python, pandas, and visualization libraries.

---

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Key Findings](#key-findings)
- [Visualizations](#visualizations)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies](#technologies)
- [Author](#author)

---

## Overview

This project analyzes a dataset of 100 students with 26 variables related 
to mental health, academic performance, lifestyle, and social factors.

Goals:
- Clean and preprocess raw data
- Engineer new features (Mental Health Score, Risk Level)
- Identify key factors affecting student mental health
- Visualize insights through professional charts

---

## Dataset

Source: `data/raw/mental_health_evaluation_data.csv`

Size: 100 rows x 26 columns

Key Variables:

| Category | Variables |
|----------|-----------|
| Mental Health | Anxiety, Depression, Stress levels |
| Academic | Performance, Engagement, Stress |
| Lifestyle | Sleep Quality, Physical Activity, Nutrition |
| Social | Family Support, Peer Support, Teacher Relationship |
| Behaviors | Social Media, Substance Use, Mood Fluctuations |

Engineered Features:
- `Mental_Health_Score` (0-30): sum of Anxiety + Depression + Stress
- `Wellness_Index` (0-10): average of Sleep + Self-esteem + Emotional Stability
- `Social_Support_Score` (0-4): Family Support + Peer Support
- `Risk_Level`: Low / Medium / High

---

## Project Structure

```
mental-health-analysis/
├── data/
│   ├── raw/                    # Original dataset
│   └── processed/              # Cleaned dataset
├── outputs/
│   └── charts/                 # Generated visualizations
├── main.py                     # Main analysis script
└── README.md
```

---

## Key Findings

### 1. High Risk Prevalence
- 45% of students are in High Risk category
- 46% are in Medium Risk
- Only 9% are in Low Risk

### 2. Strongest Risk Factors (Positive Correlation)
| Factor | Correlation |
|--------|:---:|
| Substance Use | +0.31 |
| Nutrition Quality | +0.17 |

### 3. Strongest Protective Factors (Negative Correlation)
| Factor | Correlation |
|--------|:---:|
| Motivation Level | -0.27 |
| Teacher Relationship | -0.21 |
| Sleep Quality | -0.19 |
| Work-Life Balance | -0.15 |

### 4. Teacher Relationship Impact
| Relationship | Mental Health Score | High Risk % |
|--------------|:---:|:---:|
| Negative | 17.06 | 53% |
| Neutral | 15.23 | 44% |
| Positive | 14.33 | 37% |

Conclusion: Positive teacher relationships reduce High Risk probability 
from 53% to 37%.

### 5. Surprising Finding
Social Media Addiction showed no correlation with mental health issues 
in this dataset, contradicting common belief. This suggests either:
- Confounding variables exist
- Social media may serve as a coping mechanism, not a cause

---

## Visualizations

### Distribution of Mental Health Indicators
![Distributions](outputs/charts/chart1_distributions.png)

### Correlation Heatmap
![Correlation](outputs/charts/chart2_correlation_heatmap.png)

### Key Factors by Risk Level
![Risk Factors](outputs/charts/chart3_factors_by_risk.png)

### Teacher Relationship Impact
![Teacher Impact](outputs/charts/chart4_teacher_impact.png)

---

## Installation

```bash
git clone https://github.com/YOUR_USERNAME/mental-health-analysis.git
cd mental-health-analysis
pip install pandas numpy matplotlib seaborn
```

---

## Usage

```bash
python main.py
```

---

## Technologies

- Python 3.10+
- pandas
- numpy
- matplotlib
- seaborn

---

## Author

[Fatima Al Junaid]
GitHub: [@fatimaljunaid](https://github.com/fatimaljunaid)