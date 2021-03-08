# School_District_Analysis
## Overview
The purpose of this analysis is to provide summary metrics of a school districts performance to provide organized data to a school board. This analysis looks at student's academic performance in 15 high schools, and accounts for the schools size, budget, the type of school that it is. Students are graded on their standardized test scores in reading and math. I also present an average for each subject, as well as overall passing as determined by a passing grade in both reading in math. I present a district level and school level summary of this data, so that school board members can make budgeting choices, or determine if corrective action is needed for poor performing schools. I was made aware of a data integrity issue for the ninth graders at Thomas High School - these results were voided in my analysis for purposes of determining averages, but these students were kept in for budgetary purposes. I will reference several dataframes in this analysis, but screenshots of key analyses can be found in the Resources folder of this project. 
## Results
# District Summary

![District_summary](https://user-images.githubusercontent.com/76958825/110390941-c2377080-8034-11eb-94fc-707b96de3264.png)

The results for the district can be found above. Note that the total students column has 38,709 students, which is less than we previously analyzed as in this summary we did not want to include the 9th graders at Thomas High School who had invalid test scores. Overall district scores were not impacted greatly by the removal of these students - which makes sense because they were only about 1000 out of the total near 40,000 students that we initially looked at. However, their removal will be shown more clearly later in this analysis. The overall passing score of 64.9% does jump out to me - though this metric can be slightly skewed by poorer performers in school as a whole - they are more likely to fail both reading and math. However the school board should make note of this low metric in their decision making in the future. 

Removing the ninth graders at Thomas High School had a huge impact in the performance of Thomas High School. Thomas High School's "9th Grade Included" scores can be found here, and the adjusted scores after. 

![THS_Unadjusted](https://user-images.githubusercontent.com/76958825/110391637-c87a1c80-8035-11eb-9522-3614240cbd0a.png)

![THS_AdjustedScores](https://user-images.githubusercontent.com/76958825/110391676-daf45600-8035-11eb-93d9-515b4aba3301.png)

Removing these students showed a 26% increase in % Passing Math, a 12% increase in % Passing Reading, and a 25% in overall passing. Those are impressive results for the 10-12th graders at Thomas High School! Additionally, this removal moved Thomas High School from the lowest percentile in performance to the highest. 
