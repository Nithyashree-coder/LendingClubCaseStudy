# Lending Club Case Study
This repository contains data analysis for Lending Club Use Case deciding upon the status of loan that are likely to be default. <br>
I have created a class that automates data analysis and it is designed especially to check on null column value analysis and null row value analysis.  <br>
It separates numerical and categorical columns. Rest of the EDA is done accordingly.  <br>
<p> Data Understanding is the main class which has data description, removes unwanted rows and columns. <br>
    The dataframe is reused as an object for the methods to perform the operations in accordance as after cleaning, we will get new dataframe everytime.  <br> 
<br>
Data Description - Basic information of the data from the dataframe. 
<pre>
RemoveUnwantedRowsCols - Does common data analysis for Rows and Columns
    checkForUnwantedColumns - Checks for columns only if all the values are NaN
    nullValueColumnAnalysis - Checks for higher number of null values in columns
    nullValueRowAnalysis - Checks for higher number of null values in rows. If remove rows is true then it will remove 
                            null rows. 
    detectContinuousCategorical - Seperates continuous and categorical variables in the dataset with a threshold 
                                    of 10 different values.
    numericalColumnsAnalysis - Column analysis for continuous variables. This will analyse the continuous columns that 
                               are obtained after detecting categorical and continuous variables and does 
                               segmented analysis as well given the condition.
    categoricalColumnsAnalysis - Column analysis for continuous variables. This will analyse the categorical columns 
                                 that are obtained after detecting categorical and continuous variables and does 
                                 segmented analysis as well given the condition.
</pre>
</p>


## Table of Contents
* [Data Understanding Before Cleaning](#Data-Understanding-Before-Cleaning)
* [Data Cleaning](#Data-cleaning)
* [Data Analysis](#Data-analysis)
* [Segmented Univariate Analysis](#segmented-univariate-analysis)
* [Data Analysis](#Data-analysis)
* [Bivariate Analysis](#bivariate-analysis)
* [Multivariate Analysis](#multivariate-analysis)
* [Conclusion](#Conclusion)

## General Information
- Dataset being used is loan.csv. 
- Our task is to predict the loan defaulters.
- The reason why we are doing this is because i f one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss for the company.
- Identification of such applicants using EDA is the aim of this case study.

## Conclusions
- Term has significant impact in loan_status
- Grade has significant impact in loan_status
- Loan amount has significant impact in loan_status
- term has significant impact in loan_status
- Home ownership has significant impact in loan_status
- Annual income has significant impact in loan_status
- Profit and loss has significant impact in loan_status


## Technologies Used
- pandas - version '1.2.4'
- seaborn - version '0.11.1'
- numpy - version '1.20.1'

## Acknowledgements
- Print using bold:
    https://stackoverflow.com/questions/8924173/how-do-i-print-bold-text-in-python

- Check which column contains null values:
https://stackoverflow.com/questions/36226083/how-to-find-which-columns-contain-any-nan-value-in-pandas-dataframe

- Nested class in python:
https://www.geeksforgeeks.org/inner-class-in-python/![image](https://user-images.githubusercontent.com/61308322/157503086-6a3fc97e-701b-4ccd-979b-8db996a4885a.png)



## Contact
Created by [@Nithyashree-coder] - feel free to contact me!

