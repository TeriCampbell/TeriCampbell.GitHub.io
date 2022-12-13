# SQL Bank Project
 
## INTRODUCTION

**Project description:** The IDA......
<br><br>
The goal of this project was to gain insights from loans (credits) extended by the International Development Association (IDA) thought the World Bank Group.   
“The International Bank for Reconstruction and Development (IBRD) lends to governments of middle-income and creditworthy low-income countries.
The International Development Association (IDA) provides interest-free loans – called credits – and grants to governments of the poorest countries.
Together, IBRD and IDA make up the World Bank.”
<br><br>
**HYPOTHESIS:  **
I expected to see that…countries that ____ were slower, less likely, whatever to pay back their loans
I expect lower income countries would borrow at higher rates

<br><br>
The overarching question proposed is whether or not the State should build more schools.
<br><br>
**What I Learned**
* finding 1

* finding 2

* finding 3

<br><br>
## DATA

The “IDA Statement of Credits and Grants-Historical Data” data set was downloaded from world bank.org
You can access the data here:  https://finances.worldbank.org/Loans-and-Credits/IDA-Statement-Of-Credits-and-Grants-Historical-Dat/tdwh-3krx

Data was cleaned, filtered, and analyzed using PostgreSQL

??any weird cleaning issues?

The data set contains 1,109,994 rows and 30 fields

<br><br>
A scan of college attendees by zip code NOT FOR THIS PROJECT
<img src="images/Distribution of College Attendees.png?raw=true"/>  CHANGE THIS PIC

<br><br>
## ANALYSIS

<br><br>
I started by looking at.... 
<br><br>
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL query?  
<br><br>
results show... (maybe even give a pic of first few lines)
<br><br>

BE SURE TO INCLUDE ANY RELEVANT VIZ' FROM EXCEL AND EXPLAIN THAT YOU IMPORTED TABLES INTO EXCEL TO CREATE VIZ'

Next I....
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
## RESULTS AND RECOMMENDATIONS

<img src="images/Dashboard_Massachusetts Student Success Evaluation.png?raw=true"/>  CHANGE IMAGE.  GOOD TO INCLUDE EXCEL VIZ'  MAYBE A DASHBOARD PIC

Based on the above analysis, the following recommendations are indicated:
*  these areas had the most loans.  region and specific country
*  biggest borrowers (region and country) who owes the most?
*  percentage owed after x years
*  loans with higher/lower interest took longer to pay off?  Or some other cool finding
*  any groups that were higher risk to lend to?

<br><br>
## CONCLUSION

Lending assessment reveals trends .... 
<br><br>
Further exploration of....

Monitoring interest rates and .... 

Further monitoring factors such as  
