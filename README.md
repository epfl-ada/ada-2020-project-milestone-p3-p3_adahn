### Title : Does the officer's race have an effect on racial disparities in police stops ? 

### Abstract :
  As the paper looked at racial disparities in police stops across the United States, we wanted to keep exploring the possible racial disparities in policing. In particular, we would like to investigate whether the race of the officer has an effect on racial disparities in police stops. First, we will assess potential bias in stop decisions by applying the 'veil of darkness' test. #JAMES JE SUIS PAS SUR EXACTEMENT DE LA QUESTION AUXQUEL TU REPOND#. Next, for each officer race we will look at the racial makeup of the drivers they stopped and compare it to the racial makeup of the county where the stops were made. If there are no disparities in policing the proportion of white drivers stopped in a county by a black officer should match the proportion of whites living in that county for example. Finally, we look at the rate at which an officer from a given race searches drivers with the same race as him versus drivers of a different race. However as possible disparities in search rates are not necessarily the product of discrimation as highlighted by the paper, we will also investigate the potential bias in the post-stop decision to search drivers for contraband. This will be done using outcome analysis, particularly by using the hit rates as defined in the paper. The data that we will use for our different analyses will be the datasets on policing made available by the Stanford Open Policing Project as well as the US census data.

### Research questions : 
1) Does the potential biais in search decision vary accross the different officer races ?
2) Is there a difference in the decision to stop a driver of a given race based on its sex ?
3) Is the difference in stop rates for each race due to a police bias or a different distribution of that race in the population ?
4) Does the political leaning of a state or city have an effect on race disparities in police stops ?

### Proposed datasets : 
1) Stanford Open Policing Project (paper based dataset) : https://openpolicing.stanford.edu/data/ 
2) US census data : https://www.census.gov/data.html

# A REFAIRE #
### Methods :
First we will get all the necessary datasets and do the data wrangling on them. We will use data from as many cities / states as there are on the Stanford Open Policing Project, considering they have the fields we are interested in (such as the officers race for example).

Then we would get a dataset from the US census data containing the race distributions in the cities / states where we have policing data on (from the Stanford Open Policing Project). This can be done using queries with the census data API. We would proceed similarly to optain the polical leaning of a state / city but with the Wikipedia API this time. We would infer the political leaning of the state / city by looking at how many congressmen they elected to congress from each party. However, we will consider only states where there is a wide enough difference in the number of congress members from each party, that is we exclude so called "swing states". For exemple, if a state has 6 Democratic and 5 Republican congressmen then we will not consider it leaning Democrat because the democrats represent only 54% of the congress seats for that states. We will use 60% as a first threshold.

To answer question 1), we will look at the stops officers made on drivers of the same race as them and stops made on drivers of a different race. We would make some plots to get some intuitions of the trends as well as to show our findings. Moreover, statistical tests such as t-tests would need to be performed to see if the difference (if there is any) in search / stops rate is statisticaly significant. If we have enough time we could go further and actually look at the differences between officer races, for example look at if white officers are more likely to stop black drivers than black officers are of stopping black drivers. We need to look at stops performed durng the day only since it's when the race of the driver is visible to the officer.

For question 2), we will have to separate the data based on the driver's sex and also taking only day stops. We could then see whether the race bias is still present on both sex and see whether the difference is significant with for example confidence intervals.

To answer question 3), we will look at the racial distribution of the population in a given state and compare it to the distribution of stops for that race. For example, if hispanics represent 30% of the population in a state, do they represent 30% of the drivers stopped in that state ? Any difference would not inherently mean that the cops are racist but would should that there are racial disparities in policing. Again, statistical tests would need to be performed to see if the difference (if there is one) is statistically different. We need to look at stops performed durng the day only since it's when the race of the driver is visible to the officer.

When comparing the stop rates of a Democrates and Republican states to anwser question 4), we will have to take into account the race percentage of the state. Indeed, a conservative state may have less black, hence this can give a false impression of lower search rate for black people in Republican States. We might train a regression model with significant states or counties, and observe if a dominant political party may influence the disparities. 

### Proposed timeline :

As we will have around 3 weeks to work on this extension of paper, by the end of the first week we must have collected all the necessary datasets and performed data wrangling on them. Each team member should have ideally started working on his assigned question by the end of the first week too. The second week will be used to finish answering the questions. The third week will be used to review the results, produce the data story and the video. 

### Organization within the team

Nicolas will answer question 1).
James answers question 2).
Dahn answers question 3).
We will all work on question 4) and we will do the data wrangling indivudually on our datasets since they are not the same. Moreover, Dahn will get the Census and Wikipedia datasets.
