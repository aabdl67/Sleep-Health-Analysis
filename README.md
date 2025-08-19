# Sleep Health Analysis

## Project Overview

Comprehensive analysis of sleep health data examining relationships between sleep quality, stress levels, occupation, and BMI categories using R. This project follows a standard data analysis workflow with reproducible code and visualizations.

## Original Analysis Components

1.  **Data Inspection**: Initial checks for structure and missing values
2.  **Data Cleaning**: Blood pressure column transformation and data standardization
3.  **Exploratory Analysis**:
    -   Sleep duration by disorder status
    -   Stress vs sleep quality relationship
    -   Occupation-based sleep disorder prevalence
4.  **Statistical Testing**:
    -   BMI differences in sleep apnea (t-test)
    -   BMI category association (Fisher's exact test)
5.  **Predictive Modeling**:
    -   Insomnia risk based on stress and activity

## Visualizations

-   Rplot1_sleep duration by disorder status.png
-   Rplot2_stress vs. sleep quality.png
-   Rplot3_sleep disorders by occupation.png
-   Rplot4_sleep apnea vs. BMI category.png

## How to Use

1.  Ensure R and tidyverse are installed
2.  Update the data path in the script to your local location
3.  Run the script sequentially as written

## File Structure

```         
Sleep-Health-Analysis/
├── data/
│   └── Sleep_health_and_lifestyle_dataset.csv
├── scripts/
│   └── sleep_health_Data_Story.Rmd
├── figures/
│   ├── Rplot1_sleep_duration_by_disorder_status.png
│   ├── Rplot2_stress_vs_sleep_quality.png
│   ├── Rplot3_sleep_disorders_by_occupation.png
│   └── Rplot4_sleep_apnea_vs_BMI_category.png
├── README.md
├── .gitignore
└── Sleep-Health-Analysis.Rproj
```

## Data Source

[Sleep Health and Lifestyle Dataset](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset) from Kaggle.

## Author

Abubakar Abdallah
