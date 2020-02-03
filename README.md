# Stack Overflow analysis

## Motivation
Stack Overflow hosts a community where users can ask and answer questions about computer programming. They have an annual survey where they examines all aspects of the developer experience. I wanted to investigate if there were any trends in the last three years.

This repository contains the Jupyer notebook with the source code I used for the blogpost [What does the yearly Stack Overflow survey tell us?](https://medium.com/@lukeerren/what-does-the-yearly-stack-overflow-survey-tell-us-ef273b882680)

## CRISP-DM
For this analsys I've made use of the CRISP-DM method.

### 1. Business Understanding
From the data I want to answer the following questions :
* From which country do most users come?
* How many programming languages do the user use?
* What are the most popular programming languages?
* Does number of programming languages influence income?

### 2. Data Understanding
The data consists of three separate files with the Stack Overfolw survey. Downloaded from the Stack Overflow website

The data files in this repository is an unaltered copy of the data that can be downloaded from the website from Stack Overflow. I used the surveys from 2017, 2018 and 2019.
https://insights.stackoverflow.com/survey

### 3. Data Preparation
* All three years of the suvey where loaded in one dataframe
* Harmonize the data; corrected different spellings. Like Viet Nam and Vietnam
* Delete some smaler programming languages, because there was no option to choose in all three years

### 4. Modeling the Data
Pivot tables where used for making the insights. Also some extra columns where added to make trends visable.

### 5. Results
* **From which country do most users come?**<br/>The top thre countries are United States, India and Germany. For all three years
* **How many programming languages do the user use?**<br/>An user uses on average 3.5 programming languages in 2017. And has increased to just below 4 in 2019.
* **What are the most popular programming languages?**<br/>The most popular programming languages ase JavaScript, SQL and Python
* **Does number of programming languages influence income?**<br/>Yes, a large number of Programming Languages has a negative influence on the salary if its more than about ten.

See the full blog post at : [What does the yearly Stack Overflow survey tell us?](https://medium.com/@lukeerren/what-does-the-yearly-stack-overflow-survey-tell-us-ef273b882680). 

# Files
- 2017 survey_results_public.zip	- The zipped survey results of 2017
- 2018 survey_results_public.zip	- The zipped survey results of 2018
- 2019 survey_results_public.zip	- The zipped survey results of 2019
- README.md - This file
- Stack Overflow Survey analysis.ipynb - The Jupyter notebook with the analysis

# Dependencies
This Python 3 workbook uses the following libraries:
- Pandas
- Matplotlib
- Numpy
- Seaborn

# Usage
Dowload the files to your Jupyter notebook directoy and un-zip the data files in the same directory. 

