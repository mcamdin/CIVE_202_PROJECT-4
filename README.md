# CIVE 202 Project 4 – Risk Analysis Using National Risk Index

## Files Included
- `PROJECT_#4New.ipynb` - Code with comments (for TA)
- `PROJECT_#4.ipynb` – Code/Main analysis notebook (Run each section of code in order)
- `Project 4 - ACD_McGuigan_Htoo_Rezaie` - Annotated Code Document (Purpose of each line of code)
- `Project 4 - Engineering Timesheet_McGuigan_Htoo_Rezaie` - Engineering Timesheet (Track hours & wage)
- `Project 4 - Gantt Chart_McGuigan_Htoo_Rezaie` - Gantt Chart (Keep track of progress)
- `Project 4 - Report_McGuigan_Htoo_Rezaie` - Written Report (Discussions & Results)
- `Project 4 - SOW_McGuigan_Htoo_Rezaie` - Scope of Work (Reproducible methods)
- `Project4_Combined_Cleaned_Data.csv` – Cleaned dataset file used in analysis
- `Montana.csv` - Raw dataset file used in analysis
- `Wyoming.csv` - Raw dataset file used in analysis
- `NRI_Table_CensusTracts_Montana.csv` - Raw dataset file used in analysis
- `NRI_Table_CensusTracts_Wyoming(in).csv` - Raw dataset file used in analysis
- `NRIDataDictionary(in).csv` - Raw dataset file used in analysis
- `NRIDataDictionary.csv` - Raw dataset file used in analysis
## Authors
Camdin McGuigan, Nay Law Htoo, and Ahmad Rezaie 

CIVE 202 – Spring 2026

## Overview
This project analyzes natural disaster risk using the FEMA National Risk Index (NRI) dataset for Wyoming and Montana. The goal was to understand how risk is calculated using the NRI and then create a custom risk scoring method to compare against the original values. This helps show how different definitions of risk can change results and highlight possible bias.

## Data Sources
- FEMA National Risk Index (NRI) Census Tract Data  
- CDC Social Vulnerability Index (SVI) Data  

## Methodology
- Downloaded and cleaned NRI and SVI data for Wyoming and Montana  
- Created a matching TRACTFIPS field to join datasets  
- Merged datasets together for analysis  
- Handled missing values in key variables  
- Developed a custom risk score using:
  - Expected Annual Loss (EAL)
  - Social Vulnerability (SOVI)
  - Community Resilience (RESL)

### Custom Risk Formula
Custom Risk Score =  
0.50 × EAL + 0.35 × SOVI + 0.15 × (100 − RESL)

## Results
- Created choropleth maps for:
  - NRI Risk Score (Wyoming and Montana)
  - Custom Risk Score (Wyoming and Montana)
- Compared spatial differences between NRI and custom results  
- Created a bar graph comparing wildfire risk between states  

## Discussion
The custom risk scores showed differences compared to the NRI values due to changes in how variables were weighted. The custom method placed more emphasis on economic loss and social vulnerability, which caused some areas to appear higher risk compared to the original NRI results. This shows that risk outcomes can vary depending on how the data is interpreted and weighted.

## Implications
Risk scores are used to guide funding and disaster planning decisions. Differences between methods can impact which communities are considered high risk and may affect how resources are distributed. This highlights the importance of understanding how risk is calculated and ensuring transparency in the process.

