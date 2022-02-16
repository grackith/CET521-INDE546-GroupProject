# CET521-INDE546-GroupProject
CET/INDE546 Inferential Statistics. Github for group project studying EV immersion in Washington State.

Proposal

A statistical assessment of the external and internal factors that influence personal electric vehicle adoption in the Seattle area or Washington state

A specific, testable, research question.

Driven by the issue of environmental damage caused by the emissions of fueled-vehicles, the electric vehicle (EV) has become increasingly popular in the public eyes, especially in the private automotive sector. In this project, our team is eager to predict the number of EV registrations in different zip codes based on a series of dependent factors. Studying those factors will help us make better fitted predictions. The question we will ask is: “What are the external and internal factors that influence personal EV adoption in the Seattle area or WA?”.

What data you will use, and how you will obtain the data?

The demographic data for the analysis will largely be obtained from the United States Census Bureau, which provides data for economic, social, housing, and several other categories. The data is delineated geographically by zip code or Census Block Group (CBG), which effectively represents a neighborhood-sized boundary. Geographic data, such as EV charging access and other environmental factors, will be pulled from public sources to make an assessment of other influences. EV vehicle registration will be tied to the Census data to identify trends in the data of EV user adoption in the Seattle area. The data is publicly available to download through Washington’s public database in various forms. The records have a geolocation in the form of a zip code tied to the vehicle registration data. This information will be used to associate the CBG demographic data and other geographic information with the EV registration data, which will require pulling zip code demographic data or summarizing CBG information at the zip code level.
	
What analytical methods you foresee using, and what you expect will be the independent and dependent variables?

The outcome variable of interest will be the count of registered electric vehicles per zip code dependent on a series of demographic and environmental predictors. The demographic data is population-specific and includes variables such as income, education, race, and employment rates. The environmental variables describe the setting of each zip code. For example, we thought it would be important to include the amount of charging stations available, proximity to highway access, or public transit usage. As we investigate available data, these variables are subject to change. 
As far as analytical methods used, we will first gauge how much data we can get. The census data can be quite extensive, which makes having a variable selection technique useful. If we run into a significant amount of predictors, LASSO may prove useful for selection, which helps identify variables highly correlated with the response. After variable selection is completed, cleaning and visualization of the variables will be conducted in R to understand any model transformations needed. We could use linear regression because our outcome is continuous, in which case the OLS assumptions would be checked with the Normal QQ plot, Residual plot, and VIF scores. We also believe most of our data could be attained temporally, so learning how to apply a Poisson regression could be interesting.
