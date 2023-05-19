# Statistics Data Modelling Project

## Authors
Kiersten Hamby, Breanna Ranglall, Krutika Tekwani

## Overview
This project investigates the factors influencing recruitment spending at post-secondary educational institutions in the United States. The aim is to build a multiple linear regression model to predict recruitment expenses using the data collected by the U.S. Department of Education Office of Post-secondary Education.

The variables selected for this model include Total Student Aid, Head Coach Salary for Men's Sports, Total Student Count, and Number of Head Coaches for Women's Sports. 

**Please note:**
While the model has proved to be statistically significant, it cannot be soundly used for inference purposes as the independence condition was violated due to relationships between universities in the data set.

## Dataset
The dataset includes data on athletic participation, athletic student aid, staffing, revenues, and expenses, segregated by men's, women's, and coed varsity teams. It is provided by the U.S. Department of Education Office of Post-secondary Education and includes more than 4000 variables. However, only a subset of these variables were selected for model creation.

## Project Setup
1. Clone this repository to your local machine.

2. Open your preferred R editor (e.g., RStudio).

3. Load the necessary libraries: tidyverse, skimr, Stat2Data, leaps, dplyr, and car.

4. Read the dataset from the CSV file "GroupE2-AthleticsSpendingData.csv" and filter for relevant variables.

5. Proceed with the data analysis as described in the project report.

## Structure
The script starts with data loading and initial exploration, followed by a first attempt to build a multiple linear regression model. After observing violations of model conditions (normality, equality of variance, and independence), data cleaning and transformation steps are performed.

The transformed dataset is then used for a more successful attempt to create the model, which is subsequently tested for multicollinearity. The script concludes with a coefficient interpretation and final remarks on the project outcomes and possible future steps.

## Running the Analysis
Make sure you have all the necessary libraries installed. After setting up, you can run the script in your R environment. 

```R
# Loading the necessary libraries
library(tidyverse)
library(skimr)
library(Stat2Data)
library(leaps)
library(dplyr)
library(car)

# Load your data
Athletics=read.csv("GroupE2-AthleticsSpendingData.csv")

# Proceed with the analysis as outlined in the script
```

## Output
The script includes numerous plots for data visualization and condition checking. It also generates multiple subsets for variable selection, as well as summary outputs for model testing. The final output is a statistically significant model explaining 79.72% of the variability in total recruiting expenses.

## Acknowledgments
This project was created as a part of the STAT 320 course at the University of St. Thomas. We want to acknowledge the U.S. Department of Education Office of Postsecondary Education for providing the data for this project.


