# MechaCar_Statistical_Analysis

## Overview

The purpose of this analysis is to review the production data for insights that may help the manufacturing team. Using RStudio, we will perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes, collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots,and run t-tests to determine if the manufacturing lots are statistically different from the mean population.

## Linear Regression to Predict MPG

![image](https://github.com/awill1786/MechaCar_Statistical_Analysis/blob/main/Resources/Images/lr%20summary.png?raw=true)

1. According to our results the vehicle_length (2.60e-12), and ground_clearance (5.21e-08), give us a non-random amount of variance to the mpg values in the dataset. Because of this the vehicle length and ground clearance have a significant impact on mpg on the MechaCar prototype.

2. The slope of this linear model is not zero, due to the p-value (5.35e-11), being much smaller than the assumed signigicance level of 0.05%.

3. The linear model has a Multiple R-squared value of 0.7149, which means that approximately 71.49% of all mpg predictions are determined by this model. Which means this regression model does predict mpg of the MechaCar prototypes effectively.


## Summary Statistics on Suspension Coils
Total Summary table:
![image](https://github.com/awill1786/MechaCar_Statistical_Analysis/blob/main/Resources/Images/total_summary.png?raw=true)

lot_summary table:
![image](https://github.com/awill1786/MechaCar_Statistical_Analysis/blob/main/Resources/Images/lot_summary.png?raw=true)

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. According to the tables, the current manufacturing data meets the design speciafication for all manufacturing lots in total, for Lot 1, and Lot 2. This due to the variances being around 62 for the total, around 1 for Lot 1, and around 7 for Lot 2. Lot 3 however does not meet the design specification due to the variance being around 170.


## T-Tests on Suspension Coils

In this analysis we perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch.

![image](https://github.com/awill1786/MechaCar_Statistical_Analysis/blob/main/Resources/Images/total%20PSI.png?raw=true)

Because the calculated p-value of 0.06028 is higher than 0.05 for all manufacturing lots, it is not right to reject the null hypothesis. The mean of all three lots is statistically similar to the presumed population mean of 1500.

![image](https://github.com/awill1786/MechaCar_Statistical_Analysis/blob/main/Resources/Images/each%20PSI.png?raw=true)

For Lot 1, due to the p-value being 1, we can accept the null hypothesis that there is no statistical difference between the sample mean and the population mean.
For Lot 2, with a p-value of 0.61 and a sample mean of 1,500.02, we cannot reject the null hypothesis, as the sample mean and the population mean are similar.
For Lot 3, with a p-value of 0.04 and a sample mean of 1496.14, We can reject the null hypothesis, because the sample mean and population mean are not similar.

## Study Design: MechaCar vs Competition

Consumer would be interested in several different metrics such as cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.

A Null hypothesis as there is no difference between the metrics of MechaCar vs competition. Alternate hypothesis as there is a difference between the metrics of MechaCar vs competition.

To test the hypothesis we should use T-test as if the p-value is less than the significance level, then the null hypothesis is rejected.

To run the statistical test needs to use data as cost, city or highway fuel efficiency, horse power, maintenance cost, safety rating.
