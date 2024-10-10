# README for Tree Circumference Analysis

## Overview
This repository contains scripts for analyzing tree circumference data from two sites (control and treatment) over a period of 20 years. The analysis includes calculations of mean, standard deviation, growth rates, and statistical comparisons using t-tests.

## Scripts

### 1. `RNA_seq_analysis.R`
**Purpose:**  
Analyzes RNA-seq count data to extract gene expression statistics.

**Inputs:**  
- **File:** `gene_of_interest_expression.tsv`  
  Contains RNA-seq count data for various genes across three samples.

**Outputs:**  
- **Tables:**  
  - First six genes with their count values.
  - Mean expression values for the first six genes.
  - List of the top 10 genes with the highest mean expression.
  - Count of genes with a mean expression less than 10.
- **Histogram:**  
  A plot showing the distribution of mean expression values.

### 2. `tree_growth_analysis.R`
**Purpose:**  
Analyzes tree circumference measurements from two sites to calculate growth and perform statistical comparisons.

**Inputs:**  
- **File:** `growth_data.csv`  
  Contains tree circumference measurements for control and treatment sites from the years 2005, 2010, 2015, and 2020.

**Outputs:**  
- **Summary Statistics:**  
  - Mean and standard deviation of tree circumference for the years 2005 and 2020 at both sites.
- **Boxplot:**  
  A boxplot comparing tree circumference at the start (2005) and end (2020) for both sites.
- **Growth Calculation:**  
  Mean growth over the last 10 years for both control and treatment sites.
- **Statistical Test:**  
  A t-test comparing the growth rates between the two sites, with the resulting p-value.

## Installation and Usage
1. Ensure you have R and required packages installed. 
2. Clone this repository to your local machine.
3. Open the R scripts in RStudio or any R environment.
4. Run the scripts sequentially to analyze the data as described.

## Requirements
- R (version 4.0 or higher recommended)
- Required packages: `ggplot2`, `dplyr` (if applicable)

## Contribution
This project was completed by [Your Name] and [Group Member's Names if applicable]. Each member contributed to the coding and analysis process.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
