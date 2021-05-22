# School_District_Analysis

## Overview 
The purpose of this analysis is to analyze data from multiple schools in order to gain insight into trends based on school performance on standardized tests relative to school type, size, and funding. An original analysis was conducted, although it was found that one high school's 9th grade scores were affected by academic dishonesty. In this project, I will refactor the code to eliminate these grades and determine how the original analysis was affected.   

## Results
The analysis was conducted in a python jupyter notebook and can be found here: [Analysis Script](https://github.com/fadlnabbouh/School_District_Analysis/blob/main/PyCitySchools_Challenge.ipynb). 

- The district summary was affected in the Average Scores columns and % Passing Columns. With the elimination of 9th grade data, the scores and % passing variables for Thomas High School changed, decreasing a small amount. This caused the overall values in the district summary to decrease as well. 
	- District summary old: ![Screenshot](https://github.com/fadlnabbouh/School_District_Analysis/blob/main/Resources/district_summary_old.png)
	- District summary new: ![Screenshot](https://github.com/fadlnabbouh/School_District_Analysis/blob/main/Resources/district_summary_new.png)

- Similarly, the elimination of 9th grade scores affected the school summary by decreasing the scores and % passing columns. In this case, however, only the Thomas High School values were changed, while the rest of the table remained unchanged. 
	- School summary old: ![Screenshot](https://github.com/fadlnabbouh/School_District_Analysis/blob/main/Resources/school_summary_old.png)
	- School summary new: ![Screenshot](https://github.com/fadlnabbouh/School_District_Analysis/blob/main/Resources/school_summary_new.png)

- Although changing the 9th grade scores for Thomas High School caused a drop in their overall scores and % passing, this change was insignificant relative to other schools. Thomas High School remains the second best school in overall passing percentage. 

- Replacing the 9th grade scores may also affect the following: 
	- scores by grade - the only change that occurred was that the value under 9th grade for Thomas High School was replaced with "NaN". All other values in both dataframes were unchanged. 
	- scores by spending - because the change in scores, passing percentages for reading and math, as well as overall passing percentage for Thomas High School, did not change significantly, the values for spending by school were also unchanged. To one significant digit, there is no change at all between the old and new dataframes.
	- scores by size - as with spending, no significant change occurred with the scores by size dataframe. 
	- scores by type - as above, no significant change occurred with the scores by type dataframe. 

## Summary

The district summary changed by reducing the values of the scores and percent passing variables (for both reading and math, as well as overall). In addition, the scores for Thomas High School in the school summary were reduced, although not by a significant amount. When comparing math and reading scores by grade, the 9th grade value for Thomas High School is replaced with "NaN", although the rest of the data remains unchanged. Finally, scores by school spending, school size, and school type were reduced because of the elimination of Thomas High School's 9th grade score, although this change was so insignificant that the summary dataframes were unchanged. 