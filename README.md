# python-api-challenge
Module 6 Python API Challenge

## Project Overview
For this task, I utilized SparkSQL to analyze key metrics about home sales data.

## Analysis
For my analysis of the data, I looked at the following questions:

1. What is the average price for a four-bedroom house sold for each year?

   The average price of a home in 2019 was $300,263.70. That average decreased slightly in 2020 to $298,353.78. It rose back up to $301,819.44 in 2021, and then dipped in 2022 to $296,363.88. The years that the dataset captured reflect the time of the pandemic, when housing prices were in flux, which may explain why a clear trend is not present.
   
1. What is the average price of a home for each year it was built that has three bedrooms and three bathrooms?
   
   The data shows that from 2010 to 2017, housing prices for a 3 bedroom, 3 bathroom home ranged from a low of $288,770.30 (in 2015) to a high of $295,962.27 (in 2013).
   
1. What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet?

   For homes in that same category, but with 2 stories and 2,000 sq. feet or more, the prices ranged from $276,553.81 (in 2011) to $307,539.97 (in 2012).
   
1. What is the "view" rating for homes costing more than or equal to $350,000?

   The number of views was the highest for homes priced over $1,000,000.00.

1. How did the runtime of uncached, cached, and formatted parquet home sales data differ?
   
   Starting with the data from the temporary table "home_sales," the run time to find the view rating took the longest at .87 seconds. Once the "home_sales" temporary
   table was cached, the run time was significantly reduced, taking only .53 seconds. From there, I partitioned the data and re-ran the code as third variable. The
   partitioned code ran in .39 seconds, which was significately faster than the uncached data that I started with.

### Acknowledgements
I used the following resources to help complete this project:

* AskBCS Learning Assistants
* GitHub
* UCB Coding Bootcamp GitLab
* ChatGPT
* Bootcamp Tutor David Chao
* W3 Schools
