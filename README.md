
# School District Analysis

## Overview of Project

Analyzing scores from a school district and comparing them based on school budget, size, and type.

### Purpose

Scores for 9th graders at Thomas High School (THS) appear to have been altered, remove the scores from the data set using the Pandas 'loc' method through Jupyter Notebook, and determine how this changes the overall analysis of the school district.

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

### Scores by Grade and by School Spending, Size, and Type

Looking at the DataFrame for Scores by Grade, yiu can see removing the 9th grader scores from THS only changed those cell to "nan".

![Math Scores by Grade](https://github.com/psidhu42/school-district-analysis/blob/main/resources/math_scores_by_grade.PNG)![Math Scores Without THS 9th Graders](https://github.com/psidhu42/school-district-analysis/blob/main/resources/math_scores_by_grade_altered.PNG)

## Election-Audit Summary

This script can be reused to determine outcomes of other elections if using a `.csv` file that has the results in it. One step needed would be to change the path at `file_to_load = ` by providing the correct directory and file name for the new file. Another modification needed might be referencing the correct index if the data is in a different order in the new `.csv` file. 

The data in the `.csv` file used in this analysis is as follows (Ballot ID,County,Candidate) with the index being (0,1,2). The new file for example could be (Ballot ID,Candidate,County) then at the following location in the code, the index would need to be changed for candidate_name and county_name next to `row[]`.
```
# For each row in the CSV file.
    for row in reader:

        # Add to the total vote count
        total_votes += 1

        # Get the candidate name from each row.
        candidate_name = row[2]

        # 3: Extract the county name from each row.
        county_name = row[1]
```
