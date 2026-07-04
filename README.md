# Data-Science-Assessment-2
This repository is a Data Science Assessment given by my academy for learning purpose.

# Week 2 Assessment - Data Analysis with Pandas

## Overview

This assessment demonstrates comprehensive data analysis skills using Python's Pandas library on an Indian startups funding dataset. The assessment covers theoretical concepts, practical code prediction, and real-world data manipulation and analysis.

## Assessment Structure

### Section A - Interview Theory (Questions 1-8)
Theoretical questions covering fundamental Pandas concepts:
- **Q1**: Difference between Series and DataFrame
- **Q2**: Understanding the `inplace` parameter
- **Q3**: Comparison of `fillna()` vs `dropna()` functions
- **Q4**: `pd.to_numeric()` with error handling
- **Q5**: Label-based vs integer-based indexing (`.loc` vs `.iloc`)
- **Q6**: Data transformation methods (`.map()`, `.apply()`, `.replace()`)
- **Q7**: Understanding and fixing `SettingWithCopyWarning`
- **Q8**: Binning techniques (`pd.cut()` vs `pd.qcut()`)

### Section B - Predict the Output (Questions 9-16)
Code prediction exercises testing understanding of:
- DataFrame reference behavior
- Handling missing values in statistical operations
- Type conversion and coercion
- Row selection and data types
- Warning scenarios in Pandas
- Lambda functions and mixed data types
- Unique value counting methods
- Boolean operations and operator precedence

### Section C - Applied Analysis on Indian Startups Dataset (Questions 17-40)

#### Loading & Inspection (Q17-Q19)
- Dataset shape and structure analysis
- Missing value identification
- Duplicate row detection
- Column naming conventions
- Statistical summary of founding years

#### Cleaning Verification (Q20-Q24)
- City name standardization
- Industry categorization
- Funding amount conversion and validation
- Date parsing and temporal analysis
- Funding stage distribution

#### Filtering (Q25-Q28)
- Conditional filtering based on location and funding
- Industry-based filtering
- Year-based filtering
- Pattern matching in startup names

#### Transformation & Derived Columns (Q29-Q32)
- Funding efficiency calculation
- Funding tier classification
- Era categorization based on founding year
- Investor count extraction

#### Aggregation & Grouping (Q33-Q37)
- Industry-wise funding analysis
- City-wise startup ecosystem analysis
- Cross-tabulation of industry and funding tiers
- Maximum funding identification by industry

#### Real Industry Problems (Q38-Q40)
- Emerging sector analysis (Fintech, Edtech, HealthTech)
- Regional funding hub identification
- City-industry startup concentration analysis

## Dataset Information

### Source
`indian_startups_fundingDADS.csv`

### Dataset Size
- **Rows**: 450 records
- **Columns**: 8 attributes

### Features
- **startup_name**: Name of the startup
- **city**: Location of the startup
- **industry**: Industry sector
- **funding_stage**: Stage of funding (Seed, Series A, etc.)
- **amount**: Funding amount in INR (Crores)
- **funding_date**: Date of funding round
- **investors**: Investor names/organizations
- **founded_year**: Year the startup was founded

### Data Cleaning Performed
1. Column name standardization to snake_case
2. City name normalization (e.g., Bangalore → Bengaluru)
3. Industry categorization standardization
4. Funding stage variant consolidation
5. Amount conversion to numeric (handling currency symbols, "Undisclosed" values)
6. Date parsing with multiple format support
7. Duplicate row removal

## Key Findings

### Dataset Statistics
- **Total Startups**: 450
- **Missing Funding Amounts**: 111 (24.7%)
- **Missing Funding Dates**: 358 (79.6%)
- **Missing Founded Years**: 23 (5.1%)
- **Average Funding**: ₹736.45 Crores
- **Funding Range**: ₹4 Crores to ₹3,549 Crores

### Temporal Insights
- **Busiest Year**: 2022 (23 deals)
- **Startup Founding Period**: 2008-2022
- **Average Founding Year**: 2016.4

### Geographic Distribution
- **Top Cities by Startup Count**: Noida (62), Kolkata (51), Bengaluru (49)
- **Top City by Total Funding**: Bengaluru (₹29,885 Crores)

### Industry Landscape
- **Top Industries**: SaaS (36), PropTech (32), AI/ML (22)
- **Highest Average Funding**: FinTech (₹3,545 Crores)
- **Emerging Sectors**: Electric Vehicles, HealthTech, Edtech

### Funding Patterns
- **Most Common Stage**: Bridge (41 deals)
- **Unicorn Candidates**: 75 startups (funding ≥ ₹1,000 Crores)
- **Funding Tiers**: Small/Unknown (118), Large (105), Mid (97)

## How to Use This Notebook

### Prerequisites
```bash
pip install pandas numpy
```

### Running the Analysis
1. Open `Week2_Assessment_G_Mohit.ipynb` in Jupyter Notebook or JupyterLab
2. Ensure the dataset file `indian_startups_fundingDADS.csv` is in the same directory
3. Execute cells sequentially from top to bottom
4. The notebook includes comprehensive comments explaining each operation

### Notebook Structure
- **Cell 0-8**: Section A - Theory answers
- **Cell 9-16**: Section B - Output predictions with code execution
- **Cell 18**: Data cleaning and preprocessing
- **Cell 20-24**: Loading and inspection
- **Cell 26-32**: Cleaning verification
- **Cell 33-37**: Filtering operations
- **Cell 38-42**: Data transformations
- **Cell 43-48**: Aggregation and grouping
- **Cell 49-52**: Real-world industry problems

## Technical Skills Demonstrated

- **Data Cleaning**: Handling missing values, type conversion, string manipulation
- **Data Transformation**: Creating derived columns, applying functions
- **Data Filtering**: Complex conditional queries, pattern matching
- **Data Aggregation**: GroupBy operations, statistical summaries
- **Temporal Analysis**: Date parsing, time-based filtering
- **Exploratory Analysis**: Cross-tabulation, value counting
- **Industry Best Practices**: Proper indexing, avoiding common warnings

## Author

**Name**: G Mohit  
**Assessment**: Week 2 - Data Analysis and Data Science  
**Date**: July 2026

## License

This assessment is submitted for academic evaluation purposes.

## Notes

- The dataset contains real-world messy data requiring extensive cleaning
- Multiple date formats and currency representations were handled
- Industry and city name variants were standardized for consistent analysis
- The analysis demonstrates both theoretical knowledge and practical application

