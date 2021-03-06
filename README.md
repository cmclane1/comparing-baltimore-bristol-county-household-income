# Analyzing outcomes of Baltimore, MD vs Bristol County, RI
## Background
Baltimore, Maryland is the 30th largest American city with an estimate population of 593,490 in 2019. It is a transportation hub with a port that quickly connects to Chesapeake Bay and the Baltimore Ohio Railroad, the oldest in the US. African Americans make up 63.7% of the city's population while only 29.6% are white, as of 2010. 

Bristol County Rhode Island is the third smallest county in the US by area and has a population of just 49,875 in 2010. It is made up of three towns, Bristol, Warren, and Barrington. Bristol is known for its harbor that sits between Mount Hope Bay and Narragansett Bay, with sailing being an important pastime. The county is 95.7% white with the largest ancestry groups being Portuguese (24.8%), Irish (22.2%), and Italian (21.0%). Bristol County, RI is one of only two counties with a plurality of Portuguese people, the other being the adjacent Bristol County, MA. Lastly Bristol County, RI is the 10th most Catholic county in the US with 75.14% identifying as such, only 10.95% in Baltimore.
  
I am from Warren, Rhode Island and I am interested in seeing how outcome compared to Baltimore City. There are too few data points to just use Warren, while I considered using the nearby cities of Providence, RI, or Fall River, MA, I wanted to get the comparison between the coastal town I grew up in with the city where I now live. I decided to use income as my main metric because there are a lot of data, and it is a good indicator of life standards.
  
## Business Question
How does household income differ between Americans raised by low-income parents in Baltimore City Maryland, vs Bristol County Rhode Island?

## Analysis
It differs by quite a lot. The average income of the Baltimore is $23,000 (2nd percentile), while the average in Bristol county is $38,000 (76th percentile), 55% higher. The histogram below shows the distribution of the different income tracts. This is a surprising and significant difference, I decided to check some other metrics for other indicators and education was quite different. Looking at the same groups Baltimore has a high school graduation rate of 73% (12th percentile), and college graduation rate of 12% (19th percentile). While Bristol has a high school graduation rate of 88% (92nd percentile), and college graduation rate of 33% (96th percentile). Both metrics clearly show better outcomes for Bristol but it is interesting that both rank higher in education than in income. 

Baltimore needs to examine why the education rates are so low and try and improve them, especially for low-income students. While Bristol is doing well, it needs to focus on translating its high rate of education into a similarly high income. These places are not similar in demographics or size. They require very different solutions to improve their outcomes and Bristol is far further along than Baltimore is in having good outcomes. An interesting theory I have is that Bristol has a much higher rate of Catholics, and growing up I went to one of many Catholic elementary and high schools, it should be investegated what effect religion has on the high school graduation rate.

![alt text](https://github.com/cmclane1/comparing-baltimore-bristol-county-household-income/blob/main/Bristol-Baltimore.png)

## Step by Step Walkthrough
  For the analysis I downloaded the data from opportunity atlas and copied it to a new worksheet. Then I created tables for both sets of data and used filters to remove any extra data that was not for Baltimore City or Bristol County. Then I found the maximum and minimum incomes of Baltimore using MAX and MIN functions so I could gauge the range of values. Then I divided it into ten buckets for use in the histogram, rounding the values to a range of 4,500. I then used the frequency function to see how many tracts fit into each bucket. Baltimore has many more tracts than Bristol, so I changed each histogram count from a raw count of tracts to a percent of the total for that county. This allowed me to graph them both on the same histogram side by side and get a good-looking representation of both counties outcome distributions. Other data such as the education numbers were taken directly from opportunity atlas and I did not download a CSV because it would only be one or two values. 
  
## Links to Sources
[Analysis](https://github.com/cmclane1/comparing-baltimore-bristol-county-household-income/blob/main/Baltimor-Bristol-Analysis.xlsx)

[Data](https://github.com/cmclane1/comparing-baltimore-bristol-county-household-income/blob/main/Baltimore-Bristol-Data.xlsx)

[Opportunity Atlas](https://www.opportunityatlas.org/)

[Baltimore Wikipedia](https://en.wikipedia.org/wiki/Baltimore)

[Bristol County Wikipedia](https://en.wikipedia.org/wiki/Bristol_County,_Rhode_Island)

[Catholic Counties of the US](https://www.thearda.com/ql2010/QL_C_2010_1_26c.asp)
