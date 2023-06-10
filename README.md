# Compensation_Analysis
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
### Walkthrough
* First, I created a pivot table that showed the average total salary, average total benefits, and average total compensation by year of every job within the Department of Technology so that I could see how the compensation over time.
  <img width="469" alt="Screen Shot 2023-06-10 at 5 02 02 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/3516e47f-3aa0-4bfe-8001-dc81a612dc0e">
* Next, I removed the pivot and added in the Annual CPI data from the CPI Data Sheet to my table. I also added columns for the percent change by year and the 5 year percent change. 
* I calculated the percent change by year and the five year percent change for salary, benefits, total compensation, and annual CPI by writing a macro. Below is the code for my macro and images of it running.
  <img width="480" alt="Screen Shot 2023-06-10 at 4 57 54 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/8872ee14-5a12-4577-819e-3a9fdbaf871c"> 
  
  <img width="309" alt="Screen Shot 2023-06-10 at 4 58 17 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/76effb71-b5fd-4b3b-bc9c-2acbaeccdab5"> <img width="309" alt="Screen Shot 2023-06-10 at 4 58 31 PM" src="https://github.com/DylanJ258/Compensation_Analysis/assets/104036750/6d999344-3db1-4fd4-a473-ce5f2a35a731">














