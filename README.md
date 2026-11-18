# Asteroid Analysis

Exploratory data analysis of an asteroid dataset with around 958,000 asteroids, done in Python on Kaggle.

## What I did

* Cleaned the data: removed exact duplicates, dropped columns I did not need (prefix and equinox), fixed data types and removed values that are not possible
* Filled missing values where another column could be used: moid from moid_ld, PHA labels using the PHA rule, and H with the median of each class
* Left diameter and albedo empty because about 86% of them are missing
* Looked at asteroid classes, NEOs, PHAs, diameter and how diameter relates to absolute magnitude (H)

## Main findings

* Most asteroids are in the Main Belt (855,954 MBA)
* Only 22,895 are NEOs (about 2.4%) and 2,067 are PHAs
* Diameter is known for 136,209 asteroids and most of them are a few km across. The largest is Ceres at 939.4 km
* Outer objects like TNOs are much bigger than the near Earth classes
* Diameter and H have a strong negative relationship that is clearest on a log scale

## Data

The dataset is too big for GitHub (around 450 MB), so it is not included here. You can download it from [Kaggle](https://www.kaggle.com/datasets/manishamali/asteroid-dataset-analysis).

## Tools

Python, Pandas, NumPy, Matplotlib and Seaborn

## How to run

Open the notebook on Kaggle with the asteroid dataset attached and run all cells. The cleaned data gets saved as asteroid_cleaned.csv.
