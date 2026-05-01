# Airline Safety Analysis

## Topic
This project investigates whether airline safety improved after the year 2000 compared to the period before 2000.

## Goal
The goal is to use statistical methods such as permutation testing and bootstrapping to evaluate whether airline safety has improved over time.

## Status
Completed. Analysis, visualization, permutation testing, and bootstrap uncertainty estimation have been finalized.


## Project Scaffold Table


| Element | Your Plan |
|--------|---------|
| **Topic / Question** | I am investigating whether airline safety improved after the year 2000 compared to the period before 2000. This matters because improvements in airline safety reflect advancements in technology, regulations, and operational practices that help reduce incidents and save lives. |
| **Hypothesis** | The mean number of airline incidents decreased after the year 2000 compared to before 2000. |
| **Outcome / Metric / Test Statistic** | The main test statistic is the difference in mean number of incidents between the periods 1985–1999 and 2000–2014. Additionally, I analyze the difference in median incidents for bootstrap uncertainty estimation. |
| **Units of Analysis** | Each observation represents one airline. |
| **Data Source(s)** | FiveThirtyEight Airline Safety dataset: https://raw.githubusercontent.com/fivethirtyeight/data/master/airline-safety/airline-safety.csv |
| **Why this data works** | This dataset contains airline incident and fatality counts across two clearly defined time periods, allowing a direct comparison of safety before and after 2000. The data is numeric, structured, and suitable for statistical analysis using permutation tests and bootstrap methods. |
| **Uncertainty Metric** | I use bootstrap resampling to estimate uncertainty in the median difference in incidents, since the Central Limit Theorem does not apply to medians. |
| **Null Hypothesis** | There is no difference in the mean number of airline incidents between the periods before and after 2000. |



## Final Analysis Summary

### What question did you ask?
I investigated whether airline safety improved after the year 2000 by comparing airline incident data before and after 2000.

### What data did you use?
I used the FiveThirtyEight airline safety dataset, where each row represents an airline. The dataset includes the number of incidents and fatalities for two time periods: 1985–1999 and 2000–2014.

### What patterns or relationships did you find?
The data shows that airline incidents decreased after 2000. The average number of incidents dropped from about 7.18 before 2000 to about 4.13 after 2000. Visualizations also show reduced variability and fewer extreme cases in the later period.

### How certain are you about those results?
Using a permutation test, I found a p-value of 0.0206 (2.06%), meaning we would observe a difference this large or larger only about 2.06% of the time due to random chance. This provides statistical evidence that the decrease in incidents is unlikely due to random chance.

However, a bootstrap confidence interval for the median difference ranged from approximately -1.0 to 4.0, which includes zero. This indicates some uncertainty when using the median.

This is because the Central Limit Theorem applies to means, but not directly to medians, especially with skewed data.

However, a bootstrap confidence interval for the median difference ranged from approximately -1.0 to 4.0, which includes zero. This indicates some uncertainty when using the median, although the overall trend still suggests improvement.

### What would you recommend or conclude?
Overall, the analysis suggests that airline safety improved after 2000. While the permutation test shows strong evidence of a decrease in incidents, the bootstrap analysis highlights some variability across airlines. This demonstrates the importance of using multiple statistical methods to fully understand real-world data.

