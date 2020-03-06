# Attempting to Link Baltimore City Departments to Overtime

### Procedure: ###

* Data sets were downloaded, then combined together into one master copy
* Vlookup was used to find and connect all the data together via Employee Name, in the data analysis, the names are not included
* Conditional Formatting visually tracks significant deviations of payment. 
* Pivot Tables were formed from data.
* Regression analysis from Data Analyze Tool was performed on Annual Salaries in relation to Gross Annual Salary
* Scatter Plot graphic formed by comparing average annual vs average gross salaries

### Data Selection Criteria, and Minor Changes###
* To be included in the model, people must be currently working for the city, and continuously employed by the city since 2014.
* Health Department had several locations marked out, they were pooled together, as the location data was inconsistent year to year.
* blue-chip and youth summer positions were removed post-2014, so they were filtered out per point #1.
* Three-digit identification codes of Departments were removed because it obfuscated the pivot charts.

Data retrieved from: https://data.baltimorecity.gov/browse?category=City+Government
Excel Sheet where the data is primarily analyzed: https://github.com/Gramir10/Attempting_to_Link_BaltimoreCity_Departments_to_Overtime/blob/master/Analysis%20of%20Overtime%20per%20Department%20(Edits).xlsx
 

![alt text](https://github.com/Gramir10/Attempting_to_Link_BaltimoreCity_Departments_to_Overtime/blob/master/G4.png)
![alt text](https://github.com/Gramir10/Attempting_to_Link_BaltimoreCity_Departments_to_Overtime/blob/master/G5.png)

(-0.158713687*ANNUAL 2014) +(0.897846506*ANNUAL 2016)+(-0.257523929*ANNUAL 2018)+(0.634225738*ANNUAL 2019)-1566.89= Average Gross Annual Pay (In Dollars)

In an ideal situation, all of these coefficients should be 0.25. (Reflecting that Annual = Gross in a 1:1 ratio, and each year is 1/4 of the average)

Accounting for the fact that some workers are hourly, with paid overtime, some deviation is to be expected.									
As the R-Square Value is 0.8, we find high correlation between annual salaries, and the average gross salary. (Not a surprise)								
While 80% of cases can be explained by this model, what is of interest is the 20% that cannot be explained.									
By using this model, we can accurately predict 80% of people's gross salary's (thus having a more accurate budget).									
Another model is being worked on to capture the last 20% (Which will likely be the hourly workers with overtime, with ways of automatically tracking the largest deviations.	
