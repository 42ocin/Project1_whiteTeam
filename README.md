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
### Data processing
```python
heartdiseaseCSVPath = "Resources/heart_2020_cleaned.csv"
heartdiseaseDF = pd.read_csv(heartdiseaseCSVPath)
```

### Stats / Correlations

### Features

### Documentation
[(https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease)]
### Conclusion
Results from this, help create a clearer image of prevaling indicators of heart disease across a broad range of individuals. 
Using the different variables provided, define correlations have been found to that indicate the potencial of someone having cardiovascular illness at some point in their life. From this it can be easily seen what lifestyles and habits may contribute to heart health.
