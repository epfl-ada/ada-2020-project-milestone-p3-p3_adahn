### Title : Is there an hidden feature that can influence police stops rate ? 

### Abstract :
As the paper looked at racial disparities in police stops across the United States and the effect of marijuana legalization on stop decisions, we wanted to keep exploring the possible racial disparities in policing. First we would like to investigate whether the race of the officer has an effect in the stop decision of a driver. Similarly, we want to look if the driver's sex impacts the decision of the police officer to stop the driver or not. To do so we will simply use the dataset provided by the Stanford Open Policing Project which the paper is based on. Then, we want to investigate further in the direction of the paper's focus which is the analysis of racial disparities in police stops. We would like to see if the percentage of drivers stopped from a given race correspond to the percentage of that race in the local population or not suggesting the presence or absence of a racial bias. For example, if Hispanics correspond to a given percentage of the police stops in a city we would like to compare if Hispanics correspond to that percentage of the population in the city. Finally, we want to look if the political leaning of the city or state plays a role in racial disparities for police stops. Effectively we want to compare states or cities (depending on the available data) that are either majoritarly Democratic or Republican and see if there are statistically significant differences in the stop data.

### Research questions : 
Does the officer's race have an effect on racial diparities in police stops ?
Is there a difference in the decision to stop a driver of a given race based on its sex ?
Is the difference in stop rates for each race due to a police bias or a different distribution of that race in the population ?
Does the political leaning of a state or city have an effect on race disparities in police stops ?

### Proposed datasets : 
1) Stanford Open Policing Project (paper based dataset) : https://openpolicing.stanford.edu/data/ 
2) Wikipedia API for race percentages of counties and politics majorites in states
3) US census data : https://www.census.gov/data.html

### Methods :
We will first extract from the whole dataset driver's race and officer's race to analyze if it has an effect on racial disparities. Then we will do the same but this time with subject's sex. Then we would have to get a dataset from www.cencus.gov with the race percentages in counties that have data for police stops. Those data are available. We would then normalize race stops to this percentages and see if there is still an effect of racial disparity or if the effect is even bigger. We will compare the ratio of blacks and whites stopped by the police.
Finally, we will get a dataset from Wikipedia but this time with the majority of politics of different states. We will not use Swing States but only States majoritary Democrates or Republicans. We might also go to the County level if we observe that some States have a significant politics difference between it's Counties. We will thus see if there is a correlation between state's politic and racial disparity in police stops.
When comparing the stop rates of a Democrates and Republican states, we will have to take into account the race percentage of the state. In deed, a conservative state may have less black, hence this can give a false impression of lower search rate for black people in Republican States. We might train a regression model with significant states or counties, and observe if a dominant political party may influence the disparities. 

(FAUT DEVELOPPER PLUS LES COMPARAISONS/TESTS QU'ON VA FAIRE JE PENSE - Et relire!!)

### Proposed timeline :
As we will have around 3 weeks to work on this extension of the study, we will start by answering the two first questions during the first week, as well as collecting the Wikipedia and Census dataset. The second week we will analyze those datatsets to answer the two final questions. The third week will be use to review the results and write down the possible outcomes of the data analysis. 

### Organization within the team

(A VOIR ENTRE NOUS)

### Questions for TAs (optional)

