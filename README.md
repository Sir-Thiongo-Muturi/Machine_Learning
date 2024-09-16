# Project Background
I have a dataset of 499 ski resorts distributed around the globe alongside a number of distinctive characteristics associated with them. 
Goal: come up with a windows application that predicts the most suitable resort for a skier based on their preferences. 
## Model:
Input: user preferences such as desired slope difficulty, amenities, and budget.
Output: recommended resort.
Model: content-based filtering
# Brief Overview of this project-
The exercise involves making use of an SQL script within a python code to import the necessary data from MYSQL database into Jupyter notebook. 
## Data preprocessing 
```
from sklearn.preprocessing import StandardScaler
from sklearn.decomposition import PCA
import pandas as pd

# Assuming you have loaded the data into df_read_sql
# Select relevant numerical columns for PCA
numeric_columns = ['Price', 'Highest point', 'Lowest point', 'Beginner slopes', 
                   'Intermediate slopes', 'Difficult slopes', 'Total slopes', 
                   'Longest run', 'Snow cannons', 'Surface lifts', 'Chair lifts', 
                   'Gondola lifts', 'Total lifts', 'Lift capacity']

resorts_numeric = df_read_sql[numeric_columns]

```
Our objective is to conduct a PCA, and as such, we will be using variables that are numerical.

