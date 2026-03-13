# Part 1 - A Grain of Truth: What Actually Drives Rice Yields?

**By: Brya Patterson** *University of Washington, MS Information Management (MSIM)* *Spring 2024*


## Project Overview

This project investigates the primary drivers of agricultural productivity within Indonesian rice farms. Utilizing a dataset of 1,026 observations from West Java (1975–1978), this analysis explores the relationships between land size, rice varieties, and chemical inputs (Urea and Phosphate) to determine how farmers can optimize their gross output.

This repository contains **Part 1** of an ongoing series. While this stage focuses on historical statistical drivers, **Part 2** will integrate longitudinal climate data to predict yields under modern environmental conditions.

## Key Insights

* **Scale is King:** Statistical testing (ANOVA) confirmed that farm size is the most dominant predictor of yield across all rice varieties ($p < 0.001$).
* **Variety Performance:** High-Yield Varieties (HYV) consistently outperformed traditional and mixed varieties in gross output per hectare.
* **Fertilizer Efficiency:** Regression modeling indicates that **Urea** provides a significantly higher return on yield compared to Phosphate, suggesting a clear path for input optimization.

## Technical Stack

* **Language:** R
* **Libraries:** `tidyverse`, `dplyr` (Data Wrangling), `plm` (Econometric Dataset Access), `ggplot2`, `gridExtra` (Visualization)
* **Environment:** RStudio / R Markdown
* **Methods:** * Descriptive Statistical Analysis
* Analysis of Variance (ANOVA)
* K-Means Clustering (Regional Segmentation)
* Multiple Linear Regression (Predictive Modeling)



## Repository Structure

```text
├── Data/               # Documentation for the plm RiceFarms dataset
├── Scripts/            # R Markdown and exported R scripts
├── Visualizations/     # Charts showing Fertilizer vs. Yield relationships
└── README.md           # Project summary and documentation

```

## Methodology

1. **Exploratory Data Analysis (EDA):** Identified central tendencies and distributions of gross output across various Indonesian regions.
2. **Variance Testing:** Applied ANOVA to determine if differences in output were statistically significant based on the rice variety planted.
3. **Regional Clustering:** Used K-Means clustering to group farms by geographic output patterns, identifying high-performing hubs regardless of variety.
4. **Predictive Modeling:** Built multiple linear regression models to quantify the impact of Urea and Phosphate on total harvest weight.

## Future Work: Part 2

The next phase of this project, **"Seasons of Change,"** will move beyond farm-level inputs to incorporate environmental variables.

* **Climate Integration:** Joining 1970s farm data with historical rainfall and temperature records from West Java.
* **Forecasting:** Predicting how 1970s yields would be impacted by 2024–2026 climate profiles.
* **Gap Analysis:** Investigating the "Technology-Climate Gap" in modern Indonesian agriculture.

## References

* **Data Source:** Feng Q, Horrace WC (2012). "Alternative technical efficiency measures: Skew, bias and scale." *Journal of Applied Econometrics*.
* **Original Study:** Erwidodo (1990). "Panel Data Analysis on Farm-Level Efficiency, Input Demand and Output Supply of Rice Farming in West Java, Indonesia." *Michigan State University Dissertation*.

---

*For a full technical report and executive summary of this project, please visit https://https://bryap.github.io/datasci_ricefarms_pt1.html*