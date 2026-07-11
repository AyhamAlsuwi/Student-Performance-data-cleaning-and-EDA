# Student Performance - Exploratory Data Analysis (EDA)

This repository contains a Jupyter Notebook for exploratory data analysis (EDA) on the Student Performance dataset.

## Project Overview
The goal of this project is to analyze the factors that affect a student's final Performance Index, using data inspection, distribution checks, and correlation analysis.

## Key Steps & Implementation

### 1. Data Inspection
* Loaded the dataset from a raw GitHub URL.
* Checked dataset structure using `.info()`, `.describe()`, and `.isnull()`.
* Confirmed the dataset is clean with zero missing values and no incorrect input bounds (min/max values are correct).

### 2. Distribution & Structural Analysis
* Measured the skewness of the target variable (`Performance Index`) and found it has a balanced, normal distribution.
* Plotted histograms for all key numerical features (`Hours Studied`, `Previous Scores`, `Sleep Hours`, `Sample Question Papers Practiced`) to understand how data points are distributed.
* Generated a correlation matrix heatmap to find which variables share the strongest relationships with the performance target.

### 3. Exploratory Data Analysis (EDA) Insights
* **Hours Studied**: Showed a strong positive effect on the performance index with a clear linear trend. The minimum performance for students studying 9 hours is noticeably higher than the baseline.
* **Previous Scores**: Showed a nearly perfect linear positive trend with the performance index. Students with higher scores in the past consistently achieve the highest final performance.
* **Extracurricular Activities**: Did not show a significant or obvious effect on final performance scores.
* **Sleep Hours**: Getting more sleep helps up to a certain point, but more sleep hours alone does not guarantee performance improvement.
* **Sample Question Papers Practiced**: Practicing past papers gives a slight upward push to performance, but it does not completely guarantee a top-tier score on its own.

## Tech Stack
* **Language**: Python
* **Libraries**: Pandas, NumPy, Seaborn, Matplotlib
