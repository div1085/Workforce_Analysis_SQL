# Pewlett-Hackard-Analysis

## Overview of the Project
Purpose of this deliverable, was to find out the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program. And further, analyze the results to help organization prepare for 'silver tsunami'.

Our retiring employees were select from all employees born between January, 1 1952 and December, 31 1955, who are approaching the retirement age.

## Results

1. From the finding of the eligible retirees, 30% of the workforce could retire at any given time.
2. From the job titles of the eligible retirees, the breakdown is below.
  - 36%	Senior Engineer
  - 32%	Senior Staff
  - 16%	Engineer
  - 9%	Staff
  - 5%	Technique Leader
  - 2%	Assistant Engineer

3. With the total number of eligible mentorships, 1,940 mentees may not be able cover the gap of the eligible retirees.  If Pewlett-Hackard will compensate the loss by training from withing, the Bobby will need to widen the search parameter.
4. Our retiring_titles shows us the a majority of the employees of retirment age (57,668/90,398 = 64%) have senior titles.

## Summary:

Approximately 90,000 positions needs to filled in order to mitigate "silver tsunami". 

**-- Use Count() to sum the titles of retiring employees
-- and create retiring_titles table.
SELECT count(title), title
into retiring_titles
from unique_titles
Group By title
order by count desc;**

With the queruy we can find Senior Engineers, Senior Staff and Technical Leaders who are retirement-ready and can mentor the new Pewlett Hackard employees.
