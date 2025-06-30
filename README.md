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
- Build a scatterplot and fit a line of best fit, between the relationship of alchohol content and wine quality, and repeated for pH and also residual sugar content.
- Calculated the correlation between Quality and alchohol content, pH and residual sugar content.

### Machine Learning (Supervised Segmentation Algorithm)

- Partitioned the data into 80% training and 20% testing
- Used rpart to fit a decision tree onto the data
- Ensured that the tree would not be too complex, by limiting the maximum depth/nodes
- Plot the tree and examined the output using a confusion matrix

### Final Analysis

- Used the model to determine most important variables, relating back to plots and considering information gain.

## Conclusion and discussion of findings:

It was found that alchohol content was the most important variable to consider when assessing the quality of red wine. Interestingly, it was also found that the most negligible factor was residual sugar content. This claim is boasted by the machine learning model and the fact that alchohol content is the very first split in the tree, showing that it presents the most information gain and reduces the most amount of enthalpy. Additionally, a clear relationship exists between alchohol content and quality of the wine as seen from our plots. High alchohol content does not necesarilly mean that the bottle of wine will always be good, but it is certainly a statistically significant indicator.
