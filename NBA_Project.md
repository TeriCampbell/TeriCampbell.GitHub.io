# Sports Stats Spotlight, 2021-22 NBA Case Study
 
## INTRODUCTION

**Project description:** Basketball is full of stats on players and teams.
<br><br>
This project is a case study using NBA data for the 2021-22 season.

<br><br>
**What I Learned**
* Nikola Jokić is an outlier with excellent stats for rebounds, assists, and points scored
* Most high score, high assist players are point guards
* when measuring 3-point efficiency, the strongest position varies by team 
* Rayjon Tucker stands out as a 3-point scorer while
* Trae Young stands out for overall points scored
* The greatest number of assists are made by point guards, followed by shooting guards
* James Harden, a point guard, has an impressive number of assists 


<br><br>
## DATA

I started by uploading the provided MA_Public_Schools_2017 Excel file into Tableau Public. The data set contains 200 rows and 298 fields.
<br><br>
A scan of college attendees by zip code
<img src="images/Distribution of College Attendees.png?raw=true"/>

<br><br>
## ANALYSIS
<br><br>
The first task was to determine the lowest performing schools. The data was filtered to remove null values because the dataset includes primary and secondary grades.
<br><br>
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>
<br><br>
The above visualization shows school graduation rates from lowest to highest. Data for one school, Curtis-Tufts High School, which notably has a 0% graduation rate, was filtered from analysis of graduation rates. The school is an alternative high school for students from Medford High School. Graduating Students received degrees from Medford High School. I also filtered out null graduation values so that data from primary schools would not interfere with the results.
<br><br>

My next task was to assess the impact of class size on college attendance rates.
<br><br>
On initial observation, I saw a bit of an increase in college attendance as class size increased up to around 20 students per class. But, digging deeper and filtering for economic status, it is noted that economically disadvantaged youths have a decreased college attendance rate as compared to their counterparts.
<br><br>
<img src="images/PercentCollegeVsClassSize_Image.png?raw=true"/>
Percent of College Attendees in Relation to Class Size

<br><br>
Looking deeper at the impact of economic disadvantage:
<br><br>
<img src="images/PercentCollegeVsEconomicDisadvantage_Image.png?raw=true"/>
Percent of Economically Disadvantaged Students who Attend College

<br><br>
Clearly this shows that the schools with fewer disadvantaged students have higher rates of college attendance. Further, the students who were English language learners (ELL) in this group were less likely to attend college.
<br><br>
<img src="images/PercentCollegeVsELL_Image.png?raw=true"/>
Percent of English Language Learners who Attend College
<br><br>
It is noted that the fewer ELL students are in a class, the greater the college attendance rate; however, economic status is distributed broadly across the percentage of college attendees when we isolate for ELL students as an isolated group.
<br><br>
The assumption made in this challenge is that passing 4th grade math scores are correlated with increased student success.
The next analysis looks at which schools had over 50% passing math grades in the 4th grade.
<br><br>
<img src="images/SchoolsPassingMath_Image.png?raw=true"/>
<br><br>
Now that these schools have been identified, educators in the high performing schools can be identified.

<br><br>
## RESULTS AND CONCLUSION

<img src="images/Dashboard_Massachusetts Student Success Evaluation.png?raw=true"/>

* Most high score, high assist players are point guards, but Nikola Jokić is an outlier with excellent stats for rebounds, assists, and points scored
* The strongest position for 3-point efficiency varies by team 
* Rayjon Tucker stands out as a 3-point scorer while Trae Young stands out for overall points scored
* The greatest number of assists are made by point guards, followed by shooting guards.  James Harden, a point guard, has the most impressive number of assists for the 2021-22 season





