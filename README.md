# School_District_Analysis
## Overview
The purpose of this analysis is to provide summary metrics of a school districts performance to provide organized data to a school board. This analysis looks at student's academic performance in 15 high schools, and accounts for the schools size, budget, the type of school that it is. Students are graded on their standardized test scores in reading and math. I also present an average for each subject, as well as overall passing as determined by a passing grade in both reading in math. I present a district level and school level summary of this data, so that school board members can make budgeting choices, or determine if corrective action is needed for poor performing schools. I was made aware of a data integrity issue for the ninth graders at Thomas High School - these results were voided in my analysis for purposes of determining averages, but these students were kept in for budgetary purposes. I will reference several dataframes in this analysis, but screenshots of key analyses can be found in the Resources folder of this project. 
# Results
## District Summary

![District_summary](https://user-images.githubusercontent.com/76958825/110390941-c2377080-8034-11eb-94fc-707b96de3264.png)

The results for the district can be found above. Note that the total students column has 38,709 students, which is less than we previously analyzed as in this summary we did not want to include the 9th graders at Thomas High School who had invalid test scores. Overall district scores were not impacted greatly by the removal of these students - which makes sense because they were only about 1000 out of the total near 40,000 students that we initially looked at. However, their removal will be shown more clearly later in this analysis. The overall passing score of 64.9% does jump out to me - though this metric can be slightly skewed by poorer performers in school as a whole - they are more likely to fail both reading and math. However the school board should make note of this low metric in their decision making in the future. 

Removing the ninth graders at Thomas High School had a huge impact in the performance of Thomas High School. Thomas High School's "9th Grade Included" scores can be found here, and the adjusted scores after. 

![THS_Unadjusted](https://user-images.githubusercontent.com/76958825/110391637-c87a1c80-8035-11eb-9522-3614240cbd0a.png)

![THS_AdjustedScores](https://user-images.githubusercontent.com/76958825/110391676-daf45600-8035-11eb-93d9-515b4aba3301.png)

Removing these students showed a 26% increase in % Passing Math, a 12% increase in % Passing Reading, and a 25% in overall passing. Those are impressive results for the 10-12th graders at Thomas High School! Additionally, this removal moved Thomas High School from the lowest percentile in performance to the highest. 
## Top and Bottom 5 Schools
The top 5 and bottom 5 schools can be shown here, ranked by their % Overall Passing.

![Top5Schools](https://user-images.githubusercontent.com/76958825/110395007-63c1c080-803b-11eb-9859-bf0e0be1b0be.png)

![bottom_5_schools](https://user-images.githubusercontent.com/76958825/110395019-6a503800-803b-11eb-8f52-a727b9e07a08.png)

The top 5 schools are all charter schools, and the lowest 5 schools are all District schools. Additionally, I note the relative size difference between the top 5 schools and the bottom 5. The top 5 schools all have student bodies of less than 2300. The bottom 5 have student body sizes of 2917 - 4761. There is a clear performance gap between Charter and District schools, and the size of these schools may also play a role in explaining this divide. Additionally, let's look at the per student budget for Cabrera HS, the highest performing school, versus Rodriguez HS, the lowest. There is only a $55 per student difference in their per student budget. Clearly, there is a gap in the marginal return on each dollar spent per student at these high schools. This is an area that certainly requires further analysis to first explain that gap, before we can aim to close it.

## Math and Reading Scores by Grade
Below are the math and reading scores by grade level for the district.

![Math_scores_by_grade](https://user-images.githubusercontent.com/76958825/110392269-ae8d0980-8036-11eb-894a-4ebf94954f6c.png)

![reading_score_by_grade](https://user-images.githubusercontent.com/76958825/110392318-bf3d7f80-8036-11eb-9f3a-389fb002723c.png)

Note that in each dataframe, the scores for 9th graders for Thomas High School are null. Thomas High School boasts results in the low 80% area for math scores for all grades, which is healthily above the district average in these categories.

## Scores by School Spending
Below are the scores by how much each school spends per student by spending buckets.

![score_summary_on_per_student_spending](https://user-images.githubusercontent.com/76958825/110392870-9ff32200-8037-11eb-893a-43433cf7b4fb.png)

One interesting takeaway from this dataframe is that the best performing group of schools in these buckets are actually schools that spend the least per student. The "$<584 per student" bucket actually has the best results in every test category. I also note the relatively poor performance of the schools in the "$645-675" bucket. The school board should further examine what may be driving these poor results in the group of highest budget per student group.

## Scores By School Size

Below are the score results for the various sizes of schools in the district.

![score_summary_on_school_size](https://user-images.githubusercontent.com/76958825/110393309-4f2ff900-8038-11eb-8e07-92632c18fdd0.png)

I note that the lowest score in % Overall Passing comes in the cohort of the largest schools. Large schools, with student bodies between 2000-5000 students only had a 58% passing rate. Small schools, with less than 1000 students, had an overall passing of 90%. That is a 32% gap between small schools and large schools! One interesting takeaway from this chart is that despite the overall poor passing rate of large schools, their average math and reading scores are not far from, or even above the district average. I wonder if over-burdened guidance counselors are not able to reach the poor-performers in the largest schools, and as a result more are failing. This is another area that the school district may want to further investigate.

## Scores by School Type

![score_summary_by_type](https://user-images.githubusercontent.com/76958825/110394736-ebf39600-803a-11eb-82fd-7029e989f996.png)

This chart shows that Charter schools are considerably outperforming District schools in every score category - with the highest differential coming in the % Overall Passing column. This was already apparent in the top 5 and bottom 5 analysis above. Still, these results are very plain to see - Charter schools are achieving much better results than their district counterparts. 

# Summary
* Removing 9th grade results from Thomas High School showed that the 10-12th graders performed at above District average levels in all categories
* After removing 9th grade results from Thomas High School, the school went from being in need of critical intervention to improve their scores, to a midlevel performer within the district. 
* Removing 9th graders did not have a noticeable impact on District level averages as they were a small sample of the entire population.
* Obtaining accurate data for Thomas High School is critical because as a Charter school, we observe a measureable gap in the performance of Charter versus District schools, and steps to bridge that gap require accurate data for all grade levels. 




