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

ADD LINK TO CLUSTER

The data analysis conducted on 421 U.S. colleges using Solver:
- [Cluster Analysis]() - shows three clusters (diminishing returns as additional clusters added): 
- ![alt_text](https://github.com/matthewprk/innovation-at-US-colleges-/blob/main/cluster%20analysis%20table1.png)
  - Cluster 1 - Most innovative schools with higher Asian, non-resident, and top parent income quintile populations. 
  - Cluster 2 - Slightly below average innovative schools with low Hispanic and bottom parent income quintile populations.
  - Cluster 3 - Lease innovative schools with high Black, Hispanic, and top parent income quintile populations and low top parent income quintile and non-resident populations.
- ![alt_text](https://github.com/matthewprk/innovation-at-US-colleges-/blob/main/cluster%20count.png)
  - Most colleges fall into the middle-of-the-pack Cluster 2. Almost an equal number of colleges in Clusters 1 and 3. This shows that ~75% of U.S. colleges are somewhat or not  very innovative. 
  
- [Cluster Visualization] - shows the clusters based on pct pq5 and inventors. The anchors for these variables (one for innovation and one for diversity) had the highest stdev for their z-scores 
  - ![alt text](https://github.com/matthewprk/innovation-at-US-colleges-/blob/main/clusters%20pq5%20and%20inventors.png)
  
## Summary and Next Steps
It was determined that job density and job growth are not helpful predictors for employment rate in Baltimore. Although commute time <15min, poverty rate, and median HH income can be used to predict employment rate, they are not the strongest predictors given 63% of the variation is explained by other factors. To determine factors that would better predict employment rate in Baltimore, it would he helpful to look at education status, regional industries/roles, and skillsets. These would hopefully explain any structural disconnects between employers and employees/job seekers. 
