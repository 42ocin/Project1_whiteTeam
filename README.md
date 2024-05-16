# Project1_whiteTeam
## Indicators of Heart Disease
Our team aims to find direct correlations and factors that may contribute to cardiovascular disease, ultimatley providing information that may contribute to estimating prevalence and improving early diagnosis of heart illness. We are using a dataset provided by the CDC and containing 18 different variables for the analysis.
### Intsallation

### Dependencies
numpy, matplotlib, pandas, scipy.stats and lineregress
```python
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
import scipy.stats as st
%matplotlib inLine
from scipy.stats import linregress
```
### Data Processing
```python
heartdiseaseCSVPath = "Resources/heart_2020_cleaned.csv"
heartdiseaseDF = pd.read_csv(heartdiseaseCSVPath)
```
```python
heartdiseaseDF.head()### Stats / Correlations
```

```python
yesheartDisease = heartdiseaseDF[(heartdiseaseDF["HeartDisease"] == "Yes")]
yesheartDisease### Features
noheartDisease = heartdiseaseDF[(heartdiseaseDF["HeartDisease"] == "No")]
noheartDisease
```
### Stats and Correlations
Statistical Avg
```python
combined_AvgDF = pd.concat([yesheartdiseaseAvgDF, noheartdiseaseAvgDF]).agg(['mean', 'median', 'var', 'std', 'sem'])
combined_AvgDF
```
Mean Values
```python
categories = ['BMI', 'Physical Health', 'Mental Health', 'Sleep Time']
mean_values_yes = [29.401592, 7.808242, 4.641764, 7.136156]
mean_values_no = [28.224658, 2.956416, 3.828778, 7.093416]
```
Age Group Comparison/Correlation
BMI Distrb/Corr
Sleep Corr
Mental Health Corr
Smoking vs Drinking Corr
Gender Comp/Corr
Race Comp/Corr
General Health Corr

### Features
## Bar Graph
![AgeCatHeartDiseaseVSNoBar](https://github.com/42ocin/Project1_whiteTeam/assets/164439696/97c60a1f-55fa-483e-acff-776797efb3fa)

## Scatter Plot
![AgeWHeartDiseaseScatter](https://github.com/42ocin/Project1_whiteTeam/assets/164439696/b16b641b-48d9-41aa-b5c6-4e676ac932e4)
## Pie Chart
![GenHealthPie](https://github.com/42ocin/Project1_whiteTeam/assets/164439696/ce6c7c37-d87e-4ef6-b8f2-32203ff2d6cf)

## Whisker Plot
![BMIwhisker](https://github.com/42ocin/Project1_whiteTeam/assets/164439696/3a817a95-ae6c-4124-8ea4-ec1330173f62)

## Donut Chart
![RaceDonuts](https://github.com/42ocin/Project1_whiteTeam/assets/164439696/e1b00025-a226-4343-b46d-c1be31881f60)

### Documentation
[(https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease)]
[(https://www.cdc.gov/brfss/annual_data/annual_2020.html)]
### Conclusion
Results from this, help create a clearer image of prevaling indicators of heart disease across a broad range of individuals. 
Using the different variables provided, define correlations have been found to indicate the potencial of someone having cardiovascular illness at some point in their life. From this it can be easily seen what lifestyles and habits may contribute to heart health.

