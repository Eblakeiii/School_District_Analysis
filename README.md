# School_District_Analysis

# Overview
The purpose of this analysis was to analyze the adjusted district data.  The data adjustment was replacing the reading and math scores, from Thomas High School 9th graders, with  NaN (herein to be referred to as the Thomas Freshmen).  The results of this analysis was to compare the adjusted outcome to the original analysis to determine the impact, if any. 

The district wide analysis encompased:
*  15 high schools, either considered district or charter
*  Combined total student population was 39,170
*  Total combined annual budget of $24,649,428
*  Student population of the Thomas High School was 1,635 
*  Thomas Freshmen was 461, or 28.12% of the Thomas High School population

# Results
## Thomas Freshman affect on the District
- The impact the replaced scores of the Thomas Freshmen was minimal to none on a district wide level.  Fixed variables such as number of schools, budgets and total number of students remain the same.  The changes in the scoring outcomes were close to being flat.  The only real change was a one percent decrease in % Passing Math (from 75% to 74%), % Passing Reading (from 86% to 85%) and % Overall Passing (from 65% to 64%).  

## How is the school summary affected (avg math, avg read, % math, % read, % overall
original (83.418349	83.848930	93.272171	97.308869	90.948012)  adjusted (83.350937	83.896082	66.911315	69.663609	65.076453
As in the district wide study, the items using fixed variables remain unchaged.  The averages for both the math and reading was almost negligible, even though the Thomas Freshmen represent over a quarter of the population.  The passing percentages, on the other hand, had material changes. See table below for the breakdown for math, reading and overall passing rates. 

    ORIGINAL passing rates for:            ADJUSTED passing rates for:
    math    reading   overall              math    reading   overall  
    -----   -----     --------             -----   -----     --------
    93.3%,	97.3%     90.9%,               66.9%	  69.7%	    65.1%

The differences between in all the passing rates are all over 25%.  Is this because the NaN sees the 461 scores as complete fails?

## Hows does replacing 9th graders math and reading scoores affect Thomas HS performance relative to other schools

considerable downward dips

## How does replacing the 9th grade scores affect:
- Math and reading scores by grade
- scores by school spending
- Scores by school size
- Scores by school type

screen prints links?




# Summary
## Four major changes in the updated school district analysis after reading and math scores for Thomas HS 9th graders were replaced with NaNs
- 1  Math and reading scores in the student_data_df was changed to reflect the replacement of NaNs
- 2  The replacement also affected the combined school dataframe
- 3  The averages for passing were affected
- 4  The percentage calculations for school and overall performance were affected, which in turn changes the top 5 or bottom 5 rankings

