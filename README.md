# Uncovering Biases in California Mortgage Data

## Overview
This repository contains an in-depth analysis of California mortgage loan data from 2016, focusing on potential biases based on race, income level, and sex. Utilizing data from the Consumer Financial Protection Bureau and additional county-level Gini Index measures, the analysis explores the relationship between loan amounts and various demographic factors, aiming to uncover any existing disparities in mortgage lending practices.

## Contributors
Andrew Sun
Jonathan Cheng
Louis Scheinfeld 

## Repository Structure
data/: Contains the raw data files used in the analysis.
scripts/: Contains the R scripts used to process the data and generate the analysis.
output/: Contains the generated plots and summary tables from the analysis.
report/: Contains the final report in PDF format.

## Data Sources
Consumer Financial Protection Bureau (CFPB) Mortgage Data (2016):
Contains over 1 million observations with information on loan requests, applicant demographics, and loan details.
County-Level Gini Index Data:
Measures income inequality in each county, ranging from 0 (perfect equality) to 1 (complete inequality).

## Key Questions
What are the differences in mortgage loan amounts in California based on race, income level, and sex?
What relationship does this have with measures of inequality in a county?

## Analysis Summary
Loan Amount vs. Applicant Income: A positive correlation between applicant income and loan amount was observed.
Mean Loan Amount vs. Race: Asian applicants had the highest average loan amounts, followed by White applicants.
Income Amount vs. Race: Significant income disparities were found among different racial groups.
Loan Amount for White and Non-White Races: Non-White applicants tended to have higher median and upper quartile loan amounts compared to White applicants.
Gini Index and Loan Amount: A positive correlation between county Gini Index and mean loan amount was found, with higher minority percentages correlating with higher loan amounts in counties with greater income inequality.

## Conclusion
The analysis did not find strong evidence of bias in determining mortgage loan amounts based on race, sex, or income. While White and Asian applicants received higher loan amounts, this was correlated with higher income levels. The study highlights the complexity of mortgage lending and suggests further research with more representative data.

## Usage
To replicate the analysis, follow these steps:

1. Install required packages:
```
install.packages(c("dplyr", "ggplot2", "knitr", "stringr", "RSQLite", "grid", "mapdata", "maps"))
```
2. Clone the repository:
```
git clone https://github.com/yourusername/california-mortgage-loan-bias-analysis.git
cd california-mortgage-loan-bias-analysis
```
3. Run the R scripts:
```
source("scripts/analysis.R")
```

