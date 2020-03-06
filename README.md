# Attempting to Link BaltimoreCity Departments to Overtime
Organization and systematic analysis to ID departments that should be under review

I also know that a lot of health department locations were listed with specific the other year would love for he knows not the case different keep it consistent I ever moved the specific identification card application

Also note that since the blue-chip and youth summer positions were removed post-2014 they were not included in the analysis of the state of either

Also interesting to note that five election judges were paid a small sum of cash even though all 22 judges were not listed as having an official salary

As a standard procedure three digit identification codes her Department were removed because it complicated the pivot charts to properly analyze the data

Two big formulas were used to filter the state of first people were removed whether or not they are currently working for the city and technically they were removed if they weren't continuously employed by the city

 some interesting findings

Of 8427 employees reviewed, 337 are underpaid 1147 are overpaid. The three most underpaid departments are parks and rec Recreation section, with 139 out of 196 employees being underpaid. Crossing guards 49 out of 195 being underpaid. In the health department itself 31 out of 472 underpaid. 

The most egregious offenders in order Police Department,  Department of Water Sanitation,  and Fire Department. 

Now we identified systemic over or under payment based upon how many standard deviations away from they're listed annual salary people were paid.  we also summed the difference between the gross and a listed rates for the past. 2014 2016 2018-2019. 

Should be noted that at least once an indication of away from your annual pay with needed to be identified under or over. Few individuals were listed as having underpaid consistently about below 3 standard. Hundreds of individuals were listed as being overpaid by as much as two standard deviations up to five. It should be noted that the majority of these overpaid individuals from work from the police department. 


Data sets were downloaded, then combined together into one master copy
Vlookup was used to find and connect all the data together via tractID
A logic test was used to sum minority incomes, and check if altas did not find enough data points (~4,000) to give a value.
Areas segregated by State, using Name ID.
Pivot Tables were formed from data.

Data retrieved from: https://data.baltimorecity.gov/browse?category=City+Government
Excel Sheet where the data is primarily analyzed: https://github.com/Gramir10/Attempting_to_Link_BaltimoreCity_Departments_to_Overtime/blob/master/Analysis%20of%20Overtime%20per%20Department(Edits).xlsx
 

![alt text](https://github.com/Gramir10/Attempting_to_Link_BaltimoreCity_Departments_to_Overtime/blob/master/G4.png)
![alt text](https://github.com/Gramir10/Attempting_to_Link_BaltimoreCity_Departments_to_Overtime/blob/master/G5.png)
![alt text](https://github.com/Gramir10/Attempting_to_Link_BaltimoreCity_Departments_to_Overtime/blob/master/G1.png)
![alt text](https://github.com/Gramir10/Attempting_to_Link_BaltimoreCity_Departments_to_Overtime/blob/master/G2.png)
![alt text](https://github.com/Gramir10/Attempting_to_Link_BaltimoreCity_Departments_to_Overtime/blob/master/G3.png)

(-0.158713687* ANNUAL 2014)+(0.897846506*ANNUAL 2016)+(-0.257523929*ANNUAL 2018)+(0.634225738*ANNUAL 2019)-1566.89= Average Gross Annual Pay (In Dollars)

In an ideal situation, all of these coefficents should be 0.25. (Reflecting that Annual = Gross in a 1:1 ratio, and each year is 1/4 of the average)

Accounting for the fact that some worker are hourly, with paid overtime, some deviation is to be expected.									
As the R-Square Value is 0.8, we find high correlation between annual salaries, and the average gross salary. (Not a suprise)								
While 80% of cases can be explained by this model, what is of interest is the 20% that cannot be explained.									
By using this model, we can accurately predict 80% of people's gross salary's (thus having a more accurate budget).									
Another model is being worked on to capture the last 20% (Which will likely be the hourly workers with overtime, with ways of automatically tracking the largest deviations.									

