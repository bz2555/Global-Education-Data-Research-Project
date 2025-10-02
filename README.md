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
# 7. Citation
Zhang, Bella. (2025). Global Education Data Research Project [Course Project]. Teachers College, Columbia University. DOI: pending.
# 8. Additional Details
## Which metadata standard did you choose and why?
For this project, I chose the Data Documentation Initiative (DDI) as the metadata standard. DDI is widely recognized in the social sciences and education research fields, and it provides a systematic framework for documenting datasets, including variables, methodologies, and data collection processes. Since my dataset covers multiple indicators of global education (such as enrollment, out-of-school rates, and literacy), DDI was particularly useful for ensuring that each variable was clearly defined and consistently described. Using DDI not only improves the clarity of the dataset but also increases its potential reusability for future research in education equity and learning analytics.
## Which template/software did you use?
I used R Markdown to create the README file, as it allows me to combine structured text with formatted tables and visuals in a single document. R Markdown also supports export to PDF, which is required for this assignment. For preliminary drafting and easier editing, I experimented with Stackedit, a Markdown editor with real-time preview, which helped me visualize the final structure quickly. In addition, I followed the structure of sample templates available on GitHub.
## What was the most challenging part of creating a ReadME file? How did you overcome these obstacles?
The most challenging part was creating a comprehensive data dictionary that adhered to DDI standards. My dataset contains 29 variables, many of which are technical education indicators such as out-of-school rates or gross enrollment ratios. At first, it was difficult to decide how detailed the definitions should be, especially when variables had overlapping concepts. To overcome this, I carefully studied the definitions provided in the Excel data dictionary sheet, and then restructured them into a DDI-compliant format with clear categories: variable name, description, type, units, and notes.
Another challenge was balancing clarity and readability. DDI requires thorough detail, but a README file also needs to be accessible and engaging. To solve this, I added headings, tables, and concise explanations, and I used Markdown formatting to keep the content user-friendly.
