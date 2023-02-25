# Analysis of Age and Speed in Olympic Swimming: 1896-2022
 
## INTRODUCTION

**Project description:**  Growing up as a competitive swimmer, the Summer Olympic Games were always a highlight of the season.  The swimming athletes continued to get faster year after year, and at times it appeared that the athletes got younger.  Until some star swimmers were highlighted who were in their 30’s and even 40’s.  Then came the year that is notorious in the swimming community for the introduction of swim suits with buoyant properties.  The suits were worn by swimmers in the 2008 games, but banned for use in the Olympic Games by 2010 due to performance enhancing properties.
<br><br>
I wanted to examine historical Olympic Swimming data to explore both age and speed of the athletes over the years.  In particular, I wanted to highlight the impact that the buoyant suit era had on olympic swimming results, including whether there was a lasting effect and if the times achieved would ever be beaten.

<br><br>

### This project was focused on gaining insights related to elite level swimming at the Olympic Games.
<br><br>
**Hypotheses**
* I expected to see progressively faster results in each event each year

* I expected to see that athletes ages, on average, increased slightly over the years

* I expected that the impact of the buoyant suit era might still be present, with the fastest times in some events still not yet meeting the fastest times from 2008.

* I expected any impact on time from the buoyant suit era would be represented equally across all events and seen in both men’s and women’s events.

Limitation:  this study looks exclusively at Olympic Games results and does not represent results and records outside of the Olympic Games such as other elite national-level events or world records.


<br><br>
## DATA

The dataset was downloaded from Kaggle and contains results for Summer and Winter Olympic Games for the years 1896-2022. It contains 4 tables, 3 of which were useful for the purposes of this project  It is noted that while the name of the data set is “Olympic Summer & Winter Games, 1986-2022”, the description clarifies that the data actually includes “Medals & Results & Athletes from Athens 1896 to Beijing 2022”.  Swimming records data for the 2022 Summer Games is limited to the top 8 finishers.

Olympic Swimming pool length is 50 meters long.  While some events have evolved over the years, this analysis focused solely on events that were consistent.  Certain events have not been a part of the swimming line up for as long as others, resulting in reduced overall results sections for these events.

The dataset can be found here:  https://www.kaggle.com/datasets/piterfm/olympic-games-medals-19862018

Data was cleaned, filtered, and analyzed using Excel, BigQuery Sandbox, and Tableau Public

<br><br>
## ANALYSIS

#### To start, I used SQL for cleaning and exploration and decided to focus on a single event, the Men’s 100m Freestyle.
First I wanted to see an overview of the entire field of the Men’s 100m Freestyle over all of the years recorded in this dataset.  
<br><br>
<img src="images/1A_EntireMen's100FreeField.png?raw=true" width = "80%"/>   
<br><br>
Interestingly, I was only getting results in 2020 for the top 8 finishers. To see what was going on, I took a quick peek and learned that the data set only contained the times for top 8 finishers for 2020.  I am curious who they are, how old they are, and how fast they are going.
<img src="images/1B_2020Men's100FreeOnly.png?raw=true" width = "60%"/>  
<br><br>
#### Zooming in and staying focused on the Men's 100 Freestyle, I now wanted to know who the medalists were.  Here are the top 3 finishers across the span of years.  
These results do show a drop in times for this event in 2008 that was not matched until the most recent games in 2020.  <br><br>
<img src="images/3Top3M's100FreeAllYearsHighlights.png?raw=true" width = "80%"/>     
<br><br>
<img src="images/3BM's100MTop3TimesWithPre2008.png?raw=true" width = "70%"/>  

<br><br>
#### Of course, it would be hard to say that I wasn’t interested in the overall winner in the event each year.  
The top time in 2008 was not achieved and beaten until the 2020 Olympic Games. 
<br><br>
<img src="images/4Men's100FreeWinners.png?raw=true" width = "80%"/>    
<br><br>
The relatively dramatic drop in winning time from 2004 to 2008 of 0.96 seconds is offset by a still impressive, but more modest, half second drop as the winning Olympic time from 2008 is finally beaten. 
<br><br>
<img src="images/Healthcare3Results.png?raw=true" width = "80%"/> 

<br><br>
#### In hospital service, costs incurred by procedures can be significant for the facility.  
Let's take a look at the top 10 specialties that order the most procedures on average.
<br><br>
<img src="images/HealthSQL4.png?raw=true" width = "80%"/> 
<br><br>
<img src="images/Healthcare4Results.png?raw=true" width = "80%"/>    

The results show that the medical specialties that have the largest average procedure count do not necessarily have the largest number of patients.  

In order for this information to inform business decisions, further exploration is indicated.
<br><br>
<img src="images/HealthSQL4B.png?raw=true" width = "80%"/> 
<br><br>
<img src="images/Healthcare4BResults.png?raw=true" width = "80%"/> 
<br><br>
This information can help the facility direct attention toward the specialties that are utilizing the most resources.

<br><br>
#### A hospital facility has further interest in understanding if the number of lab procedures might correlate to the number of days in hospital.
<br><br>
<img src="images/HealthSQL6.png?raw=true" width = "80%"/> 
<br><br>
<img src="images/Healthcare6Results.png?raw=true" width = "50%"/>    
<br><br>
As expected, there is an increase in the average number of procedures performed the longer the hospital stay.


<br><br>
#### A facility should understand what is going well and benefitting both patients and the business.  Here we explore data from patients who had an emergency admission, but who stayed less than the average time in the hospital.
<br><br>
<img src="images/HealthSQL5.png?raw=true" width = "80%"/>  
<br><br>
<img src="images/Healthcare5Results.png?raw=true" width = "80%"/>  

<br><br>
#### In addition to costs, a facility must be aware of any subconscious bias when providing care.  We can, for example, look at specific services and compare how care is provided across different demographics. 
<br><br>
<img src="images/HealthSQL7.png?raw=true" width = "80%"/>   
<br><br>
<img src="images/Healthcare7Results.png?raw=true" width = "110%"/> 
<br><br>
The above example reveals a need to explore deeper and address underlying contributing factors to what appears to be a racial discrepancy in obstetric and gynecological care practices. 


<br><br>
#### The facility management team will also be interested in readmission status in the specialty service of interest.   
<br><br>
<img src="images/HealthSQL8.png?raw=true" width = "80%"/> 
<br><br>
<img src="images/Healthcare8Results.png?raw=true" width = "90%"/>   
<br><br>
This easy to read set of results can serve as a template to help with a targeted investigation based on re-admission status.   


<br><br>
## RESULTS

The above analysis provides these insights:
* The majority of hospital admissions are less than 7 days
* Patients who have longer than 1 week hospital stays have a somewhat greater average number of diagnoses
* The medical specialties that perform the most procedures, on average, do not necessarily have the largest number of patients
* On average, the number of procedures performed increases the longer a patient is in hospital
* There is evidence to explore racial difference in the provision of medical care

<br><br>
## CONCLUSION AND RECOMMENDATIONS
Facilities can utilize insights from analysis such as that performed in this project to understand factors influencing patient care outcomes as well as financial impacts.<br><br>
Following trends over time for countries receiving loans could reveal successes and failures in the lending process and is worth further exploration.
<br><br>
The information gathered can guide policy, strategy, and staff education.
<br><br>
Regular analysis is indicated to stay on top of the impacts of these changes as well as health trends that may require updated strategies and policies.
<br><br>
Further research is also indicated to understand potential differences in care provided to patients of different races and demographics.
