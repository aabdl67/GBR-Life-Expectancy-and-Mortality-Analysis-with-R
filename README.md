
# GBR Life Expectancy and Mortality Analysis

## Project Overview

Comprehensive analysis of Great Britain mortality data (1950-1984) examining life expectancy trends, mortality patterns, and demographic shifts using R. This project investigates the epidemiological transition that occurred during this transformative period in British public health history, following a standard data analysis workflow with reproducible code and visualizations.


## Analysis Components

1. **Data Inspection**: Initial checks for structure, summary statistics, and missing values  
2. **Data Cleaning**: Year column transformation, variable standardization, and column name cleaning
3. **Exploratory Data Analysis**:  
   - Life expectancy trends by sex (1950-1984)
   - Mortality patterns across age groups and time periods
   - Infant vs. elderly mortality comparisons and ratio analysis
   - Population structure changes through pyramid comparison
   - Survival probability from birth to age 65
4. **Statistical Testing**:  
   - Life expectancy improvement significance (t-test: 1950s vs. 1980s)
5. **Visual Analytics**: Eight comprehensive visualizations illustrating key trends namely:

- `Rplot1_Life_Expectancy_at_Birth.png`  
- `Rplot2_Mortality_Trends_by_Age_Group.png`  
- `Rplot3_Mortality_Rate_Heatmap_by_Age_&_Year.png`  
- `Rplot4_Population_Pyramid.png`  
- `Rplot5_Survival_Probability_from_Birth_to_Age_65.png`  
- `Rplot6_Infant_Mortality_Rate_in_First_Year.png`  
- `Rplot7_Infant_vs_Elderly_Mortality_Trends.png`  
- `Rplot8_Ratio_of_Infant_to_Elderly_Mortality_Rates.png`

## How to Use

1. Ensure R and tidyverse are installed  
2. Update the data path in the script to your local location  
3. Run the script sequentially as written to reproduce the analysis
4. Find generated visualizations in `Output/Figures/` folder
5. Review comprehensive findings in `Output/Key_Findings.md`

---

## File Structure

```
GBR-Life-Expectancy-and-Mortality-Analysis/
│
├── GBR.csv                                        # Raw source data
├── GBR Life Expectancy and Mortality Analysis.Rmd # Main data analysis script (R Markdown)
├── GBR-mortality-analysis-with-R.Rproj           # RStudio project configuration
├── README.md                                      # Project overview and documentation
├── .gitignore                                     # Git exclusion rules
│
└── Output/                                        # Generated analysis outputs
    ├── Figures/                                   # Folder containing all visualizations
    │   ├── Rplot1_Life_Expectancy_at_Birth.png
    │   ├── Rplot2_Mortality_Trends_by_Age_Group.png
    │   ├── Rplot3_Mortality_Rate_Heatmap_by_Age_&_Year.png
    │   ├── Rplot4_Population_Pyramid.png
    │   ├── Rplot5_Survival_Probability_from_Birth_to_Age_65.png
    │   ├── Rplot6_Infant_Mortality_Rate_in_First_Year.png
    │   ├── Rplot7_Infant_vs_Elderly_Mortality_Trends.png
    │   └── Rplot8_Ratio_of_Infant_to_Elderly_Mortality_Rates.png
    │
    └── Key_Findings.md                            # Summary of analysis results and conclusions
```

---

## Data Source

**Great Britain Mortality Data (1950-1984)**  
Source: Human Mortality Database (HMD)  
Link: [www.mortality.org](https://www.mortality.org)
Specific dataset: Period life tables for Great Britain


*Note: The dataset contains period life tables for Great Britain with detailed mortality parameters by age and sex.*

## Key Variables Analyzed

- `Year1`, `Year2`: Period years combined to create midpoint analysis year
- `Sex`: Biological sex (1 = Male, 2 = Female)  
- `Age`: Age in years (0 to 110+)
- `AgeInt`: Age interval for each life table entry
- `m(x)`: Central death rate at age x (number of deaths divided by person-years lived)
- `q(x)`: Probability of death between exact age x and x+1
- `l(x)`: Number of survivors to exact age x from original cohort of 100,000
- `d(x)`: Number of deaths between exact age x and x+1
- `L(x)`: Person-years lived between exact age x and x+1
- `T(x)`: Total person-years lived above exact age x
- `e(x)`: Life expectancy at exact age x (average number of years remaining to live)

## Required R Packages

- tidyverse (dplyr, ggplot2, tidyr, readr)


## License & Attribution

**Project Context & Data Attribution**

This analysis was conducted to demonstrate competency in data processing, statistical analysis, and visualization using real-world demographic data. It explores foundational concepts in epidemiology and public health, specifically the epidemiological transition in a high-income country.

The dataset (`GBR.csv`) is sourced from the **Human Mortality Database** (www.mortality.org). As a standard practice in academic and professional work, any use of this analysis or its findings must include proper citation of this original source.

*Code and visualizations are my own.*

## Author
Abubakar Abdallah

##
*Last updated: `August 27, 2025`*




















