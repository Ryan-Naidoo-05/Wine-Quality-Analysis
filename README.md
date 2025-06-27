# EDA and Supervised Segmentation Analysis of Red Wine
A solution to the classification problem: "What makes wine good?"

## Dataset
Download [here](https://www.openml.org/search?type=data&sort=runs&id=40691&status=active)

 ## Tools & Technologies Used
- **R** (v4.3.1)  
- **RStudio** (IDE)  
- **R Markdown** (for analysis & reporting)  
- **CRAN Packages**:
  - `tidyverse` (ggplot2, dplyr, tidyr) – Data manipulation & visualization  
  - `corrplot` – Correlation matrices  
  - `rmarkdown` – Dynamic report generation  

## Project Process

### Preprocessing
- Loaded relevant libraries and dataset "winequality-red.csv"
- Edited the table to add the "is_good" column, which ensures a relevant target variable.
- Ensured that this mutated column was in a "factor" format for categorical usage.

### Exploratory Descriptive Analysis

- Built a bar graph the visualise the number of records for each quality category.
