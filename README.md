# School District Analysis

## Overview of Project

### Background Information
Py City School District's school board asked for an analysis of high school math and reading scores along a variety of measures: per school, per grade level, by school spending per student, by school size, and by school type. After reviewing the original analysis, the school board expressed concern that the data showed evidence of academic dishonesty, specifically in the 9th grade reading and math scores at Thomas High School (THS). At the board's request, a new analysis was done with the THS 9th grade scores removed. This report will describe the impact of removing the affected scores on Thomas High School's results and on the school district's results as a whole.

Throughout the analysis, student privacy was maintained and all identifying information has been removed from the final dataframes in this report.

### Method
We began by locating the 9th grade reading and math scores from Thomas High School in our data frame and replacing them with a null value, NaN. We then determined the number of THS 9th grade students (461) so that we could rerun the school and district calculations without the impacted scores. After cleaning up the data, we reran all the reports that were included in the first analysis.

## Results
### District Summary
As the two images below demonstrate, there is no significant impact to the school district results. The revised average math score is 0.1 less than the original, and there is no change in the average reading score. All passing percentages are identical when rounded to the nearest whole. *(Top image: School District Summary - Original, Bottom image: School District Summary - Revised).*

![sd_summary_original](https://user-images.githubusercontent.com/103977956/172311639-8fb418bd-f6cb-4da0-ae7f-ca945eeaf48d.png)
![sd_summary_revised](https://user-images.githubusercontent.com/103977956/172311642-5ec9eecb-8550-4704-a559-f124749273d1.png)

### Thomas High School Summary
Similar to the district results, the impact of removing the 9th grade scores is insignificant. The most significant difference is in the % Passing Reading and % Overall Passing where the revised scores are about 3/10 of a percentage point lower than the original. *(Top image: Top 5 High Performing Schools - Original, Bottom image: Top 5 High Performing Schools - Revised).*

![THS_summary_top5_original](https://user-images.githubusercontent.com/103977956/172318745-d8bdf693-0be6-43eb-a518-be95b1e5a277.png)
![THS_summary_top5_revised](https://user-images.githubusercontent.com/103977956/172318747-03f85110-47a9-42e9-b936-05a9f39e5c16.png)

### THS Performance Relative to Other Schools
In the original and revised results, THS is the second top highest scoring school in the district. There is no change to the ranking order as a result of removing the 9th grade THS scores (refer to images above).

### Impact on Other Measures
- *Math and Reading Scores by Grade.* The scores by grade are calculated by the grade level per school. As such, the only impact in this measure is to the THS 9th grade math and reading scores which are now marked NaN. (Images of math scores by grade below).

![math_scores_grade_original](https://user-images.githubusercontent.com/103977956/172323709-42d94254-9344-4d7a-994b-393ad857059c.png) ![math_scores_grade_revised](https://user-images.githubusercontent.com/103977956/172323712-f42e33a2-d7c2-4aa5-a2e4-74917d8f5885.png)

![reading_by_grade_original](https://user-images.githubusercontent.com/103977956/172333968-fc730fb3-8921-4b19-9320-781f5ab15484.png) ![reading_by_grade_revised](https://user-images.githubusercontent.com/103977956/172333972-7acaed2c-cf10-4b81-9500-4406e365360b.png)


- *Scores by school spending per student.* The data shows that the two middle spending categories were impacted by removing the 9th grade THS scores. In the $586-630 range, all scores increased in the revised analysis, the most significant being a 9 point rise from 81 to 90 percent in % Overall Passing. The 631-645 range saw more modest increases, the largest being three points in both % Passing Math and % Overall Passing.

![school_spending_original](https://user-images.githubusercontent.com/103977956/172326309-8907eea6-61f7-4f13-aa50-6fc7231414a3.png)
![school_spending_revised](https://user-images.githubusercontent.com/103977956/172326311-ed17cf90-a5ff-444c-8752-ef1ca557e6f7.png)

- *Scores by school size.* Removing the THS 9th grade reading and math scores made no impact on the results for scores by school size.

![school_size_original](https://user-images.githubusercontent.com/103977956/172329199-54707a61-95e8-44dc-a3cd-fda714b3914b.png)
![school_size_revised](https://user-images.githubusercontent.com/103977956/172329201-4fe0ca87-a1de-4b73-a515-6dd140b40d1a.png)

- *Scores by school type.* Removing the THS 9th grade reading and math scores made no impact on the results for scores by school size.

![scores_by_type_original](https://user-images.githubusercontent.com/103977956/172330340-7a677472-1571-493a-aaac-bec38dd0ea04.png)
![scores_by_type_revised](https://user-images.githubusercontent.com/103977956/172330341-03855b40-3140-4bab-a712-feb3b517074a.png)

## Summary
The impact of removing the reading and math scores for 9th graders at Thomas High School is, for the most part, insignificant. There was a slight drop in the overall district scores, 0.1 at most. THS scores saw a slightly bigger drop, 0.3 at most. The most surprising result is in the Scores by School Spending. The original and revised analyses show that schools in the two lowest per student spending categories have the highest overall passing percentages. In the revised analysis, the second lowest category has a nine point rise to tie with the lowest category for the highest overall passing pecentages at 90%. With the two higher spending categories scoring at 66% and 54%, school spending per child is an area that the district may want to investigate more thoroughly.
