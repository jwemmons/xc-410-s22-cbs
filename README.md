# XC 410 Spring 2022 - CBS Gender Pay Gap
This project was completed as a part of Boston University's Justice Media Journalism Co-lab during the Spring 2022 semester. The contributing members were Conor Kelley, Suzanne Crow, Phillip Huynh, Wenyan Zhang, Matteo David, and Jeffrey Emmons.

## Background
The concept of a gender pay gap, in which women are paid less than men for the same work, is something that has been investigated in the professional world for some time. CBS Boston wanted to investigate whether such a gap existed in state departments and executive offices in the state of Massachusetts. The state Comptroller provides open-access payroll data for these departments, but gender is not one of the listed data fields, presenting a challenge in investigating a potential pay disparity.

Therefore, we set out to determine the gender of the employees listed in the database. Using the gender-assignment algorithm Namsor, our team was able to calculate the most likely gender for each individual and conduct analysis to determine if a gender pay gap existed. After initial investigation, the scope of the project was narrowed to focus specifically on the University of Massachusetts System.

## Process
Data for the years 2017-2022 was first pulled from the Comptroller database (CTHRU) through the corresponding API. The focus of the project was on non-unionized individuals, so those associated with a bargaining group were filtered from the data. Individuals whose listed pay was negative were also removed. 
