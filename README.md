# School_District_Analysis

## Challenge Analysis

### Objective: 
There is an issue with the testing scores for 9th graders at Thomas High School. The objective is to remove all of these scores and re-run the analysis for the school district. We will determine what effect replacing these values with NaN has on downstream analyses. 

The original analysis can be found [here.](PyCitySchools.ipynb)
The updated analysis with Thomas High School 9th grade scores changed to NaN can be found [here.](PyCitySchools_Challenge.ipynb)


#### How is the the district summary affected?
The district summary is affected with only minor changes. The average math scores decreased by 0.1 while the average reading scores did not change. The percent of students passing at the distrcit level decreased by 1% for the % passing math, % passing reading, and % overall passing (passing both).

#### How is the school summary affected?
As the issue was only with Thomas High School, other schools in the district were unaffected. However, Thomas High School saw a number of changes. While there averages for both math and reading were still ~83, their passing rate saw a sharp decline. In the original analysis their passing rates were all of 90% but they all fell to 65-69%. This is because none of the 9th graders from Thomas High School would achieve a passing grade. The lack of major affect on average test score is because NaN is ignored when calculating the average (it is treated as blank rather than as 0).

#### How is Thomas High School's performance relative to other schools affected?
Thomas High School was previously the 2nd best performing school by overall passing rate. After removing the 9th grade scores from Thomas HS, they fell to the 8th position by overall passing rate.

#### How does replacing the ninth grade scores affect the following?
- Math and reading scores by grade: The only aspect of this analysis that is changed is the cell with data for the 9th graders of Thomas High School. Before removal they had a 83.6 average at math and a 83.7 average for reading. After removal, the values in these cells are now NaN.
- Scores by school spending: Thomas High School spending per student fell into the $630-644 range so only data from this range changed. While the average math and reading score did not change, the % passing math decreased from 73 to 67, the % passing reading decreased from 84 to 77 and the percent overall passing decreased from 63 to 54. 
- Scores by school size: Thomas High School is a medium sized school so only data from this category changed. While the average math and reading score did not change, the % passing math decreased from 94 to 88, the % passing reading decreased from 97 to 91 and the percent overall passing decreased from 91 to 85.
- Scores by school type: Thomas High School is a charter school so only data from this category changed. While the average math and reading score did not change, the % passing math decreased from 94 to 90, the % passing reading decreased from 97 to 93 and the percent overall passing decreased from 90 to 87.
