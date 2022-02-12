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


## Tools Used :

### 1. R - 
R is a versatile and extensible programming language with many benefits. One of the benefits of using an interpreted programming language such as R (or Python) is that the analysis scripts are written in plaintext. The versions of plaintext files are easy to control using tools such as Git, which means that R analysis scripts (or RScripts) are highly reproducible and easy to share with peers and collaborators. Another benefit to using R is that the R programming language was specifically designed for data analysis. This means that the process of loading in a dataset, visualizing the data, and performing statistical tests is straightforward and easy to interpret. In fact, many of the statistical tests in Python have been directly ported from R due to how well they were implemented. In addition to the native statistical functions, there are many other useful data transformation and modelling libraries, such as the tidyverse package, that simplify the process of ETL and visualizations.

### 2. RStudio Integrated Development Environment - 
Just as Jupyter Notebooks are an integrated development environment (IDE) used to help design and test Python scripts, RStudio is an IDE used to help design and test RScripts. RStudio provides users a graphical user interface (GUI) with multiple dynamic windows and perpetual access to their RScript and R console.

Similar to Jupyter Notebooks, RStudio enables users to test their analysis scripts line by line while allowing users to view different environment variables and outputs. This means that for each line of code written and executed, users can verify the results and troubleshoot any problems quickly and easily.
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

