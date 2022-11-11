# MechaCar_Statistical_Analysis

## Overview

The whole purpose of this project was to learn how to use R to analyze data and creat visualizations that are helpfull to analyze the car industry. Through this project I learned how to use tidyverse to manipulate and clean data and ggplot2 which makes visualizations that are easy to understand. In this project I used different statistical methods in order to creat relationships between variables in a dataset in order to identify possible relations and make possible predictions. This statistical methods include Linear Regression, Summary Statistics and T-test. With this information I was able to find very intresting information which will be helpful for AutosRUs.

## Linear Regression to Predict MPG

Linear Regression helps us find relationships between two variables. In this case, this statistical method helped me answer important questions for AutosRUs. 

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

Acording to the results we had, there are some variables that are statistically significant and affect the MPG:

<img width="524" alt="Screen Shot 2022-11-10 at 18 19 02" src="https://user-images.githubusercontent.com/108498940/201233395-ab4e5a59-8703-4c18-9d41-8166a1d5de62.png">

This image shows the statistical summary of the variables and we found that the following variables have a significant relation to a vehicles mpg:
mpg: 0 < .05, statistically significant, non-random amount of variance
vehicle length: 0 < .05, statistically significant, non-random amount of variance
ground clearance: 0 > .05 statistically significant, non-random amount of variance

This information tells us that with a 95% level of confidence we can say that mpg, vehicle length and ground clerance have a direct impact on mpg. 

2. Is the slope of the linear model considered to be zero? Why or why not?

<img width="783" alt="Screen Shot 2022-11-10 at 18 18 34" src="https://user-images.githubusercontent.com/108498940/201233931-85ecf18f-f911-493c-b3e7-405a95f21ff2.png">

The linear regression formula for mpg is: 

mpg = -.01 + 6.267(vehicle length)+.001(vehicle weight)+.069(spoiler angle)+3.546(ground clearance)-3.411(AWD)

This means that the slope is not 0 because a slope exists acording to the formula. 

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

The R-squared was 0.7149 and the Adjusted R-squared was 0.6825 which indicates a high level of correlation. This means that our model predicts the mpg of MechaCar effectively but there are still other variables that affect mpg. 

## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

The variance of the total manufacturing lot is 62, which meets the design especifications of not exeeding 100. Even though the total manufacturing variance meets the requirement, lot 3 individualy has a variance of 170 which does not comply with the design requirements. 



## T-Tests on Suspension Coils



