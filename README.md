# XC 410 Spring 2022 - CBS Gender Pay Gap
This project was completed as a part of Boston University's Justice Media Journalism Co-lab, in collaboration with CBS Boston, during the Spring 2022 semester. The contributing members were Conor Kelley, Suzanne Crow, Phillip Huynh, Wenyan Zhang, Matteo David, and Jeffrey Emmons. Instructors for this course were Brooke Williams and Osama Alshaykh.

## Background
The concept of a gender pay gap, in which women are paid less than men for the same work, is something that has been investigated in the professional world for some time. CBS Boston wanted to investigate whether such a gap existed in state departments and executive offices in the state of Massachusetts. The state Comptroller provides open-access payroll data for these departments, but gender is not one of the listed data fields, presenting a challenge in investigating a potential pay disparity.

Therefore, we set out to determine the gender of the employees listed in the database. Using the gender-assignment algorithm Namsor, our team was able to calculate the most likely gender for each individual and conduct analysis to determine if a gender pay gap existed. Through investigation and analysis, the scope of the project was eventually narrowed to focus specifically on individuals in the University of Massachusetts System that made $150k or more in a year.

## Process
Data for the years 2017-2022 was first pulled from the Comptroller database (CTHRU) through the corresponding API. The focus of the project was on non-unionized individuals, so those associated with a bargaining group were filtered from the data. Individuals whose listed pay was negative were also removed. 

Names from the dataset were then run through Namsor in batches of a hundred. Each batch took the form of a list of Python dictionaries and was passed in as part of a request to Namsor's API. A JSON was returned by the algorithm, from which the gender associated with each name was extracted and added to a new column in the dataset.

Analysis then began, consisting of several different calculations, visualizations, and transformations of the data. Of these, notable actions and visualizations include:
* a table displaying the difference in pay (as a percentage of male pay) between genders for every school, year, and position title combination.
* the calculation of the average difference in pay for a series of salary range buckets.
* a master report for the median pay per year between 2017-2021 of every position title earning $150k+ in a year, separated by gender. 
* color-coded pivot tables displaying pay difference by year.
* bar charts for the counts of individuals and unique position titles earning $150k+, separated by year, school, and gender. 

## Included Files
In this repository, you will find the code that we wrote to collect, clean, transform, and analyze the payroll data. All code was written in Python using pandas in Google Colab and Jupyter notebooks. You will also find visualizations made using Tableau and charts made in Excel.
