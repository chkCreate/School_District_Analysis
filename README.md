# School_District_Analysis
  
## Overview of Project
  
### Purpose
  
The school board has notified that the students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. Although the school board does not know the full extent of the academic dishonesty, they want to uphold state-testing standards and have turned to our client for help. The client has asked us to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. This report presents some of our findings and summary on the impacts to the statistical results from omiting the subset under investigation.
  
## Results
  
The results are stated below.
  
- How is the district summary affected?
  
  See the images below for detail on the district summaries before and after the omission of the subset. The district average math score decreased by 0.1 point; % passing math score is lower by 0.2%; % passing reading score is lower by 0.3%; and therefore % overall passing is lower by 0.1%. The subset under investigation inflated the overall passing percentage by a 0.1%, which amounts to 3,917 students who may have passed or failed depending on the result of the academic dishonesty investigation. 
  
* Note that certain columns were not updated as it was not explicitly requested for in the challenge.
  
<p align="center">
  <img width="400" height="700" src= "https://github.com/chkCreate/School_District_Analysis/blob/2bed10f2b010f26b07fb177e5ca4e22728963577/Resources/pre_district_summary.PNG" title "Original District Summary">
</p>
  
<p align="center">
  <img width="400" height="700" src= "https://github.com/chkCreate/School_District_Analysis/blob/07e19a87e8ea9b5461cd5d47b3605d5315dda38d/Resources/district_summary.PNG" title "New District Summary">
</p> 
  
- How is the school summary affected?
  
School summary remained much of the same except for the results of Thomas High School. Before the omission of the ninth grade data, Thomas High School's percentage of students passing math, reading, and both were all higher that 90%. However, with the omission of the subset, the percentage of students passing dropped to the 60%'s - see the second image. This is not the end though, the percentages were recalculated without the ninth grade data in the total student pool and see the third image for the slight differences in results compared ot the original analysis. Most of the percentage of passing students decreased by a small tenth digit difference. Further investigation is recommended to assess the validity in question. See tables below for comparison.
  
<p align="center">
  <img width="400" height="700" src= "https://github.com/chkCreate/School_District_Analysis/blob/8f17f9a0fa9a8b20e6dbbbcc9fcc015d6e805d88/Resources/pre_School_summary.PNG" title "Original School Summary">
</p>
  
<p align="center">
  <img width="400" height="700" src= "https://github.com/chkCreate/School_District_Analysis/blob/aad3279f06b6ef5f9c706ad0c0b8972999834016/Resources/School_summary.PNG" title "New School Summary">
</p>
  
<p align="center">
  <img width="400" height="700" src= "https://github.com/chkCreate/School_District_Analysis/blob/a6a0906952d7fbc2a631b880db51301e6586708c/Resources/actual_school_summary.PNG" title "Actual School Summary">
</p>
  
* Note that certain columns were not updated as it was not explicitly requested for in the challenge.
  
- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
  
Compared to the high 80% to the low 90% of the overall passing percentage of students from Charter Schools, Thomas High School scores at ~65%. Before the replacement, the % overall passing was at ~90%. If the doubts prove true, Thomas High School could have been motivated to close the gap with the other Charter Schools, but the differences in the percentage passing data differ by the tenth digits. There needs to be a further investigation.
  
- How does replacing the ninth-grade scores affect the following:
  
* Math and reading scores by grade
  
See images below for math and reading scores by grade per school. The main differences to note are that both math and reading scores for 9th grade Thomas High School has been replaced as *NaN*.
  
<p align="center">
  <img width="400" height="700" src= "https://github.com/chkCreate/School_District_Analysis/blob/91be57e592d6e90f510e5090b1e348fca47db9c8/Resources/pre_math_scores.PNG" title "Original Math Scores by School Grade">
</p>
  
<p align="center">
  <img width="400" height="700" src= "https://github.com/chkCreate/School_District_Analysis/blob/91be57e592d6e90f510e5090b1e348fca47db9c8/Resources/math_scores.PNG" title "New Math Scores by School Grade">
</p>

<p align="center">
  <img width="400" height="700" src= "https://github.com/chkCreate/School_District_Analysis/blob/91be57e592d6e90f510e5090b1e348fca47db9c8/Resources/pre_reading_scores.PNG" title "Original Reading Scores by School Grade">
</p>
  
<p align="center">
  <img width="400" height="700" src= "https://github.com/chkCreate/School_District_Analysis/blob/91be57e592d6e90f510e5090b1e348fca47db9c8/Resources/reading_scores.PNG" title "New Reading Scores by School Grade">
</p>

* Scores by school spending
  
The % of students passing change from 90% to 81% in the $585-629 range; and from 66% to 63% in the $630-644. 9% change in the $585-629 and 3% change in the $630-644 range can amount to huge sums of money depending on the total number of students. The removal of the subset suggests that spending $585-629 increased the overall passing percentage by 9% and therefore, schools may believe higher spending per student in the two ranges may increase the overall percentage passing. See images below for the details.
  
<p align="center">
  <img width="400" height="700" src= "https://github.com/chkCreate/School_District_Analysis/blob/21a687a68b89a02240753f19893b31afbaef9b56/Resources/pre_school_spending.PNG" title "Original Scores by School Spending">
</p>
  
<p align="center">
  <img width="400" height="700" src= "https://github.com/chkCreate/School_District_Analysis/blob/21a687a68b89a02240753f19893b31afbaef9b56/Resources/school_spending.PNG"  title "New Scores by School Spending">
</p>
  
* Scores by school size
  
  The scores did not appear to differ too much from the original data set by school size. See figures below.
  
<p align="center">
  <img width="400" height="700" src= "https://github.com/chkCreate/School_District_Analysis/blob/ba449f1615c7e9944789a1d45417a0e692de8d62/Resources/pre_school_size.PNG" title "Original Scores by School Size">
</p>
  
<p align="center">
  <img width="400" height="700" src= "https://github.com/chkCreate/School_District_Analysis/blob/ba449f1615c7e9944789a1d45417a0e692de8d62/Resources/school_size.PNG" title "New Scores by School Size">
</p>
  
* Scores by school type
  
  The scores by school type did not differ too much with the amount of significant digits. See figures below.
  
<p align="center">
  <img width="400" height="700" src= "" title "Original Scores by School Type">
</p>
  
<p align="center">
  <img width="400" height="700" src= "" title "New Scores by School Type">
</p>
  
  
## Summary
  
After the reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs, the number of overall passing percentage of students in the district summary was reduced by 0.1%. With the omission the ninth grade subset, Thomas High School was not too far off from the original passing percentage of students compared to Charter Schools especially as it is identified as such. Analysis of scores by school spending show an increase of passing percentage of students in the second and third spending ranges, and therefore may suggest that higher spending per student in those ranges may be correlated to higher overall passing percentages. Scores by school size and school type did not appear to have been affected significantly from the change.
  
## References
  
(1) I referenced the image centering script from "https://stackoverflow.com/questions/12090472/github-readme-md-center-image".
  

