# School_District_Analysis
## Project Overview

Given a large data set with information about a specific school district, we analyzed that data to see what trends and insights we can glean into school performance. Did one type of school perform better than another? How did school size or school budget effect scores? Which schools performed the best or the worst in math, reading, or overall? These are all questions we answered through our research and analysis. Additionally, after performing our analysis with the full data set, we were informed that there had been questions regarding the academic integrity of a certain grade from a certain school. This required us to wipe that grades results from our data, and then to re run our analysis with the new data set. Our results and how this change affected our analysis will be detailed below.

## Resources

Data Source: schools_complete.csv, students_complete.csv

Software used: Python 3.8.8, Anaconda 4.10.3, Jupyter Notebook, Virtual Studio Code Version: 1.57.0

## Results
First, we replaced the scores for all 9th graders from Thomas High School with NaN values, to remove them from our analysis without affecting the other school's scores. Once we removed the 9th grade scores from our dataframe, we ran the same district analysis that we had run previously and by comparing the two dataframes, found some interesting results. The two data frames are displayed below with per school analysis. The Thomas High School line shows the differences that are described below. First image is the original data frame, the second image is our analysis without Thomas High 9th graders.
<img src = Resources/Per_School_Analysis_Original.png>
<img src = Resources/Per_School_Analysis_new.png>


### Overall District Analysis
* The average math score dropped from 79.0 to 78.9, while the percentage of students who passed math dropped from 75% to 74.8%.
* The average reading score remained at  81.9, but interestingly the percentaeg of students who passed reading dropped from 85.81% to 85.66%.
* The overall percentage of students who passed both math and reading dropped from 65.17% to 64.86%
### Thomas High School Analysis
We only looked at the 10th, 11th, and 12th graders from Thomas High school for the following analysis.
* The percentage of students who passed math dropped from 93.3% down to 93.2%.
* The percentage of students who passed reading dropped from 97.3% down to 97.1%.
* The overall percentage of students who passed both math and reading dropped from 90.9% to 90.6%.
### School Ranking Analysis
Re running our analysis without the scores from Thomas High School 9th graders, Thomas High actually retained its overall position of 2nd out of 15 schools in terms of overall passing percentage.
<img src = Resources/Top_Performing_Schools_new.png>

### Scores by grade, size, type, and budget
* Removing the 9th grade scores from Thomas High did not affect the other schools performance. Nor did this affect the other grades at Thomas High.
* By splitting the data into bins by school type, school size, and school budget, there was no appreciable change in the data. 
<img src = Resources/Scores_School_Size.png>
<img src = Resources/Scores_School_Type.png>
<img src = Resources/Scores_School_Budget.png>

## Summary
While our analysis did not change a lot when looking at the overall results of by school size, type and budget, this could be attributed to the fact that we were only removing 461 scores out of 39,170 total students and scores. However we did see that there were changes in the overall passing percentage of Thomas High students, as well as a decrease in scores from those same students. The specific changes can be seen in the above analysis, but removing the scores in question did cause Average Math, Average Reading, Passing Math %, Passing Reading %, and Overall Passing % to all decline among Thomas High students and among the entire data set as a whole. 