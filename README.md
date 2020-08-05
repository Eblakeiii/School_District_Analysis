# School_District_Analysis

# Overview
The purpose of this analysis was to analyze the adjusted district data.  The data adjustment was replacing the reading and math scores, from Thomas High School 9th graders, with  NaN (herein to be referred to as the Thomas Freshmen).  The results of this analysis was to compare the adjusted outcome to the original analysis to determine the impact, if any. 

The district wide analysis encompased:
*  15 high schools, either considered district or charter
*  Combined total student population was 39,170
*  Total combined annual budget of $24,649,428
*  Student population of the Thomas High School was 1,635 
*  Thomas Freshmen was 461, or 28.12% of the Thomas High School population, or 1.18% of the total district population
*  Thomas High School school type is Charter

# Results
## Thomas Freshman affect on the District
- The impact the replaced scores of the Thomas Freshmen was minimal to none on a district wide level.  Fixed variables such as number of schools, budget and total number of students remained the same.  The changes in the average scoring outcomes were similiarly close to being unchanged.  The only notable difference was a 1% decrease in % Passing Math (from 75% to 74%), % Passing Reading (from 86% to 85%) and % Overall Passing (from 65% to 64%).  

## How is the school summary affected 
As in the district wide study, the calculations using fixed variables remain unchaged.  The averages for both the math and reading was almost negligible, even though the Thomas Freshmen represent over a quarter of the population.  The passing percentages, on the other hand, had material changes. See table below for the breakdown for math, reading and overall passing rates. 

    ORIGINAL passing rates for:            ADJUSTED passing rates for:
    math    reading   overall              math    reading   overall  
    -----   -----     --------             -----   -----     --------
    93.3%,	97.3%     90.9%,               66.9%	  69.7%	    65.1%

The percentage decrease in passing rates are all slightly over 28%.    XXXXXX Is this because the NaN sees the 461 scores as complete fails? XXXXXXX

## Hows does replacing 9th graders math and reading scoores affect Thomas HS performance relative to other schools
Prior to any replacement of the Thomas Freshmen, Thomas High School was ranked #2 at 90.9% in terms of overall achievement performance.  With the Thomas Freshmen adjustment, their ranking fell to to ranking #8 at 65.1%.  xxx add screen shots of the two reports xxx


## How does replacing the 9th grade scores affect:
- Math and reading scores by grade
Making any comparisons on a school grade level is not possible as the Thomas Freshmen math and reading scores were replaced with NaN.  However, 

- scores by school spending
The spneding per student amount does not change, nor do the average math and reading scores.  The lack of impact is expected as calculations are based on fixed values.  Regarding percentage passing scores, there is a decline in rates when they are compared in their spending bin.

	            Spending Bin	Avg Math Score	Aveg Reading Score	% Passing Math	% Passing Reading	% Overall Passing
                ----------------------------------------------------------------------------------------------------------
    Original:	    $630-644	    78.5	            81.6	          73	            84	                63
    Adjusted:	    $630-644	    78.5	            81.6	          67	            77	                56

- Scores by school size
Thomas High School is a medium size school (Bin 1000-2000).  Again, the averages in the math and reading remain unchanged.  The percentage passing rates fell slightly.
	
	 	Avg Math Score	Avg Reading Score	% Passing Math	% Passing Reading	% Overall Passing
					
Original: 	83.4			83.9			94		97			91
Adjusted:	83.4			83.9			88		91			85



- Scores by school type
There was no impact on the average math and reading scores.  However, there was a slight decline in the percentage passing rates.  See below table for details.

                           Avg Math Score  Avg Reading Score	% Passing Math	% Passing Reading	% Overall Passing	
    ------------------------------------------------------------------------------------------------------------------
    Original:   Charter	        83.5	         83.9	            94	             97	                90                            
    Adjusted:   Charter         83.5	         83.9	            90	             93	                87



screen prints links?




# Summary
## Four major changes in the updated school district analysis after reading and math scores for Thomas HS 9th graders were replaced with NaNs
- 1  Math and reading scores in the student_data_df was changed to reflect the replacement of NaNs
The reduction in passing rates for math, reading and overall was an expected result.  When the scores for the Thomas Freshmen were replaced with NaN, their scores were eliminated from calcuations invovling scores.  The result was an equivalent of using scores of zero (0).  Exacerbating that imprecision, the count of the students (461) was not removed from the total and individual population of students.  Reducing the numerator while holding firm on the denominator, the result will be a smaller number.

- 2  The replacement also affected the combined school dataframe.
Parallel to the comments noted above, the combined school passing results were slightly skewed lower.  The impact of the combined passing scores is not as large, as the Thomas Freshmen population was a very small percentage of the overall student body.    

- 3  The analysis of bins and sizes were affected
Using the combined school information calculated using fixed values for count and budget.  Categorizing each school into one of several spending bins, statistics were measured.  Since you're slicing and dicing the same information into different buckets, the passing rates will always come out lower.  The severity of the reduction will depend on how large a component Thomas High School was in that particular calculation.  The same logic applies to the analysis of slicing the data by the size of the school.  The changes in the medium bin was, once again, affected by the scores replaced with NaN. 

- 4  The percentage calculations for school and overall performance were affected, which in turn changes the top 5 or bottom 5 rankings
It follows the lower passing scores changed the achievement ranking for Thomas High School - falling from the #2 spot to #8.  This shift downwardis mirorred in all the other analysis invovling passing scores.  

# Conclusion
There are various approaches to perform an analysis when a portion of the dataset is potentially compromised.  Replacing the math and reading scores was a simplistic method and findings of the analysis was expected.  Only one variable changed, skewing the results in a predictable pattern.  To improve the veracity of the results, the student count for Thomas High School should have been reduced by 461 students.  Calculations invovling any scores would have been adjusted appropriately - reducing both numerator and denominator.    

