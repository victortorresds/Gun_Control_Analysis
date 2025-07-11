# 📉 Gun Control Analysis

**Author:** Victor Torres  
**Date:** October 2, 2024  
**Tool:** R & RMarkdown  

---

## Objective

This project explores whether **stricter firearm control laws** are associated with **lower firearm mortality rates** in the United States using public health data and gun law scores.

---

## Data Sources

-  **CDC Firearm Mortality Rates**  
  🔗 [CDC Mortality Data](https://www.cdc.gov/nchs/pressroom/sosmap/firearm_mortality/firearm.htm)  
  🔗 [CDC Open API](https://open.cdc.gov/apis.html)

-  **Gun Law Grades**  
  Data scraped from the Law Center to Prevent Gun Violence Scorecard.

---

## Methodology

1.  Load and filter 2023 CDC firearm mortality data.
2. Clean and convert gun law grades into a 5-point Likert scale:
   - `1 = Most Lax` 🔴
   - `5 = Most Strict` 🟢
3.  Merge datasets by state.
4. Create **heatmaps** and **scatterplots** to explore relationships.
5. Perform visual trend analysis with linear regression.

---


---

## 📸 Visualizations

> To see the full analysis and interactive graphs, view the RMarkdown or HTML report.

### Firearm Mortality Rate by State

![Firearm Mortality Heatmap] (https://github.com/victortorresds/Gun_Control_Analysis/blob/main/images/gun_control.png)

### Gun Death Rate vs. Law Strictness (Linear Regression)

![Gun Law vs Mortality Scatter] https://github.com/victortorresds/Gun_Control_Analysis/blob/main/images/gun_control_1.png"?raw=true

---

## Conclusion

**Yes, stricter firearm control laws are associated with lower firearm mortality.**  
States like **California**, **Connecticut**, and **New Jersey** (with strong laws) have lower gun death rates than states like **Alabama**, **Arizona**, and **Georgia** (with weaker laws).

---

## R Libraries Used

```r
library(tidyverse)
library(jsonlite)
library(plotly)
library(rvest)


