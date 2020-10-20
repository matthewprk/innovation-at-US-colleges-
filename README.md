# innovation-at-US-colleges-and-diversity
How innovative are U.S. colleges and how do parent incomes and ethnicities contribute to innovation? 
## Background
Explored how U.S. colleges are clustered in terms of 1) innovation (inventors and patents) 2) diversity (ethnicities and parent incomes). [The U.S. boasts more innovative colleges than any other nation (46/100 in 2019)](https://www.forbes.com/sites/dereknewton/2019/10/28/american-universities-still-lead-the-world-in-innovation-impact/#13e946986c98). Generally, it is agreed that innovation is important to make progress in global commerce, business, and research. However, with respect to discussions about a college's impact on social mobility, are the most innovative colleges the ones that are also the most diverse? 
![alt text](https://github.com/matthewprk/innovation-at-US-colleges-/blob/main/Most%20Innovative%20Colleges%202019.png)

[The odds of picking any two students from a four-year U.S. college and them being from different racial or ethnic backgrounds is 69.6%](https://www.usatoday.com/story/money/2020/02/13/these-colleges-have-the-most-diverse-student-bodies/41152233/). While this may show that U.S. colleges are diverse, it doesn't show how U.S. colleges can be grouped in terms of innovation and diversity. Thus, for how innovative U.S. colleges are I chose to examine 1) inventors (the % of students who are inventors) and 2) total patents (the total # of patents granted to students). For diversity, I chose to examine 3) pct Asian 4) pct Black 35 pct Hispanic 6) pct alien (non-resident) 7) pct pq1 (% of students whose parents are in the bottom income quintile) and 8) pct pq5 (% of students whose parents are in the top income quintile). 

The goal is to understand how U.S. colleges can be grouped in terms of innovaiton and diversity. Ensuring that innovative colleges are accessible to a diverse group of students is important. If the more diverse colleges are the most innovative, then that indicates one area where less diverse colleges can improve to promote innovation.
 
## Business Question
How are U.S. colleges grouped based on metrics relating to innovation and social mobility (ethnicities, parent incomes)?

## Data Sources
- [Opportunity Insights](https://opportunityinsights.org/data/?geographic_level=100&topic=105&paper_id=0#resource-listing) - U.S. college data on innovation metrics and parent income quintiles
  - [Innovation Rates by College](https://github.com/matthewprk/innovation-at-US-colleges-/blob/main/Innovation%20Rates%20by%20College.csv)
- [Equality of Opportunity](http://www.equality-of-opportunity.org/data/college/Codebook%20MRC%20Table%2010.pdf) - U.S. college data on students' parent income quintiles
  - [Parent Income Quintiles](https://github.com/matthewprk/innovation-at-US-colleges-/blob/main/equalityofopportunity.xlsx)

## Data Analysis
The data question that the analysis will answer:
- How are U.S. colleges clustered in terms of: inventors, patents, pct Asian, pct Blacks, pct Hispanic, pct alient, pct pq1, and pct pq5?
  - How many clusters? What characteristics define each cluster? How many colleges are in each cluster?

The data analysis conducted:
- [Initial regression table shows that job density and job growth do not explain employment rate (p>0.05)](https://github.com/matthewprk/baltimore-city-employment-rate-2015/commit/ae82633f7204e4845eb398dc863d423f6100d682)
- Revised regression table shows that commute time <15min, poverty rate, and median HH income can be predictors of employment rate (p<0.05)
  - The equation used to predict employment rate is: Employment Rate = - 0.1278(traveltime15_2016) - 0.0680(poverty rate) + 2.0810E-06(median HH Income) + 0.6897
  - [Rsquared = 0.37 -> 37% of the variation can be explained by the inputs -> still need to identify more significant inputs](https://github.com/matthewprk/baltimore-city-employment-rate-2015/blob/master/baltimore_working_rP_gP_pall.xls)
- Linear Regession for Employment Rate and Poverty Rate Visualization
  - Rsquared = 0.2294 -> 23% of the observed variation is explained by poverty rate -> need to consider other variables in prediction
  - Slope = -0.1913 -> for every 1 unit increase in poverty rate, employment rate decreases by -0.1913
![alt text](https://github.com/matthewprk/baltimore-city-employment-rate-2015/blob/master/linreg_povertyrate.png)
## Summary and Next Steps
It was determined that job density and job growth are not helpful predictors for employment rate in Baltimore. Although commute time <15min, poverty rate, and median HH income can be used to predict employment rate, they are not the strongest predictors given 63% of the variation is explained by other factors. To determine factors that would better predict employment rate in Baltimore, it would he helpful to look at education status, regional industries/roles, and skillsets. These would hopefully explain any structural disconnects between employers and employees/job seekers. 
