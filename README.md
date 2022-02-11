# MechaCar_Statistical_Analysis

A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

## Background :





## Purpose :

In this challenge, I will help Jeremy and the data analytics team do the following:

 - Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
 - Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
 - Run t-tests to determine if the manufacturing lots are statistically different from the mean population
 - Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. 
 
 Thus, this project consists of three technical analysis deliverables and a proposal for further statistical study. The project is divided into the following parts:

 - Deliverable 1: Linear Regression to Predict MPG
 - Deliverable 2: Summary Statistics on Suspension Coils
 - Deliverable 3: T-Test on Suspension Coils
 - Deliverable 4: Design a Study Comparing the MechaCar to the Competition

## Results :

### 1. Deliverable 1 - Linear Regression to Predict MPG - 

The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using the knowledge of R, I  designed a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file. This is followed by  a short interpretation of the multiple linear regression results.


#### Summary of Linear Regression to Predict MPG -

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
2. Is the slope of the linear model considered to be zero? Why or why not?
3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?



### 2. Deliverable 2: Summary Statistics on Suspension Coils - 

The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using knowledge of R, I have created a summary statistics table to show:

 - The suspension coil’s PSI continuous variable across all manufacturing lots
 - The following PSI metrics for each lot: mean, median, variance, and standard deviation.

#### Summary Statistics on Suspension Coils - 
A short summary using screenshots from the total_summary and lot_summary dataframes, and addressing the following question: 

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?


### 3. Deliverable 3: T-Test on Suspension Coils -

Here we will perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch. An RScript is written for t-test that compares all manufacturing lots against mean PSI of the population. This was done using the t.test() function to determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch. Secondly, An RScript is written for three t-tests using t.test()  function and its subset() argument to determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 pounds per square inch.

#### Summary of T-Test on Suspension Coils - 
Summarizing the interpretation and findings for the t-test results below -


### 4. Deliverable 4: Design a Study Comparing the MechaCar to the Competition -



#### Summary of T-Test on Suspension Coils - 
## Summary :

## Resources : 

Datasets- 

