# School_District_Analysis
Data cleaning and School District testing analysis.

## Summary
The purpose of the project is to evaluate data for the school board. Evidence shows that certain classes may have cheated, and our goal with the project is to alter and evaluate data while keeping non-cheating parties' data intact.

### Background
The data in "schools_complete.csv", "students_complete.csv" found in the "Resources" folder, was given to us to perform our analysis on. 

#### Resources

Data input files:
- schools_complete.csv 
- students_complete.csv

The technology used here were the following:

Python 3.7.6
Jupyter Notebooks

## Results
During our analysis, we discovered the following trends in our data:

- <strong>District Summary</strong>: When it came to the district as a whole, the following were the results:
![image of District Analysis](Images/district_summary.png)
As you can see, the math scores are in a worse position than the average reading scores. In the district, improving math scores would be more beneficial to having more students pass overall. 

- <strong>School Summary</strong>: The results of the district analysis, when broken down by school, were the following:
![image of District Analysis](Images/district_summary_by_school.png)
Based on the results, we can tell that Cabrera High is the leader in testing scores, with an overall passing rate of 91.3%, and a 97.0% reading passing rate, and a 94.1% math passing rate. In this dataset, we can see an interesting outlier - Thomas High School. Upon further investigation, we determined that the ninth grader's dataset must be removed, and the results after removal brought overall scores to fit the rest of the district. 

### The Effects of Replacing Ninth-Grade Scores
Based on the district data, Thomas High School has some obvious deficiency in their passing scores. Upon further investigation, their low scores are due to the 9th graders' data. 

Once we removed the 9th graders from Thomas from our sample, the following happened:
![image of District Analysis](Images/district_summary_by_school_after_edits.png)
Here, you can clearly see that the Thomas grades were improved overall, which was indicative of the data being cleaned. 

For spending, there was a substantial increase in the "medium-low" (585-615) bracket. Here was the initial, pre-cleaned data:
![image of Spending Before](Images/spending_before.png)
After the ninth graders were removed, the numbers increase substantially:
![image of Spending After](Images/spending_after.png)


### Challenges Encountered
During the series of analysis, we had a difficult issue:
- Organization of code: Between the initial analysis and the "repeat" analysis, the code presented did not feel easy to read. There were many steps, and getting lost in the steps frequently made it hard to stay accurate in the reporting.

## Conclusions
After changing the data to drop Thomas High's ninth graders, we can note the following changes:
1. Scores by spending increased for the medium-low spending bucket ($585-615), which was where Thomas High School fell under. For spending by school budget per student, overall passing rates 
2. When Thomas High School's 9th grade classs was dropped, scores across the board increased. However, when comparing scores by school size, not much was changed in the "Medium" size bucket, which was where Thomas High School fell under. This may be due to the fact that the 9th grade class did not have much of an impact on the overall sample, or that it was not properly factored into the analysis. 
3. For spending ranges, the average math scores increased greatly in the medium-low (585-615) bracket once 9th graders from Thomas were removed, increasing math scores from 87 to 94% passing.
4. When broken down by type, the Charter schools' scores increased by a hair. Overall, not much changed before and after the analysis, which may be due to the small impact that Thomas High School's 9th grade class played in this bracket.
