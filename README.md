
# School District Analysis

## Overview of Project

Analyzing scores from a school district and comparing them based on school budget, size, and type.

### Purpose

Scores for 9th graders at Thomas High School (THS) appear to have been altered, remove the scores from the data set using the Pandas `loc` method through Jupyter Notebook, and determine how this changes the overall analysis of the school district.

## Results of Analysis

The following compares the outcome of the analysis with and without the scores of the 9th graders from Thomas High School.

### District Summary

* District Summary Changes
    - Total Students: No Change
    - Total Budget: No Change
    - Average Math Score: Dropped from 79.0 to 78.9
    - Average Reading Score: No Change
    - % Passing Math: Dropped by 0.2%
    - % Passing Reading: Dropped by 0.3%
    - % Overall Passing: Dropped by 0.1%

* With All Scores:

![District Summary](https://github.com/psidhu42/school-district-analysis/blob/main/resources/district_summary.PNG)

* Without 9th Grader Scores from THS:

![District Summary Without THS 9th Grader Scores](https://github.com/psidhu42/school-district-analysis/blob/main/resources/district_summary_altered.PNG)

### School Summary

The school summary only changed for Thomas High School as it was the only school that had the 9th grader scores removed.

* Thomas High School Summary Changes
    - Total Students: No Change
    - Total Budget: No Change
    - Per Student Budget: No Change
    - Average Math Score: Dropped from 83.41 to 83.35
    - Average Reading Score: Increased from 83.84 to 83.89
    - % Passing Math: Dropped by 0.1%
    - % Passing Reading: Dropped by 0.3%
    - % Overall Passing: Dropped by 0.3%

* With All Scores:

![School Summary](https://github.com/psidhu42/school-district-analysis/blob/main/resources/school_summary.PNG)

* Without 9th Grader Scores from THS:

![School Summary Without THS 9th Grader Scores](https://github.com/psidhu42/school-district-analysis/blob/main/resources/school_summary_altered.PNG)

### Scores by Grade

Looking at the DataFrame for Scores by Grade, you can see removing the 9th grader scores from THS only changed those cells to "nan" on both math and reading scores.

* Math Scores by Grade

![Math Scores by Grade](https://github.com/psidhu42/school-district-analysis/blob/main/resources/math_scores_by_grade.PNG)![Math Scores Without THS 9th Graders](https://github.com/psidhu42/school-district-analysis/blob/main/resources/math_scores_by_grade_altered.PNG)

* Reading Scores by Grade

![Reading Scores by Grade](https://github.com/psidhu42/school-district-analysis/blob/main/resources/reading_scores_by_grade.PNG)![Reading Scores Without THS 9th Graders](https://github.com/psidhu42/school-district-analysis/blob/main/resources/reading_scores_by_grade_altered.PNG)

### Scores by School Spending, Size, and Type

The scores by school spending, size, and type did not change at all, as shown in the following images of the DataFrames

* With All Scores:

![Scores by Spending](https://github.com/psidhu42/school-district-analysis/blob/main/resources/scores_by_spending.PNG)

* Without 9th Grader Scores from THS:

![Scores by Spending Without THS 9th Graders](https://github.com/psidhu42/school-district-analysis/blob/main/resources/scores_by_spending_altered.PNG)

## Summary