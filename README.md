# LendingClubCaseStudy
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
