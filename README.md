# MechaCar_Statistical_Analysis

AutosRUs is having production issues with its newest prototype, the MechaCar. The data analytics team has been given the production data to analyze and determine 
which variables are impacting the manufacturing team's progress.

## Linear Regression to Predict MPG
Multiple linear regression analysis was performed to identify which variables in the dataset predict the mpg of the MechaCar prototypes.

The three variables and their cooresponding cooficients below provided a non-random amount of variance to the mpg values in the dataset:
- Vehicle length (5.08e-08)
- Vehicle weight (2.60e-12)
- Ground clearance (5.21e-08)

![Multiple regression](MultipleRegression.gif)

The slope of the linear model is not considered to be zero, as a slope of zero would mean that the mpg of the MechaCar prototypes would be determined by random chance. As noted above, there are three variables that provided a non-random amount of variance to the mpg values.

Although this linear model identifies variables that provided a non-random amount of variance, the r-squared value is 0.7149, which leaves approximately 29% of the variability of mpg unexplained. To effectively predict the mgp of MechaCar prototypes, additional modeling should be completed.

## Summary Statistics on Suspension Coils
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.

The current manufacturing data shows that when looking at all three lots combined, the variance is 62.29356 and the specificatinon appears to be met. However, looking at the lots individually provides much needed insite. Lots 1 and 2 have vary low variances, but Lot 3 is well above the 100 pound per square inch threshold. The data confirms that Lot 3 is not meeting the design specification.

![total_summary](total_summary.gif)

![lot_summary](lot_summary.gif)

## T-Tests on Suspension Coils
The t-tests performed on the combined lots, Lot 1, and Lot 2 all produced p-values greater than .05, signifying that the means are statistically similar to the population mean of 1,500 pounds per square inch.

![t_test](t_test.gif)

![lot1_t_test](lot1_t_test.gif)

![lot12_t_test](lot2_t_test.gif)

Lot 3's t-test produced a p-value of 0.04168, signifying that the mean for this lot is statistically different to the population mean.

![lot3_t_test](lot3_t_test.gif)
