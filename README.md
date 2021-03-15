# Education vs. Economic Opportunity

Group project using python/Jupyter notebook to uncover potential relationships between educational attainment and income opportunity

* Research questions
* Digging into the data
  * In search of….
  * Regional Economic Analysis profiles
  * Educational Attainment in CA
* Does education translate to higher income?
  * Data cleaning/analysis
  * Education vs. Income analysis
  * Percent of Population with a Bachelor’s degree
* How does gender affect the relationship between income and education?
  * Data cleaning/analysis
  * Education vs. Income weighted for gender
  * Statistical significance
* Median wages versus job openings
  * Highest earning occupations by education level
* GitHub learnings
* Conclusions

---------------------------------------------------------------------------------------------------------------------


## What is the real value of pursuing an education in California?
Intuitively, we recognize the power education can have in shaping a life for the better. 

Higher education tends to be tied to a perceived economic gain in some shape or form. 

*But education is not cheap.*

According to insights from Deloitte, "the price tag for a traditional residential four-year degree program averages just over 
$30,000 per year," and that "the College Board estimates that annual tuition costs will rise to a staggering $62,000 per year 
by 2025." 

Again, education is not cheap. One student may be assumed to pursue a university degree based on their financial upbringing, but another may be the first in their family to go to college. 

*So, what is a degree really worth in California?*

The **questions** we started off with were:
* How does one’s education influence their potential for income?
* Which industry sectors are the most lucrative? 
* Where do we see the most job openings for each level of education received?
* Do men and women see similar, if any, economic gains upon completion of some education level?
---------------------------------------------------------------------------------------------------------------------

## Digging into the Data
We set out to look for datasets with information which may correlate with the level of education attained (high school, college, masters, etc.), such as projected wage/salary estimates, relevant occupations, and some demographic data to tell us more about those who make up the population in the higher education landscape. 

We looked to the Open Data Portal on our state’s public website (data.ca.gov), and settled upon the following datasets for our analysis:
* *Regional Economic Analysis Profiles 
  * Provides data for industry clusters* & related future job opportunities to help California’s workforce development system understand future employment opportunities.
  * **Link:** https://data.ca.gov/dataset/regional-economic-analysis-profiles/resource/601ba4d4-6770-4446-894b-193e1f608bdd
* *Educational Attainment
  * Contains information collected in California from 2008 to 2014 with the percent of population age 25 and up with a four-year college degree or higher, along with their income, education level, and gender
  * **Link:** https://data.ca.gov/dataset/educational-attainment


In order to investigate patterns in CA education trajectories, we examined relationships in the context of:
* Educational attainment versus income levels and employment prospects
* Potential gender disparities across education and income levels
* How these trends may have evolved over time


---------------------------------------------------------------------------------------------------------------------

### Does Education Translate to Higher Income?
*Exploring whether or not income levels are related to having a college degree.*

**Cleaning the data**
* *Educational attainment
  * Created a visual to compare the population of education level and income.  Cleaned the data to create a multi bar graph.
  * Cleaned data to create a line graph that shows trends in education level from 2008 to 2014.
  * To create graphs used filtering with loc, looping to gather data, matplotlib for graphing.

**Insights/Observations**
* The proportion of Bachelor’s degrees in each income level has not changed much from 2008 to 2014
* Over 75% of people making $75,000 and over have a Bachelor's degree.
* Low-income populations tend to have a lower percentage of Californians with a Bachelor’s degree


### How does gender affect the relationship between income and education?
*Examining whether or not gender has an impact on earning potential through statistical analysis.*

* **Null Hypothesis:**  Income levels are independent of gender for equivalent educational levels
* **Hypothesis:**  There is a linear relationship between gender and income for equivalent educational levels

**Cleaning the data**
* *Educational attainment
  * Split the data for gender
  * Used matplotlib to produce bar charts
  * Did a Chi-test statistical analysis on the gender  data to check if income  is independent of gender.
  * Weighted the data for gender separately for each income level category


**Insights/Observations**
* There is an imbalance in the number of males and females in each education level.
* Weighted the numbers for each education level  separately.
* There are many more men in the 'no high school' and 'high school' categories
* More women in the 'some college' and 'college' categories


## How does the job market vary across different education levels?
*Exploring job openings for different education levels and their associated wages/income.*

**Insights/Observations**
* Bachelor’s degree median income is higher than masters
* Bachelors degree has the 3rd most job openings available
  * Possibly reflects the diversity of jobs available to bachelor’s graduates  
  * Considered an entry-level education for most higher-paying jobs
* Master’s degrees might be in more niche industries (i.e. social services), which aren’t as high paying or plentiful
* Less than high school has, by far, the most job openings
  * This could imply that even as we move toward a more technology-oriented society, the need for less technical work is still in high demand 
  * Also demonstrated by the high volume of high school job openings

---------------------------------------------------------------------------------------------------------------------



## So, is it worth it?

Your chances of earning >$75k are much better if you attain a Bachelor’s degree. Sounds enticing, but interestingly, the proportion of the population getting a Bachelor’s degree has not changed much from 2008 to 2014. 


There tends to be much greater earning potential for those who pursue higher education, yet there are more jobs available for those without a college degree.


This may suggest a disparity and limited mobility in terms of who can afford to make such a large investment in their education.

***

On average, we see that women tend to earn less than men, and there are more women who earn “no income” than there are men reporting the same. 


Slightly more women pursue a higher education than men. Yet the income levels for each gender suggest a disparity in the job market.


This suggests that women face additional barriers to achieving economic equity with their male counterparts.


