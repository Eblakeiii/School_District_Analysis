# School District Analysis

# Overview
The purpose of this analysis was to analyze the adjusted district data.  The data adjustment was replacing the reading and math scores, from Thomas High School 9th graders, with  NaN (herein to be referred to as the Thomas Freshmen).  The results of this analysis compared the adjusted outcome to the original analysis to determine the impact, if any. 

The district wide analysis encompased:
*  15 high schools, considered either District or Charter.
*  Combined total student population was 39,170.
*  Total combined annual budget of $24,649,428.
*  Student population of the Thomas High School was 1,635. 
*  Thomas Freshmen was 461, or 28.12% of the Thomas High School population, or 1.18% of the total district population.
*  Thomas High School school type is Charter.

# Results
## Thomas Freshman affect on the District Analysis
The impact the replaced scores of the Thomas Freshmen was minimal to none on a district wide level.  Fixed variables such as number of schools, budget and total number of students, remained the same.  The changes in the average scoring outcomes were similiarly close to being unchanged.  The only notable difference was a small decrease in % Passing Math (from 75% to 74%), % Passing Reading (from 86% to 85%) and % Overall Passing (from 65% to 64%).  

## Thomas Freshman affect on the By School Summary Analysis
As in the district wide study, the calculations using fixed variables remain unchaged.  The change in averages for both the math and reading was almost negligible, even though the Thomas Freshmen represent over a quarter of the population of their school.  The passing percentages, on the other hand, had material declines. The percentage decrease in passing rates are all slightly over 28%.  See table below for the breakdown for math, reading and overall passing rates. 

    ORIGINAL passing rates for:            ADJUSTED passing rates for:
    math    reading   overall              math    reading   overall  
    -----   -----     --------             -----   -----     --------
    93.3%,   97.3%     90.9%,              66.9%    69.7%     65.1%

## Thomas Freshmen affect on School Ranking
Prior to any replacement of the Thomas Freshmen, Thomas High School was ranked #2 at 90.9% in terms of overall achievement performance.  With the Thomas Freshmen adjustment, their ranking fell to to ranking #8 at 65.1%.  This aligns with the 28% fall in passing scores shown above.


## Thomas Freshmen affect on:
- Math and reading passing scores by grade

	Making any comparisons on a school grade level is not possible as the Thomas Freshmen math and reading scores were replaced with NaN.   

- Passing scores by school spending

	Spending per student was calculated by dividing the budget amount by the number of students for a particular school.  The schools were then classified into spending 		bins based on the amount.  The spending per student amount does not change, nor does the average math and reading scores.  The lack of impact is anticpated as 			calculations are based on fixed values.  Percentage passing scores, however, saw a decline in rates when they were compared in their spending bin.  Click to see the 		[table](https://github.com/Eblakeiii/School_District_Analysis/blob/master/Resources/bySpend.png) for details.
		        
- Scores by school size

	Each high school was classified by as size as small, medium or large based on the student population.  Thomas High School is a medium size school was was placed in Bin 	1000-2000.  Again, the averages in the math and reading remain unchanged.  The percentage passing rates fell slightly.  Click to see the [table](https://github.com/Eblakeiii/School_District_Analysis/blob/master/Resources/bySize.png) for details.

- Scores by school type

	There are two different types of school, District or Charter.  Thomas High School is a Charter school.  There was no impact on the average math and reading scores.  		However, there was a slight decline in the percentage passing rates.  Click to see [table.](https://github.com/Eblakeiii/School_District_Analysis/blob/master/Resources/byType.png) for details.

# Summary
## Four major changes  due too the Thomas Freshmen 
### 1. Math and reading scores was changed to reflect the replacement of NaNs

The reduction of the passing rates for math, reading and overall was an expected result.  When the scores for the Thomas Freshmen were replaced with NaN, their scores 		were eliminated from calcuations involving average and scores.  The result was equivalent to using scores of zero (0).  Exacerbating that imprecision, the count of the 	students (461), was not removed from the population of students, thus skewing the data even further.  Mathematically, reducing the numerator while holding firm on the 		denominator, will result in a smaller number.  This factor is the driver for the downward shift in passing scores.

### 2. The replacement also affected the combined school results

Parallel to the comments noted above, the combined school passing results were slightly skewed lower.  The impact of the combined passing scores is not as large, as the 	Thomas Freshmen population was a very small percentage of the overall student body.    

### 3. The analysis of speding bins and school sizes were affected

As mentioned above, schools were grouped into categories by school size (small, medium, large) and by spending per student amounts (4 spending bins).  Classifying each 	school into one of several spending bins and size category, achievement markers were compared.  Because the rates themselves are lower, the apportioned values were also 	lower.  The severity of the reduction depended on how large a component Thomas High School was in that particular calculation.     

### 4. The top 5 rankings reordered

In the original analysis, Thomas High School was consiered a top ranked school based on passing rates.  With the adjustment of the Thomas Freshmen, their passing rates 	plunged, causing their ranking to fall to #8.  This shift downward was mirorred in all the analysis involving passing scores.  

# Conclusion
There are various approaches to perform an analysis when a portion of the dataset is potentially compromised.  Replacing the math and reading scores with NaN was a simplistic method and the findings were predictable.  Only one variable changed, skewing the results in a anticpated pattern.  To improve the veracity of the results, the student count for Thomas High School should have been reduced by 461 students.  Then the calculations involving scores would have been adjusted appropriately - reducing both numerator and denominator.    

