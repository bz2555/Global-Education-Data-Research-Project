# Global-Education-Data-Research-Project
HUDK 4054 Individual Assignment 2
# 1. General Information
Title: Globle education data research project  
Creator: Bella Zhang
ORCID ID: https://orcid.org/0009-0003-6205-9059  
Affiliation: Teachers College, Columbia University  
Research Date: 09/27/2025  
# 2. Project Abstract
This project investigates **global education disparities** using a dataset of 200+ countries and regions, which includes 29 variables covering indicators such as school enrollment, out-of-school rates disaggregated by gender, literacy rates, and transition rates across different educational stages. The dataset allows us to explore how **educational access and attainment vary globally**, with a particular focus on **gender differences** and **regional inequalities**. For example, the dataset captures the percentage of boys and girls who are out of school at pre-primary, primary, and lower secondary levels, as well as adult and youth literacy levels, providing a rich foundation for analyzing education systems across diverse contexts.
# 3. Dataset & File Overview and Features
## Data Format
The dataset is stored as an Excel file (.xlsx) with two sheets:  
- GlobalEducationData: Contains the raw numerical indicators for each country/region.
- Data Dictionary: Provides definitions and descriptions for all 29 variables, ensuring consistent interpretation.
## Global Education Data
To explore worldwide educational access and equity, this project uses a dataset that covers over 200 countries and regions. The dataset includes 29 variables representing indicators of school enrollment, out-of-school rates, literacy rates, and educational transitions. These measures are disaggregated by education stage (pre-primary, primary, lower secondary, upper secondary) and, where applicable, by gender (male/female).
- Geographic Information: Latitude and longitude coordinates to enable regional or spatial comparisons.
- Education Access Indicators: Out-of-school rates for children and adolescents at different educational stages.
- Enrollment and Completion Rates: Gross enrollment ratios and transition rates between education levels.
- Literacy Indicators: Youth and adult literacy rates that reflect longer-term educational outcomes.
- Equity Measures: Gender parity indices and gender-disaggregated statistics to evaluate differences between boys and girls.
## File Name
Global Education Data_Week 4.xlsx
# 4. Data Labels
| Variable Name | Discription | Data Type | Units / Values |Notes |
|----------|----------|----------|----------|----------|
| Country    | Name of the country or area     | String     | Text     | Primary identifier     |
| Latitude    | Latitude coordinate of the country’s centroid    | Numeric (Float)     | Degrees (−90 to +90)     | Geographic indicator     |
| Longitude    | Longitude coordinate of the country’s centroid     | Numeric (Float)     | Degrees (−180 to +180)     | Geographic indicator     |
| OOS_PrePrimary_Male    | Out-of-school rate for pre-primary age males     | Numeric (Percentage)     | 0–100 (%)     | Indicates % of boys not enrolled     |
| OOS_PrePrimary_Female    | Out-of-school rate for pre-primary age females     | Numeric (Percentage)     | 0–100 (%)     | Indicates % of girls not enrolled     |
# 5. Python Library
In order to properly run the models, the following Python libraries are used:
```python
import numpy as np
import pandas as pd
import sklearn as sk
import keras
from keras import utils as np_utils
```
# 6. Methodological Information
## Variable Definition and Construction
- **Out-of-school rates**: Calculated as the percentage of children or adolescents in a specific age group who are not enrolled in the corresponding level of education. Values are disaggregated by gender (male/female).
- **Enrollment ratios**: Gross enrollment ratios (GER) are computed as the number of students enrolled in a specific education level, regardless of age, expressed as a percentage of the official school-age population.
- **Transition rates**: Represent the percentage of students who successfully move from one level of education (e.g., primary) to the next (e.g., lower secondary).
- **Literacy rates**: Youth (ages 15–24) and adult (15+) literacy rates measure the percentage of individuals who can read and write a simple statement about everyday life.
- **Gender parity index (GPI)**: The ratio of female-to-male values for enrollment or literacy. A value of 1 indicates parity, values below 1 favor males, and values above 1 favor females.
## Software and Tools
The dataset is analyzed using Python (pandas, matplotlib, seaborn) for data cleaning, statistical analysis, and visualization. Documentation and metadata are structured using the DDI (Data Documentation Initiative) standard to ensure reproducibility and clarity.
