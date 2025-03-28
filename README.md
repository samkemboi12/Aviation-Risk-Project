# Aviation-Risk-Project
This is my Aviation risk Project description
Aviation Risk Analysis

Project Overview

This project aims to analyze aviation accident data to assess the risk associated with different aircraft. The goal is to provide actionable insights to help a company make informed decisions on purchasing low-risk aircraft for commercial and private aviation expansion.

Dataset
Source: Aviation accident dataset with 88,889 records and 31 attributes.
Attributes Include:
Aircraft specifications
Accident severity
Operational factors
Environmental conditions

Objectives
Identify aircraft models with the lowest accident risk.
Analyze key factors contributing to aviation accidents.
Assess accident severity trends based on operational and environmental conditions.
### Visualize the accident occurence caused by 'Broad.phase.of.flight'
![image](https://github.com/user-attachments/assets/ed3d5393-444e-44c4-ba26-9d61b6350fd2)
During Landing, Takeoff, Cruise, Maneuverings and Approach have a significantly higher number of recorded accidents.
### Analyze 'Make' and 'Total.Fatal.Injuries' to understand how make affected fatalities during accidents
![image](https://github.com/user-attachments/assets/bdddf623-941e-4e19-b0dd-0d3b505ac759)
Cessna, Boeing, Piper and Beech Aircraft Make Have Significantly More Fatalities
Commercial airliners Airbus and Mcdonnell Douglas generally have low fatality-per-accident.
### Grouping by Number.of.Engines and Model, summing Total.Fatal.Injuries
![image](https://github.com/user-attachments/assets/06ed4d6c-5eb0-4ff2-adf5-d2a5dda8edb1)
From the Graph, Boeing 737-222 model has one of the highest recorded fatal injuries
Some models have hundreds of fatalities, while others have only a few despite having one engine.
For Example Airbus 320 and R44 have significantly lower fatal injuries but also have one engine This means that Model of Aircraft play a big role in determining total fatalities.
Technologies Used
Python
Pandas
NumPy
Matplotlib & Seaborn
Jupyter Notebook

Project Structure
Project Notebook.ipynb: Jupyter Notebook with data analysis and visualizations.
AviationData.csv: Dataset containing aviation accident records.

README.md: Project documentation.
How to Run the Analysis
Install required libraries:
pip install pandas numpy matplotlib seaborn
Open Project Notebook.ipynb in Jupyter Notebook.
Run the notebook cells to load, clean, and analyze the data.

Load Data

import pandas as pd
# Read the AviationData using pandas
df = pd.read_csv("AviationData.csv", encoding="latin1")
# Display the last 5 rows of the data
df.tail()

Check Missing Values

# Check the null values and get the percentage
missing_percent = df.isnull().sum() / len(df) * 100
print(missing_percent.sort_values(ascending=False))

Basic Data Insights
Insights & Findings

Identifies high-risk and low-risk aircraft based on historical accident data.
Highlights key contributing factors such as weather, aircraft age, and operational procedures.
Provides recommendations for aircraft purchase based on risk assessment.
Future Improvements
Incorporate machine learning models for predictive risk analysis.
Enhance data visualization with interactive dashboards.
Include real-time aviation data for dynamic risk assessment

This is My Tableau Dashboard Link:
https://public.tableau.com/views/ProjectDashboard_17431499279480/AircraftRisksAnalysis?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link
