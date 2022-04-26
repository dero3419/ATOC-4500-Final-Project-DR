# ATOC-4500-Final-Project-DR
CU Boulder ATOC 4500 Spring 2022 Class Final Project by Devon Romero 
For my project I wanted to test the seasonal variability in New Mexico the same way we did in our Colorado datasets. I chose New Mexico based on that’s where I was born and raised and based on lived experience, the northern part of new Mexico has a very similar climate to Colorado, or at least boulder where I chose to study and now live. I wanted to do my analysis with santa fe, my home town but unfortunately I was not able to locate any weather data. I has similar experiences with most locations in new Mexico and decided to switch to southern new Mexico and compare it to Colorado. To do this, I will be using machine learning to identify patterns and assess the significance of each variable. The data is unsupervised which means I will be applying the K-Means clustering analysis.

I got my data from NCAR Mesa Laboratory in Boulder, Colorado and from NMSU ZiaMet Weather station in La Mesa, New Mexico. My datasets are called 2_nm_data_2018-2021.csv and hw4_mesa_data_2016-2021_withmissing.csv. Data munging was done by myself as there was missing data in both datasets and has since been corrected. I also had to reduce the amount of years in dataset 2, the boulder dataset. 

The hypothesis leading this project is that Colorado will have more seasonal variability than Southern New Mexico. I chose Boulder and La Mesa due to their location and their altitude differences. I hope to learn the similarities and differences between both climates, and to see which variables influence either location more than the other. I expect temperature and snow to be the biggest determiner in Colorado whereas snow in southern New Mexico is not common. I expect southern New Mexico to work best in four clusters whereas Colorado will be three clusters. I do not expect wind to be a big determiner as both locations experience winds frequently. 

I ran the code with less clusters in other notebooks but you will see those clusters in this notebook for comparison. The code is the same, it is just less clusters and without the rain variable. I chose to remove the rain variable when adjusting the cluster amount because the rain was just all over the place and it wasn’t the biggest influencer in any season in either location.

Dataset 1 w/4 clusters
When we look at the clusters by day of the year we can see the different seasons with a little bit of overlap. Cluster 2 is a very small cluster with more variability than the other 3. Summer and spring are a bit harder to define but overall this plot furthers my prediction that there is not as much variability in southern new Mexico that clustering works well. 

In my plots I used mean air temperature in degrees Celsius to compare with the other four variables. All of the variables seemed to produce clear clusters with the exception of relative humidity and wind direction which both had one cluster all over the place. 


Dataset 2 w/4 clusters
We see a similar scenario in the clusters by day of the year plot as we did with the new Mexico data. Cluster 2 appears to be less defined with less points. But we can still make out the seasons. 

When looking at the individual variable plots, I used dry temperature degrees Celsius to compare with the other 4 variables, following the process I did with the new Mexico data. All of the variables had horrible clustering. None of the clusters were clearly defined. When we did this analysis in the homework 4, the clusters were well defined. But the data was munged and two years were taken out and the loss of those two years of data is resulting in our poor plots. With this we can conclude that just four years of data isn’t enough data to make a conclusion about our hypothesis. There is too much variability in Colorado that more data is needed to get better, clear results.

Dataset w/3 clusters and no rain variable
Neither dataset worked super well with four clusters. So I adjusted the cluster amount to 3 and also decided to take out the rain variable as neither location is heavily impacted by rain nor receives large notable amounts. 

In the New Mexico dataset, the plot of the scaled data was so much better than it was with the rain variable. The clusters by the day of the year plot also looked a lot cleaner. You could easily see three seasons and the variability when the season changes. As for individual plots, the clusters were well defined with relative humidity still needing more definition. It appeared that fall seemed to be the transition period and was the season that did not have a defined season. 

In the boulder dataset, we also can see three defined seasons in the clustering by days of the year plot. For the individual variables, three clusters work better than 4, but were still not defined enough to be clear seasons or to indicate which are more influential than others. 

Dataset w/2 clusters and no rain 
It appeared that taking rain out as a variable helped with clustering. Three clusters worked really well for new Mexico but not so much for Colorado so I wanted to go another step in my analysis and try 2 clusters with no rain. 

The new Mexico dataset with 2 clusters for the day of the year I found to be really odd to say the least. You could still see the difference in winter and summer but I was surprised to see the transition period from season to season was longer than I expected which I think shows that new Mexico works well with three clusters but not necessarily two. But for the individual variable plots, 2 clusters worked really well with the exception of relative humidity not as well defined as the others. In the histogram you are able to see the clustering of summer and spring and fall and winter together really well. 

For the boulder dataset, the clustering by days of the year plot looks pretty good. Pretty similar to the new Mexico plot where you can see winter and summer and those transition periods. But, I was shocked what I saw when looking at the individual variable plots. The clusters were all over the place and not well defined at all. Not a single variable had two defined clusters. The seasonal variability in Colorado is kind of crazy but also goes to show that we definitely need more data to see more defined clusters. 
![image](https://user-images.githubusercontent.com/101827981/165368844-27bc4845-cd3c-4162-af3e-c01e883de841.png)
