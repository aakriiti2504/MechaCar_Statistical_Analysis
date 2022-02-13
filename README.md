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

## 1. Deliverable 1 - Linear Regression to Predict MPG - 

The MechaCar_mpg.csv dataset contains mpg test results for 50 prototype MechaCars. The MechaCar prototypes were produced using multiple design specifications to identify ideal vehicle performance. Multiple metrics, such as vehicle length, vehicle weight, spoiler angle, drivetrain, and ground clearance, were collected for each vehicle. Using the knowledge of R, I  designed a linear model that predicts the mpg of MechaCar prototypes using several variables from the MechaCar_mpg.csv file. This is followed by  a short interpretation of the multiple linear regression results.



## Summary of Linear Regression to Predict MPG -

![del1](https://user-images.githubusercontent.com/23488019/153746057-2e93f5ee-e775-4208-8445-ca3867175f7e.PNG)

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
Statistically speaking, the vehicle ground clearance and the vehicle length are more likely to provide non random amounts of variance to the model. They have a significant impact on miles per gallon of the prototype. The p-values of spoiler angle, AWD and the vehicle weight have varying variance with the given dataset.  

2. Is the slope of the linear model considered to be zero? Why or why not?
The assumed signifance level is 0.05% and the p-value for the given model is 5.35e-11. This value is much smaller hence the null hypothesis can be conveniently rejected. Hence, the slope of the linear model is not zero.

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
The r-squared value of 0.7149, that is 71% of all th empg predictions can be determined fo rthis linear model. Hence the multiple regression model does predict the Mechacar prototypes effectively.


## 2. Deliverable 2: Summary Statistics on Suspension Coils - 

The MechaCar Suspension_Coil.csv dataset contains the results from multiple production lots. In this dataset, the weight capacities of multiple suspension coils were tested to determine if the manufacturing process is consistent across production lots. Using knowledge of R, I have created a summary statistics table to show:

 - The suspension coil’s PSI continuous variable across all manufacturing lots
 - The following PSI metrics for each lot: mean, median, variance, and standard deviation.
 
![del2](https://user-images.githubusercontent.com/23488019/153746961-1ad14dc3-b50b-4e8f-8b05-4e60c1c0237b.PNG)

The total_summary dataframe looks like the following - 

![tot summary del 2](https://user-images.githubusercontent.com/23488019/153746521-a3cbf286-9de7-4cd6-b6c5-c6525079666c.PNG)



The lot_summary looks like the following - 

![lot summary del 2](https://user-images.githubusercontent.com/23488019/153746551-8d0d1e6d-51b3-487a-9063-6fd4a58b78a2.PNG)

## Summary Statistics on Suspension Coils - 
A short summary using screenshots from the total_summary and lot_summary dataframes, and addressing the following question: 

- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
The entire population of the production lot, the variance of the coils is 62.29 PSI, which is well within the 100 PSI variance requirement. Lots 1 nad 2 are within the given range however lot 3 has some variance. As we know the following Ho and Ha definitions - 

- Ho: There is no significant difference between the mean PSI of all manufacturing lots and individual lots and population mean of 1500 PSI. 
- Ha: There is significant difference between the mean PSI of all manufacturing lots and population mean of 1500 PSI

The design specifications for the suspension coils show that the variance of the suspension coils must not exceed 100 pounds per square inch. It can also be noted that the Lot 1 and Lot 2 are  within design the specifications since they have similar mean and median. Lot 3 shows the most variance and exceeds the manufacturers specifications.

## 3. Deliverable 3: T-Test on Suspension Coils -

Here we will perform t-tests to determine if all manufacturing lots and each lot individually are statistically different from the population mean of 1,500 pounds per square inch. An RScript is written for t-test that compares all manufacturing lots against mean PSI of the population. This was done using the t.test() function to determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch. 

![del 3](https://user-images.githubusercontent.com/23488019/153746969-63007434-3aa6-44cf-89be-02dbb6a9434f.PNG)

Secondly, An RScript is written for three t-tests using t.test()  function and its subset() argument to determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 pounds per square inch.


## Summary of T-Test on Suspension Coils - 
There are two main forms of the t-test that we use: the one-sample t-test and the two-sample t-test. The one-sample t-test is used to determine whether there is a statistical difference between the means of a sample dataset and a hypothesized, potential population dataset. In other words, a one-sample t-test is used to test the following hypotheses:

- H0 : There is no statistical difference between the observed sample mean and its presumed population mean.
- Ha : There is a statistical difference between the observed sample mean and its presumed population mean.
Before we can apply any statistical test to our data, we must check if there are any assumptions regarding our input dataset. When it comes to our one-sample t-test there are five assumptions about our input data:

- The input data is numerical and continuous. This is because we are testing the distribution of two datasets.
- The sample data was selected randomly from its population data.
- The input data is considered to be normally distributed.
- The sample size is reasonably large. Generally speaking, this means that the sample data distribution should be similar to its population data distribution.
- The variance of the input data should be very similar.
As long as our input data satisfies (or mostly satisfies) the above assumptions, we can use the one-sample t-test to assert the similarities or differences in our data.

Finally, summarizing the interpretation and findings for the t-test results below -
After conducting the  t-test on the suspension coil data to determine whether there is a statistical difference between the mean of this provided sample dataset and a hypothesized, potential population dataset, we find that the true mean of the sample is 1498.78. the p-value of 0.06 is higher than the common significance level of 0.05. As a result it looks like there is not much evidence to do away with th enull hypothesis. The mean of all the three lots manufactured are statistically similar to the pre assumption mean of 1500. 
For lot 1, the sample has the true sample mean of 1500. Thus there is no statistical difference between the observed sample mean and presumed population mean. Hence the null hypothesis cannot be rejected.
For lot 2,the outcome is similar with sample mean of 1500.02, p-value of 0.61. The null hypothesis cannot be rejecetd. Also, the sample and population means are statistically similar.
For lot 3, the sample mean is 1496.14 and pvalue is 0.04 which is lower than the common significance level of 0.05. Hence we will reject the null hypothesis since the p-value is low enough. This lot needs to be reevaluated.


## 4. Deliverable 4: Design a Study Comparing the MechaCar to the Competition -
In this deliverable we will design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers.

## Study Design: MechaCar vs Competition.
Here we will discuss the statistical study that can quantify how the MechaCar performs against the competition. We need to ponder upon the metrics that would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating. As a result, the following questions can be answered - 

1. What metric or metrics are you going to test?
A lot of different metrics will be tested for this study. Some of them are shown below:
 - Selling price as dependent variable
 - Engine type as independent variable
 - Efficiency as independent variable
 - Maintenance as independent variable
 - Customer satisfaction rating as independent variable
 - Safety rating as independent variable

2. What is the null hypothesis or alternative hypothesis?
The N ull Hypothesis and the Alternative Hypothesis can  be defined as follows:
- Null Hypothesis (Ho) - Based on the key factors, the MechaCAr is priced right.
- Alternative Hypothesis (Ha) - Based on the key factors, the MechaCAr is NOT priced right.

3. What statistical test would you use to test the hypothesis? And why?
Multiple linear regression is a statistical model that extends the scope and flexibility of a simple linear regression model. Instead of using a single independent variable to account for all variability observed in the dependent variable, a multiple linear regression uses multiple independent variables to account for parts of the total variance observed in the dependent variable.
 I would use the multiple linear regression test because it will be helpful in determining the factors having the greatest predictability with the dependent variable, that is the selling price in this case. Although the multiple linear regression model is far better at predicting our current dataset, the lack of significant variables is evidence of overfitting. Overfitting means that the performance of a model performs well with a current dataset, but fails to generalize and predict future data correctly.

4. What data is needed to run the statistical test?
Since a multiple linear regression uses multiple independent variables to account for parts of the total variance observed in the dependent variable, a lot of different data like the selling price and all the variables that have the most impact on the selling price will be needed to run the test effectively. 


## Resources : 

1. Datasets- MechaCar_mpg.csv and Suspension_Coil.csv
2. https://courses.bootcampspot.com/courses/791/pages/15
3. https://github.com/rstudio/cheatsheets/blob/main/data-visualization.pdf
4. https://cran.r-project.org/mirrors.html
5. https://cran.r-project.org/doc/manuals/r-release/R-intro.pdf


