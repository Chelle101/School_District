# School_District Analysis
Module 4
## Overview
The school board has notified Maria and her supervisor that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to Maria for help.

The analysis conducted compares previous school district analysis against this firm's analysis in order to determine how the suspected academic dishonesty affects school performance.

The school board has requested the following deliverables:

- A high-level snapshot of the district's key metrics, presented in a table format
- An overview of the key metrics for each school, presented in a table format
- Tables presenting each of the following metrics:
- Top 5 and bottom 5 performing schools, based on the overall passing rate
- The average math score received by students in each grade level at each school
- The average reading score received by students in each grade level at each school
- School performance based on the budget per student
- School performance based on the school size
- School performance based on the type of school

## Objective
Maria has asked you to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once you’ve replaced the math and reading scores, Maria would like you to repeat the school district analysis that you did in this module and write up a report to describe how these changes affected the overall analysis.

In this comparative analysis between counting and not counting Thomas High School Ninth Grade scores to see average and scores at:
 - School Level
 - District Level
 - School Type

## Results/ Analysis
### How is the district summary affected?
The average math score decreased by 0.1 points while the average reading score stayed the same. The percentage of students passing math decreased by 1% as did the percentage of students passing reading. The overall passing percentage also decreased by 1%.

- Average Math Scores: moved from 79 to 78.9 as a result of taking out Thomas High School Ninth Grade scores.
- Average Reading Scores did not change.
- Percent Passing Math moved from 75% to 74%.
- Percent Passing Reading moved from 86% to 85%.
- Percent Overall Passing moved from 65% to 64%.

![Screenshot 2022-04-16 190137](https://user-images.githubusercontent.com/99842026/163693812-e545df97-c5c0-412c-99a2-2a579d5bde3c.png)

### How is the school summary affected?
The only change in data is with Thomas High School. The overall math and reading passing numbers decreased.
Math and reading scores for ninth graders at Thomas High School were replaced with 'NaN' (Not a Number) so that their scores would not affect future calculations. If all of the students' scores were replaced with a 'O', then this would negatively impact averages for the school and school district.

- Average Math at Thomas decreased from 83.42 to 83.35.
- Average Reading at Thomas slightly increased from 83.84 to 83.89.
- Average Percent Passing Math at Thomas greatly decreased from 93.3% to 66.9%.
- Percent Passing Reading at Thomas decreases from 97.3% to 69.7%.
- Average Percent Overall passing both Math and Reading decreased from 90.9% to 65.1%

![Screenshot 2022-04-16 190758](https://user-images.githubusercontent.com/99842026/163693900-a8efb0b4-5aea-468b-b78f-3234d94d23d7.png)

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Thomas High is no longer in the top 10 after adjusting 9th grades scores with NaNs.
Thomas High School moved from 2nd place overall with a passing % of 92% down to last place with a passing % of 68%.

### How does removing the ninth grade scores affect the following?

- Math and Reading Scores by Grade
Thomas High School's 9th grade class has no math or reading score data to count. Everything else was unaffected.
- Scores by School Spending
District spending per school was calculated by determining average spending ($620), standard deviation (~30), minimum spending amount ($578), lower quartile ($592), mid quartile ($628), upper quartile ($642), and mximum spending amount ($655) across all 15 schools:.
- Scores by School Size
The Medium (1000-2000) bin saw a decrease in the passing percentages since Thomas High School was in that school size.

![Screenshot 2022-04-16 191815](https://user-images.githubusercontent.com/99842026/163694049-2881832f-6722-4be2-88d4-c46757466143.png)

- Scores by School Type
The Charter schools saw a decrease in the passing percentages since Thomas High School was in that school type. Though, interestingly the average math and reading scores for that range remained the same.

![Screenshot 2022-04-16 192115](https://user-images.githubusercontent.com/99842026/163694103-3a30171c-5583-40f8-9f02-5801f553686a.png)


### Summary

#### Removing 9th grade student scores from Thomas High School affected the school district in the following ways:

- Average math scores dropped slightly (<1%)
- Average reading scores were not affected
- Percentage of students passing math dropped slightly (-1%)
- Percentage of students passing reading dropped slightle (-1%)
- The overall passing rate dropped (-1%)

### Only scores for Thomas High School were affected:

- Perentage of students passing math dropped from 93.2% to 66.9%
- Percentage of students passing reading dropped from 97.3% to 69.7%
- Overall passing percentage dropped from 90.9% to 65.1%

### Thomas High School affected school rankings in the following ways:

- Thomas High school dropped out of the top 5 high schools in the district
- Wright High School moved into the top 5 high schools in the district
- Bottom 5 high schools was unaffected

### 9th grade student scores from Thomas High School affected other reports:

- Math and reading scores by grade remained the same for all other schools
- Thomas High School had no data to report for 9th grade math and reading scores

** Scores by school spending chaged at the $601-650 range:
- Percentage passing math dropped from 73% to 67%
- Percentage passing reading dropped from 84% to 77%
- Overall passing percentage dropped from 63% to 56%

** Scores by school size changed for medium-sized schools (1000-2000):
- Percentage passing math dropped from 94% to 85%
- Percentage passing reading dropped from 97% to 91%
- Overall passing percentage dropped from 91% to 85%

** Scores by schools type were affected in the following ways:
- Percentage passing math dropped from 94% to 90%
- Percentage passing reading dropped from 97% to 93%
- Overall passing percentage dropped from 90% to 87%

## Resources
- Data Sources: students_complete.csv/school_complete.csv files
- Client Requirements from School Board
- Software: Python 3.7.7, Anaconda, Jupyter Lab, Git 2.27
- Output Files: PyCitySchools.ipynb & PyCitySchools_Challenge.ipynb (with NaN)

## Develpoment Environment
- Jupyter Notebook
- Python v3.7.x
- Dependencies
- Python Pandas library
- Python Numpy library
