# ADSPP
## This is Groups' 5 Read-Me file for the Applied Data Science for Public Policy 2018 Spring Semester final paper.

## Impact of noise complaints on school test scores
An analysis using 311 complaints, New York State Mathematics and 
English Language Arts (ELA) Test Score (2013-2015)


In this paper we try to explore possible correlations between the density of 311 Noise Complaints and school performance. In order to do this we work our way from all the 311 complaints registered in the New York City (NYC) open data portal to just the Noise related complaints between 2013 and 2015 during weekdays. The selection of the period 2013-2015 relates to the fact that these are the years for which we have the aggregated results for schools in NYC in both Math and English tests. Finally we also work with LODES data in order to assign sicioeconomic characteristics to the surroundings of the school, because of privacy issues we cannot know were the choldren that took the test lived, so we must assume that the only environment that they are exposed to is that of the surroundings of the school, leading us to use census tracts as our geographic units.

In order to develop the model we count the number of 311 noise complaints in each of them and divide by the area, leaving us with a "noise complaint density" value by census tract. To each census tract we also assign the income characteristics provided by LODES. Finally to each school we assign the characteristics of the census tract were it is located. Finally we run 6 linear regression models (2 subjects times 3 years) that correlate the mean test score with the noise complaint density by census tract and the percentage of people inside a census tract that make more than 3.333 USD. 

The results of the model show that initially it is very hard to prove any correlation between the noise complaint density in a census tract and the performance of schools located in it, there might be many reasons for this, first because we cannot account for the context of the children when they are out of school, secondly because we might be ommiting relevant variables, due to preventing multicolinearity without losing the interpretability of the variable of Noise Complaint Density. We believe the model can be improved, or even have a different approach, nonetheless with our results it is impossible to say that Noise Complaints can help explain variations in the test results of schools in NYC. 
