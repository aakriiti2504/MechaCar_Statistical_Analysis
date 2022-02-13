# MechaCar_Statistical_Analysis

A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

## Background :

Jeremy has been working with AutosRUs industry for a long time. In his time he has seen a lot of cars come and go. The company is finally realizing that the decision making process could be moved into the 21st century. Jeremy with his strong external connections and exhaustive knowledge of the product has been chosen as the data primary analyst for the company's data analytics team. The data analytics team is in charge of performing retrospective analysis of historical data, analytical verification and validation of current auto motor specifications and study design of future product testing. The executive team recognizes that the most successful automobile launches utilize data analytics in every decision making process. Therefore, Jeremy must ensure that his analysis contain a statistical backbone, quantitative metric and clear interpretation of the results in order to keep the upper management happy. Additionallt the data team consist of 5 members who only know how to program using 'R'. So Jeremy will have to learn a new language in order to perform the statistical tests. In this project I will help Jeremy perform statistical tests using 'R'. 

![a1](https://user-images.githubusercontent.com/23488019/153745054-a55f6d55-d97a-4ea7-9f41-9124a403d4cc.PNG)

## Purpose :

In this challenge, I will help Jeremy and the data analytics team do the following:

 - Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
 - Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
 - Run t-tests to determine if the manufacturing lots are statistically different from the mean population
 - Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. 
 
 
 ![a2](https://user-images.githubusercontent.com/23488019/153745092-3eaf2d23-6fe5-430a-b508-c5d80b554467.PNG)


 Thus, this project consists of three technical analysis deliverables and a proposal for further statistical study. The project is divided into the following parts:

 - Deliverable 1: Linear Regression to Predict MPG
 - Deliverable 2: Summary Statistics on Suspension Coils
 - Deliverable 3: T-Test on Suspension Coils
 - Deliverable 4: Design a Study Comparing the MechaCar to the Competition


## Software Used :

### 1. R - 
R is a versatile and extensible programming language with many benefits. One of the benefits of using an interpreted programming language such as R (or Python) is that the analysis scripts are written in plaintext. The versions of plaintext files are easy to control using tools such as Git, which means that R analysis scripts (or RScripts) are highly reproducible and easy to share with peers and collaborators. Another benefit to using R is that the R programming language was specifically designed for data analysis. This means that the process of loading in a dataset, visualizing the data, and performing statistical tests is straightforward and easy to interpret. In fact, many of the statistical tests in Python have been directly ported from R due to how well they were implemented. In addition to the native statistical functions, there are many other useful data transformation and modelling libraries, such as the tidyverse package, that simplify the process of ETL and visualizations.

### 2. RStudio Integrated Development Environment - 
Just as Jupyter Notebooks are an integrated development environment (IDE) used to help design and test Python scripts, RStudio is an IDE used to help design and test RScripts. RStudio provides users a graphical user interface (GUI) with multiple dynamic windows and perpetual access to their RScript and R console.

Similar to Jupyter Notebooks, RStudio enables users to test their analysis scripts line by line while allowing users to view different environment variables and outputs. This means that for each line of code written and executed, users can verify the results and troubleshoot any problems quickly and easily.


## Data Tools:

1. tidyverse
2. ggplot2
3. dplyr


## Results :

### 1. Deliverable 1 - Linear Regression to Predict MPG - 

The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using the knowledge of R, I  designed a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file. This is followed by  a short interpretation of the multiple linear regression results.



## Summary of Linear Regression to Predict MPG -
![del1](https://user-images.githubusercontent.com/23488019/153746057-2e93f5ee-e775-4208-8445-ca3867175f7e.PNG)
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

1. Datasets- MechaCar_mpg.csv and Suspension_Coil.csv
2. https://courses.bootcampspot.com/courses/791/pages/15
3. https://github.com/rstudio/cheatsheets/blob/main/data-visualization.pdf
4. https://cran.r-project.org/mirrors.html
5. https://cran.r-project.org/doc/manuals/r-release/R-intro.pdf


