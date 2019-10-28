# DS5500_HW2
please find all plots and codes for HW2 at https://github.com/wzxqwe/DS5500_HW2/blob/master/5500%20HW2.md

Problem 2
For Manvita Markala's visualization.(Link). This visualization effectively show us the distribution of income across countries and also the trend of income’s growth by time. Mine is similar to this one, as we both used static line plot and denote different regions by color. I like the plot in which the author also make a visualization on countries level, which provide additional information, although it’s kind of hard to read those large number of lines in detail. Overall, I think the visualization is effective and easy to interpret.

Problem 3

For Nick Tyler’s visualization project. (Link here). This visualization is generated in R but is very similar to the one before and mine which are from python. We both use static line plots and the idea are pretty much the same. One thing to notice is Noah also add a bar plot to visualize distribution across region, which I think is a good idea as bar plot is easier to interpret as it has steady scale as measurement. The ordering of bars also provides an easy interpretation of the rank of incomes. Overall, I think the visualization is effective and easy to interpret.

Problem 4

As there are not too many features and data points, we can use a simple linear regression to fit the model. We can first fit without any transformation on Life Expectancy ~ GDP + Time; From the prediction plot and residual plot 
![alt text](https://github.com/wzxqwe/DS5500_HW2/blob/master/output_10_1.png)
![alt text](https://github.com/wzxqwe/DS5500_HW2/blob/master/output_11_1.png)

we can see there is a need for transformation of gdp data, so we then fit model on Life ~ log(GDP) + Time. Then result seems better:
![alt text](https://github.com/wzxqwe/DS5500_HW2/blob/master/output_12_1.png)
![alt text](https://github.com/wzxqwe/DS5500_HW2/blob/master/output_13_1.png)
For this linear model we get a mse of 29 and R score of 0.703.
Regarding time’s effect, we see the coefficient of time is 0.18 and significant, which implies time has a positive effect on life expectancy.



Problem 5

For problem 5, we also use a simple linear regression to fit the model. We can first fit without any transformation on Children Mortality ~ GDP + Time; 
From the model fitting plot and residual plot:
![alt text](https://github.com/wzxqwe/DS5500_HW2/blob/master/output_18_1.png)
![alt text](https://github.com/wzxqwe/DS5500_HW2/blob/master/output_19_1.png)

we clearly see it’s not randomly distributed and we need transformation of data, so we then fit model on Mortality ~ log(GDP) + Time. Then result is better. 
https://github.com/wzxqwe/DS5500_HW2/blob/master/output_25_1.png
https://github.com/wzxqwe/DS5500_HW2/blob/master/output_26_1.png

We see the residual is still not randomly distributed and there is some heteroscedasticity in the data which might need some further transform or add features. The mse is 108 and Adj Rscore is 0.705. However, to keep model simple and focus on relation between mortality and GDP we will use this model. Regarding time, now time has a negative coefficient of -0.48, which suggest time has a negative effect on children mortality.
