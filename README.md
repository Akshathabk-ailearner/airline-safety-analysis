# Airline Safety Analysis

## Topic
This project investigates whether airline safety improved after the year 2000 compared to the period before 2000.

## Goal
The goal is to use statistical methods such as permutation testing and bootstrapping to evaluate whether airline safety has improved over time.

## Status
Project setup in progress.


## Project Scaffold Table

### Topic / Question  
I am investigating whether airline safety improved after the year 2000 compared to the period before 2000. This matters because improvements in airline safety reflect advancements in technology, regulations, and operational practices that help reduce incidents and save lives.

### Hypothesis  
The mean number of airline incidents decreased after the year 2000 compared to before 2000.

### Outcome / Metric / Test Statistic  
The main test statistic will be the difference in mean number of incidents between the periods 1985–1999 and 2000–2014.
Additionally, I will analyze the difference in median incidents for bootstrap uncertainty estimation.

### Units of Analysis  
Each observation represents one airline. 

### Data Source(s)  
FiveThirtyEight Airline Safety dataset:
https://raw.githubusercontent.com/fivethirtyeight/data/master/airline-safety/airline-safety.csv 

### Why this data works  
This dataset contains airline incident and fatality counts across two clearly defined time periods, allowing a direct comparison of safety before and after 2000. The data is numeric, structured, and suitable for statistical analysis using permutation tests and bootstrap methods.  

### Uncertainty Metric  
I will use bootstrap resampling to estimate uncertainty in the median difference in incidents, since the Central Limit Theorem does not apply to medians.This difference will be evaluated using a permutation test.

### Null Hypothesis  
There is no difference in the mean number of airline incidents between the periods before and after 2000.
