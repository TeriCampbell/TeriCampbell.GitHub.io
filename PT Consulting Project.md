# Group Consulting Project:  Locating a New Physical Therapy Business in Florida
 
## INTRODUCTION

**Overview:**  
This collaborative group healthcare business consulting project utilized data mining and exploration of open source public datasets in order to provide data-informed recommendations to the client.  
<br><br>
### Business Problem: The client wants to open up a new physical therapy clinic in Florida. What are the top 3 locations for the client to open a new location?
<br><br>
**Assumptions:** 

1. The client wants a market in which to grow their business
2. The client will focus on an insurance based payment model and will accept Medicare, which is a growing population.  

**Findings**
<br><br>
Regions that support a greater number of physical therapists have:
* Average age over 38.5 years
* Middle to High average household income
* Larger population
* County unemployment rate < 7.3

Based on this analysis, a recommendation can be made to consider each of these specific locations as locations for a new physical therapy clinic with local demographic findings that match those of other regions that support higher numbers of physical therapists:
* Charlotte County, City of Punta Gorda, Zip Code 33982
* Collier County, City of Naples, Zip Code 34117
* Bay County, Panama City, Zip Code 32409


<br><br>
## DATA

Multiple public sources of data were identified, cleaned using SQL, and combined for this analysis.

Resultant data tables utilized for this business problem:
* uszips.csv - zip codes, population city, coordinates, county 2015-2022

* Fl.csv:  includes clinic locations, provider information, taxonomy codes

* FL_City_Pop.csv:  includes business address, number of providers, city and county names, and zip city population

* FL_Providers_Address.csv: includes business address, city, zip code, and number of providers at each address

**Data sources can be found here:** 
* https://hub.arcgis.com/datasets/FDACS::florida-demographic-information/explore?showTable=true
* http://edr.state.fl.us/content/population-demographics/data/index-floridaproducts.cfm
* https://download.cms.gov/nppes/NPI_Files.html
* https://www.nucc.org/index.php/code-sets-mainmenu-41/provider-taxonomy-mainmenu-40/csv-mainmenu-57
* https://simplemaps.com/data/us-cities

Data was cleaned, filtered, and analyzed using spreadsheets, SQL, and Tableau Public

<br><br>

## ANALYSIS

#### Joining the number of providers at each location with the demographic table reveals correlations associated with a higher number of providers.
Introductory exploratory analysis shows that:

* The lowest average age in the top regions that support the greatest number of physical therapists is 38.7
* The city population range in the top regions lies above 524 
* The zip code population range lies above 4700
* The county population range in the top regions is above: 155,000
* Unemployment rate by county in the top regions is below 7.3

<br><br>
<img src="images/PT_SQL_1.png?raw=true" width = "80%"/> 

<br><br>
<img src="images/PT_Results_1.png?raw=true" width = "80%"/>   
<br><br>

---
<br><br>
#### Exploring the average providers in each clinic in our top performing regions reveals that the top identified regions that support the most physical therapists have an average of 1.6 to  2.67 PT’s per clinic.
<br><br>
<img src="images/PT_SQL_1.png?raw=true" width = "80%"/>  
<br><br>
<img src="images/PT_Results_2.png?raw=true" width = "60%"/>     

#### As compared to an overall average provider rate of 1.66 by zip code  
<br><br>
<img src="images/PT_SQL_3.png?raw=true" width = "50%"/>
<br><br>
<img src="images/PT_Results_3.png?raw=true" width = "30%"/>

<br><br>
#### This reveals a successful saturation rate by city and zip. Criteria for inclusion should include regions with an average provider ratio below 1.6.
<br><br>
---
<br><br>
#### Further exploration identifies a city population range between 3 and 1186954, a zip code population range from 30 to 75705, and a county population range from 8308 to 2549075.
<br><br>
---
<br><br>
#### First the question of whether or not household income plays a role must be considered, which can be more easily visualized when categorized.

#### The range for median income falls between $32,497 and $64,876 by county:
* low: 30,000-40,000 
* middle: 40,000-50,000
* high: over 50,000 

#### Using these established criteria parameters gives quick view of average household income in the areas that support the greatest density of PT’s:

<img src="images/PT_SQL_4.png?raw=true" width = "100%"/>    
<img src="images/PT_Results_4.png?raw=true" width = "60%"/>   
<br><br>

#### Average household income above $39,000 is correlated with the greatest ratio of working providers in the population, indicating another aspect of successful business/market fit.
<br><br>
---
<br><br>

#### So far it is identified that the regions that support the greatest number of physical therapists have:
* Average PT/s Clinic between 1.6-2.67 (for city), overall average 1.66 for zip
* Larger population (county population > 155000, city pop > 524, zip pop over 4700
* Population median age > 38.5
* Average household income above $39,000
* Unemployment rate < 7.3   
<br><br>

#### TASK: Identify regions with less than 1.66 average therapists per zip while also having > 4700 zip population, County Population >155,000, median age over 38.5, Average Household Income above $39,000, and an unemployment rate below 7.3
<br><br>

---
<br><br>
#### As a final criteria addition, a look at the total number of facilities in the upper end of the established parameters is seen here:
<img src="images/PT_SQL_5.png?raw=true" width = "80%"/> 
<img src="images/PT_Results_5.png?raw=true" width = "80%"/> 
<br><br>

#### There is a trend for areas with larger county populations supporting a greater number of facilities.  Target regions for a new clinic should have a larger population, middle-to-high income, but a lower provider to population ratio and generally a lower number of facilities.
<br><br>  

---
<br><br>
#### Finally, Adding in the city population and ordering this from the lowest provider ratio we see the underserved areas population statistics.
<br><br>
<img src="images/PT_SQL_6.png?raw=true" width = "100%"/> 
<img src="images/PT_Results_6.png?raw=true" width = "100%"/> 
<br><br>
#### Further narrowing down to a city population over 19,000, the top potential regions emerge.
<br><br>
<img src="images/PT_Results_7.png?raw=true" width = "100%"/> 
<br><br>
<br><br>
## RESULTS & RECOMMENDATIONS

Based on this analysis, a recommendation can be made to consider each of these specific locations as locations for a new physical therapy clinic with local demographic findings that match those of other regions that support higher numbers of physical therapists:

* Charlotte County, City of  Punta Gorda, Zip Code 33982
* Collier County, City of Naples, Zip Code 34117
* Bay County, Panama City, Zip Code 32409

Specifically, we can recommend these individual locations as promising locations for a new physical therapy clinic with growth potential because the regional demographics fit the following identified criteria and each is relatively under-served compared to areas that support a greater percentage of providers:

* Average age of > 38.5
* Middle to High average household income
* Low provider to population ratio
* Higher population
* Unemployment Rate < 7.3

<br><br>
## CONCLUSION & CONSIDERATIONS
Other Considerations/options to pursue deeper:
<br><br>
The data found in these public data sets did not include information on lease prices in each area.
Looking at the client budget vs rent prices (eg. West Palm Beach seems like a good choice, but perhaps there are lower numbers of providers in that location because overhead is restrictive to profit).
<br><br>
Potential for further data exploration:
Average square footage cost for commercial real-estate for each city.
<br><br>
