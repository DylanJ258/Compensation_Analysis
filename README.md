# Compensation_Analysis
## Tools Used
* Python
* Jupyter Notebook
* Excel
## Introduction
* In this project, I will be playing the role of a Data Analyst tasked with looking into compensation for the Department of Technology in San Francisco.
* The goal is to use Excel to showcase my data analytics skillset and thought process by analyzing a mock issue within the department.
## Dataset Collection
### Employee Compensation Data San Francisco
* The original dataset contained over 850,000 rows of compensation data on employees across various departments in San Francisco between 2012-2022. I didn't need all of this data for my analysis so I decided to use Pandas within a Jupyter Notebook to clean it.
* First I imported my dependecies and loaded in the original employee compensation dataset.

  <img width="1008" alt="Screen Shot 2023-06-10 at 4 35 31 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/7d757088-e633-4e4c-a165-8e94de5e8b5a">
  
* I then created a new dataframe by selecting certain columns from the original dataset that would be necessary for this analysis, excluding the ones that were not in order to make things easier to read.

  <img width="1012" alt="Screen Shot 2023-06-10 at 4 26 59 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/63616c86-7075-4574-8000-6963dbc21399">
  
* Then I cleaned this dataset down to just show data between the years 2018-2022.

  <img width="1012" alt="Screen Shot 2023-06-10 at 4 31 07 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/d1b573db-0314-410c-b05c-2422b1a6f486">
  
* Next, I made the dataframe only inlude the Department of Technology.

  <img width="999" alt="Screen Shot 2023-06-10 at 4 31 56 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/8223d595-3ff7-43f3-9e59-6d244d957758">
  
* Finally I exported my new dataframe as a CSV in order to run my analysis on it in Excel.

  <img width="1009" alt="Screen Shot 2023-06-10 at 4 36 29 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/3aec2bca-8498-4672-bf89-3ffc7696c7d6">
  
### Consumer Price Index, San Francisco Area
* This dataset contained monthly/annual reports of the Consumer Price Index in the San Francisco area.
* I downloaded the Excel file for this dataset then moved it to a new sheet in my Technology_Compensation Excel file.
## Problem
* The City of San Francisco’s Department of Technology has been receiving complaints within their Accounting and IT departments regarding low compensation. 
* I have been tasked by management take a deeper look at our data on compensation and report back on any possible issues.
## Analysis
### Overview
* For this analysis, I will look at compensation trends within the Department of Technology over the past five years.
* To better see if the changes in compensation are within reason, I will compare it to the changes in the Consumer Price Index (CPI) in San Francisco over the same period.
  * CPI measures the average change over time in the prices paid by urban consumers for a market basket of consumer goods and services.
  * Therefore, by comparing the changes in compensation to the changes in CPI, we can see if the Department of Technology is adjusting its compensation according to the changes in the cost of living.
### Walkthrough of Excel Workbook Creation
* First, I created a pivot table that showed the average total salary, average total benefits, and average total compensation by year of every job within the Department of Technology so that I could see how the compensation over time.

  <img width="469" alt="Screen Shot 2023-06-10 at 5 02 02 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/3516e47f-3aa0-4bfe-8001-dc81a612dc0e">
  
* Next, I removed the pivot and added in the Annual CPI data from the CPI Data Sheet to my table. I also added columns for the percent change by year and the 5 year percent change. 
* I calculated the percent change by year and the five year percent change for salary, benefits, total compensation, and annual CPI by writing a macro that runs when you click a button. Below is the code for my macro and images of it running.

  <img width="480" alt="Screen Shot 2023-06-10 at 4 57 54 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/8872ee14-5a12-4577-819e-3a9fdbaf871c"> 
 
  <img width="84" alt="Screen Shot 2023-06-10 at 5 20 58 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/681cefc1-a076-4be6-8c8e-019a48a4aa84"><img width="309" alt="Screen Shot 2023-06-10 at 4 58 17 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/76effb71-b5fd-4b3b-bc9c-2acbaeccdab5"> <img width="309" alt="Screen Shot 2023-06-10 at 4 58 31 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/6d999344-3db1-4fd4-a473-ce5f2a35a731">
  
* Here is the resulting table: 

  <img width="680" alt="Screen Shot 2023-06-10 at 5 12 45 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/633025dc-7bf0-4d6c-b775-7e963e367ae3">
  
* Next, I added conditional formatting to the percent change by year cells in order to clearly show how they are changing in relation to annual CPI. I wrote a macro to do this that runs when you click a button.
  *  Red: Negative percent change
  *  Yellow: Positie percent change, but lower than the percent change in CPI for a given year.
  *  Green: Percent change is greater than the percent change in CPI for a given year.
  
  <img width="743" alt="Screen Shot 2023-06-10 at 5 19 39 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/04d50195-8068-4fab-a439-1f8de090d168">
  <img width="82" alt="Screen Shot 2023-06-10 at 5 20 51 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/8558b2ea-c9b6-44b7-aeb2-99193eb8ab26">
  
* Here is the resulting table:

  <img width="682" alt="Screen Shot 2023-06-10 at 5 24 16 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/2834cbdc-d971-47b5-b3ba-44ffc1cb4fe9">
 
* Next, I added the same conditional formatting to the 5 year percent change cells. Again, I wrote a macro to do this that runs when you click a button.

  <img width="737" alt="Screen Shot 2023-06-10 at 5 29 41 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/82fee653-df22-433d-bb7f-a15493705149">
  <img width="84" alt="Screen Shot 2023-06-10 at 5 29 57 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/2c8faf1f-a263-41d4-a554-bbf4bc7d64ab">

* Here is the final table displaying the compensation for the Technology Department that will be used for my analysis:

  <img width="681" alt="Screen Shot 2023-06-10 at 5 31 06 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/5edc90b8-92a5-4a4c-8f7b-b533a9f59cc8">

* I then repeated this process to create similar tables for specific job groups that I want to analyze. I used the macros I wrote to fill in the percent changes and apply the conditioal formatting. I excluded roles that didnt have at least one person with that title every year for the past five years in order to not skew the results.
* Accountants II-III Compensation

  <img width="680" alt="Screen Shot 2023-06-10 at 5 40 47 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/602b2b6a-a031-48a1-a6fd-d6e715c17ac6">

* IT Support Operations Admin II-V Compensation

  <img width="681" alt="Screen Shot 2023-06-10 at 5 41 16 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/fcbe5317-80b9-469f-8f15-0e162b91e9e2">

* Managers II-VII Compensation

  <img width="681" alt="Screen Shot 2023-06-10 at 5 41 29 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/8c4b02f6-d217-4e6e-ba16-b9bda9b3db64">

* Engineers Compensation

  <img width="681" alt="Screen Shot 2023-06-10 at 5 41 36 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/d47aa305-13ea-406a-9964-98a5d8442e56">
  
* Finally I created charts to visualize the data within these tables.

  <img width="305" alt="Screen Shot 2023-06-10 at 5 46 41 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/f18b7868-7080-403a-8ef4-35f1cdcaabbd">

  <img width="226" alt="Screen Shot 2023-06-10 at 5 47 07 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/b0e4fd8b-43a6-4551-8068-e1d610f72c1e">

### Analysis of Tables and Charts
* Department of Technology Compensation
  * When looking at the entire Department of Technology, you can see that there has been a gradual increase in total compensation each year aside from 2022, where we see our first negative change. 
  * While this recent decrease in total compensation, mainly in the form of benefits, might look bad, it is not a massive cause for concern, and further analysis would be required to see what caused this change. 
  * Overall, the change in total compensation over the past five years (13.8%) is just about in line with the change in annual CPI in the same period (14.5%), meaning we are accurately adjusting our employee’s total compensation with changes in the cost of living.
* Accountants II-III Compensation
  * We see a different story when narrowing our scope down to the Accountants.
  * There were sizable increases in aspects of compensation from 2018-2020. However, that was followed by sizable decreases in all aspects of compensation from 2020-2022.
  * While the overall change within these five years is positive (7.5%), it is not in line with the change in annual CPI over the same period (14.5%), which is a cause for concern.
* IT Support Operations Admin II-V Compensation
  * When looking at IT jobs, we can see that they were hit hard by the overall decrease in compensation that the Department of Technology saw in 2022.
  * There was a steady increase in all aspects of compensation from 2018-2022. However, this increase was followed by a significant drop in 2022.
  * This drop caused the overall change within the past five years (5.2%) to fall well out of line with the overall change in annual CPI (14.5%) in the same period, which is a cause for concern.
* Managers II-VII Compensation
  * When looking at Managers' compensation over the past five years, we see that they were affected by the overall decrease in total compensation for the Department of Technology in 2022. However, they were less affected than the average. 
  * They have seen some slight decreases in total compensation within this period and some sizable increases.
  * These significant increases put their changes in total compensation within the past five years (28.5%) well over the change in annual CPI (14.5%) within the same period.
* Engineers Compensation
  * Engineering jobs saw a slight decrease in total compensation in 2019, followed by increases every year from 2020-2022. 
  * These increases in total compensation for Engineering jobs resulted in the overall change within the past five years (27.9%) being well over the change in CPI (14.5%) within the same period. 
  * This shows that the Department of Technology is adjusting total compensation at a great rate regarding changes in the cost of living.
## Conclusion
### Summary
* When looking at the Department of Technology as a whole, the changes in total compensation align with the changes in annual CPI. 
* However, we see some glaring differences when narrowing down the scope by looking at job groups within the Department of Technology. 
* Certain job groups, such as Managers and Engineers, are seeing significant increases in total compensation in regard to changes in annual CPI.
* However, job groups such as Accountants and IT are seeing just slight increases in total compensation that are well below the changes in annual CPI.
### Possible Solutions
* While it is good that the Department of Technology as a whole is properly adjusting total compensation with changes in CPI, it is concerning to see the disparity between certain job groups.
* This disparity needs to be addressed in order to make sure all employees compensation is being properly adjusted.
* Given that the Department of Technology as a whole is in line, no additional funding would be necessary to make sure every job is receiving a fair change in compensation.
* A reallocation of funds could be a possible solution. While this means certain groups might see smaller increases in compensation over the following years, it will also mean that other groups will be able to see increases more in line with changes in the cost of living.
## Sources
* Employee Compensation Data San Francisco: (https://data.sfgov.org/City-Management-and-Ethics/Employee-Compensation/88g8-5mnd Write references of books)
* Consumer Price Index, San Francisco Are: (https://www.bls.gov/regions/west/news-release/consumerpriceindex_sanfrancisco.htm)


*
























