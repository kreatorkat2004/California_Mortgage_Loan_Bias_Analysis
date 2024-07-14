# Uncovering Biases in California Mortgage Data

## Overview
This repository contains an in-depth analysis of California mortgage loan data from 2016, focusing on potential biases based on race, income level, and sex. Utilizing data from the Consumer Financial Protection Bureau and additional county-level Gini Index measures, the analysis explores the relationship between loan amounts and various demographic factors, aiming to uncover any existing disparities in mortgage lending practices.

## Data Sources
- **Consumer Financial Protection Bureau (CFPB) Mortgage Data (2016):** Contains over 1 million observations with information on loan requests, applicant demographics, and loan details.
- **County-Level Gini Index Data:** Measures income inequality in each county, ranging from 0 (perfect equality) to 1 (complete inequality).

## Key Questions
1. What are the differences in mortgage loan amounts in California based on race, income level, and sex?
2. What relationship does this have with measures of inequality in a county?

## Analysis Summary
- **Loan Amount vs. Applicant Income:** A positive correlation between applicant income and loan amount was observed.
- **Mean Loan Amount vs. Race:** Asian applicants had the highest average loan amounts, followed by White applicants.
- **Income Amount vs. Race:** Significant income disparities were found among different racial groups.
- **Loan Amount for White and Non-White Races:** Non-White applicants tended to have higher median and upper quartile loan amounts compared to White applicants.
- **Gini Index and Loan Amount:** A positive correlation between county Gini Index and mean loan amount was found, with higher minority percentages correlating with higher loan amounts in counties with greater income inequality.

## Conclusion
The analysis did not find strong evidence of bias in determining mortgage loan amounts based on race, sex, or income. While White and Asian applicants received higher loan amounts, this was correlated with higher income levels. The study highlights the complexity of mortgage lending and suggests further research with more representative data.

## Usage
To replicate the analysis, follow these steps:

### Dependencies
Install the required R packages:

```R
install.packages(c("dplyr", "ggplot2", "knitr", "stringr", "RSQLite", "grid", "mapdata", "maps"))
```

### Installing
Clone the repository to your local machine and navigate to the project directory:

```bash
git clone https://github.com/yourusername/california-mortgage-loan-bias-analysis.git
cd california-mortgage-loan-bias-analysis
```

### Executing program
Run the R scripts to perform the analysis:

```R
source("scripts/analysis.R")
```

## Authors
Contributors' names and contact info:

- Andrew Sun
- Jonathan Cheng
- Louis Scheinfeld

## Version History
- 0.1
  - Initial Release

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.

## Acknowledgments
- Consumer Financial Protection Bureau for the mortgage data.
- Researchers and analysts who have contributed to the field of mortgage lending studies.
- Open-source community for the R packages used in this analysis.
