# School_District_Analysis

## Overview
The purpose of this project was to assist Maria and the school board analyze academic grades for math and reading at 15 schools. The ninth grade scores at Thomas High School showed signs of academic dishonesty. As ar esult, the ninth grader's scores were removed from the data (using NaN values) and the analysis was recompleted.

## Results
In order to complete the analysis, the freshman at Thomas High School needed their grades replaced with 'NaN'. This was accomplished using the `loc` method as well as pandas `np.nan`. The code to replace the Thomas High School freshman's reading grades is 

`student_data_df.loc[(student_data_df["school_name"] == "Thomas High School") 
& (student_data_df["grade"] == "9th"),"reading_score"] = np.nan`


After merging the changes, the new dataframe looked [like this](Resources/Removal_THS_Freshman.png). Note the "NaN" values wherever the freshmen Thomas High School Students are.

### Math and Reading Scores
Overall, the changes in the overall analysis were near negligible. The scores at Thomas High School did not change more than half a percent. Thes results can be [seen here](Resources/Percent_Changes.png). This is due to the number of freshmen students at Thomas High School. There were 461 freshman at the high school.

### Scores by School Spending
There were no changes found when comparing the first and second analysis.
The results can be [found here](Resources/Scores_School_Spending.png).

### Scores by School Size
There were no changes found when comparing the first and second analysis.
The results can be [found here](Resources/Scores_School_Size.png).

### Scores by School Type
There were no changes found when comparing the first and second analysis.
The results can be [found here](Resources/Scores_School_Type.png).



## Summary

Five changes, although negligble, in the analysis:
* A decrease in average math score
* An increase in average reading score
* A decrease in passing math percentage
* A decrease in passing reading percentage
* A decrease in overall passing percentage

Overall, there was not a lot of change in the analysis. There were 39,170 students analyzed from 15 different schools. 461 freshman students from Thoms High School will not have a large impact on the high-level results.
