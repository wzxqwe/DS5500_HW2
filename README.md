# DS5500_HW2
please find all plots and codes for HW2 at https://github.com/wzxqwe/DS5500_HW2/blob/master/5500%20HW2.md


Problem 4
As there are not too many features and data points, we can use a simple linear regression to fit the model. We can first fit without any transformation on Life Expectancy ~ GDP + Time; From the residual plot (in ipynb) we can see there is a need for transformation of gdp data, so we then fit model on Life ~ log(GDP) + Time. Then result seems better:

 For this linear model we get a mse of 29 and R score of 0.703.
Regarding time’s effect, we see the coefficient of time is 0.18 and significant, which implies time has a positive effect on life expectancy.



Problem 5

For problem 5, we also use a simple linear regression to fit the model. We can first fit without any transformation on Children Mortality ~ GDP + Time; 
From the residual plot we clearly see it’s not randomly distributed and we need transformation of data, so we then fit model on Mortality ~ log(GDP) + Time. Then result is better. We see the residual is still not randomly distributed and there is some heteroscedasticity in the data which might need some further transform or add features. The mse is 108 and Adj Rscore is 0.705. However, to keep model simple and focus on relation between mortality and GDP we will use this model. Regarding time, now time has a negative coefficient of -0.48, which suggest time has a negative effect on children mortality.
