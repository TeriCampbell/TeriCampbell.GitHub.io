# SQL Bank Project
 
## INTRODUCTION

**Project description:** The Historical Data for The International Development Association (IDA).  <br><br>
The IDA Statement of Credits and Grants provides data on "publicly guaranteed debt extended by the World Bank Group.  The IDA provides developmental credits, grants, and guarantees to its recipient member countries to help meet their development needs.  Credits from IDA are at concessional rates.  Data are in U.S. dollars calculated using historical rates."
<br><br>
“The International Bank for Reconstruction and Development (IBRD) lends to governments of middle-income and creditworthy low-income countries.
The International Development Association (IDA) provides interest-free loans – called credits – and grants to governments of the poorest countries.
Together, IBRD and IDA make up the World Bank.”
<br><br>
### The goal of this project was to gain insights and a snapshot view from loans (credits) extended by the International Development Association (IDA) though the World Bank Group.   

<br><br>
**What I Learned**
* India has both the greatest outstanding loan amounts and greatest number of recorded transactions

* Most loan amounts in India are held by "Controller of Aid Accounts & Audit"

* finding 3

<br><br>
## DATA

The “IDA Statement of Credits and Grants-Historical Data” data set was downloaded from world bank.org
The data can be found here:  https://finances.worldbank.org/Loans-and-Credits/IDA-Statement-Of-Credits-and-Grants-Historical-Dat/tdwh-3krx

Data was cleaned, filtered, and analyzed using PostgreSQL

The data set contained 1,109,994 rows and 30 fields


<br><br>
## ANALYSIS

<br><br>
#### First I wanted to know, what were the greatest amounts due? 
<br><br>
<img src="images/SQL1_top_10_amt_due.png?raw=true" width = "40%"/>  
<br><br>
<img src="images/1Table_top_10_amt_due.png?raw=true" width = "50%"/> 

<br><br>
#### Then which countries had the greatest outstanding amount?
<br><br>
<img src="images/SQL2_Max_owed_to_IDA.png?raw=true" width = "40%"/>    
<br><br>
<img src="images/2Table_max_owed_to_IDA.png?raw=true" width = "50%"/>   

#### Which countries had the greatest number of transactions?
<br><br>
<img src="images/SQL3B_Greatest_Number_of_Transactions.png?raw=true" width = "50%"/>    
<br><br>
<img src="images/3BTable_Greatest_Number_of_Transactions.png?raw=true" width = "60%"/> 

<br><br>
#### Looking deeper, here are the top project categories in India, which was found to have the most outstanding loan amounts 
<br><br>
<img src="images/SQL3_most_frequent_projects_India.png?raw=true" width = "50%"/>  
<br><br>
<img src="images/3Table_most_frequent_projects_India.png?raw=true" width = "60%"/>   

<br><br>
#### Which entity or entities hold the most loan amounts in India?
<br><br>
<img src="images/SQL4_who_has_most_loans_in_India.png?raw=true" width = "60%"/>   
<br><br>
<img src="images/4Table_who_has_most_loans_in_India.png?raw=true" width = "60%"/>   

<br><br>
#### Zooming back out; What percentage of the original loan amount remains unpaid by region?
<br><br>
<img src="images/Table6_Percent_loan_outstanding.png?raw=true" width = "60%"/>  
<br><br>
<img src="images/6SQL_percent_loan_outstanding.png?raw=true" width = "50%"/>  

<br><br>
#### Are the top percentages of unpaid loan amounts in India?
<br><br>
<img src="images/SQL7_Top_percent_outstanding.png?raw=true" width = "60%"/>  
<br><br>
<img src="images/7Table_top_percent_outstanding.png?raw=true" width = "50%"/>   

<br><br>
#### Finally, I explored which countries had the longest and shortest scheduled loan duration
<br><br>
<img src="images/Longest Loan Times.png?raw=true" width = "70%"/>  
<br><br>
<img src="images/Table Longest Loan Times.png?raw=true" width = "40%"/>  
<br><br>
<img src="images/Shortest Loan Times.png?raw=true" width = "70%"/>  
<br><br>
<img src="images/Table Shortest Loan Times.png?raw=true" width = "40%"/>  


<br><br>
## RESULTS AND RECOMMENDATIONS

The above analysis reveals the following:
*  India has the greatest outstanding loan amounts 
*  India also has the largest number of transactions
*  biggest borrowers (region and country) who owes the most?  The most loan amounts in India are held by the Controller of Aid Accounts & Audit
*  percentage owed after x years
*  loans with higher/lower interest took longer to pay off?  Or some other cool finding
*  any groups that were higher risk to lend to?

<br><br>
## CONCLUSION

The above insights could be used to further the stated goal of helping meet developing countries needs.  
<br><br>
Further research to understand barriers met by loan recipients could provide deeper understanding of each regions specific needs.
