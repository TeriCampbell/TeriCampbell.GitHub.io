# SQL Bank Project
 
## INTRODUCTION

**Project description:** The Historical Data for The International Development Association (IDA).  
The IDA Statement of Credits and Grants provides data on "publicly guaranteed debt extended by the World Bank Group.  The IDA provides developmental credits, grants, and guarantees to its recipient member countries to help meet their development needs.  Credits from IDA are at concessional rates.  Data are in U.S. dollars calculated using historical rates."
“The International Bank for Reconstruction and Development (IBRD) lends to governments of middle-income and creditworthy low-income countries.
The International Development Association (IDA) provides interest-free loans – called credits – and grants to governments of the poorest countries.
Together, IBRD and IDA make up the World Bank.”
<br><br>
The goal of this project was to gain insights and a snapshot view from loans (credits) extended by the International Development Association (IDA) though the World Bank Group.   
 
<br><br>
**HYPOTHESIS:  **
I expected to see that…countries that ____ were slower, less likely, whatever to pay back their loans
I expect lower income countries would borrow at higher rates

<br><br>
**What I Learned**
* finding 1

* finding 2

* finding 3

<br><br>
## DATA

The “IDA Statement of Credits and Grants-Historical Data” data set was downloaded from world bank.org
The data can be founc here:  https://finances.worldbank.org/Loans-and-Credits/IDA-Statement-Of-Credits-and-Grants-Historical-Dat/tdwh-3krx

Data was cleaned, filtered, and analyzed using PostgreSQL

The data set contained 1,109,994 rows and 30 fields


<br><br>
## ANALYSIS

<br><br>
First I wanted to know, what were the 10 amounts due? 
<br><br>
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL query?  
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL results? 

<br><br>
Then which countries had the greatest outstanding amount
<br><br>
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL query?  
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL results? 

<br><br>
There are ---x--- total transactions from ---y---- which was found to have the most outstanding 
<br><br>
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL query?  
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL results? 

<br><br>
----y---- has the most loans (also from country with most outstanding)
<br><br>
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL query? 
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL results? 

<br><br>
Then total transactions per country (is this redundant to above?)
<br><br>
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL query?  
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL results? 

<br><br>
Top percentages of original loan scheduled for repayment by region/country
<br><br>
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL query? 
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL results? 


<br><br>
Next I explored which country was the most recent to make a payment
<br><br>
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL query? 
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL results? 


<br><br>
Finally I explored which region had the largest percentage of outstanding balance due
<br><br>
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL query? 
<img src="images/LowestGradRates_MA_Schools.png?raw=true"/>  CHANGE THIS PIC, SQL results? 



<br><br>
## RESULTS AND RECOMMENDATIONS

The above analysis reveals the following:
*  these areas had the most loans.  region and specific country
*  biggest borrowers (region and country) who owes the most?
*  percentage owed after x years
*  loans with higher/lower interest took longer to pay off?  Or some other cool finding
*  any groups that were higher risk to lend to?

<br><br>
## CONCLUSION

The above insights could be used to further the stated goal of helping meet developing countries needs.  
<br><br>
Further research to understand barriers met by loan recipients could provide deeper understanding of each regions specific needs.
