# -VA-Boston-Healthcare-System
The Data Science Assessment 

Predictive Model of One Year Survival after diagnosis with NSCLC Write Up

I began this project by examining the two data files and the descriptions of their contents and variables.
Starting with clinical.csv, I Checked for duplicates found none from the ID names.
Then I removed all rows with a Survival Month of less than 1 year as the core task was to create a model 
  dealing with survivability after one year of diagnosis. 
Missing values were treated next by examining which variables corresponded to each other and how much relative
  data was missing and how much total data was missing per variable. 
This led me to removing 4 groups from the data set as it was missing most of the remaining data or the related 
  groups together were missing a majority of the data to be used in building a model. 
After trimming the missing data from the remaining variable, I next checked each variable for the unique 
  variables and their counts to check for duplicate groups or other items that needed to be combined.
Correcting informaiton in several groups to be a consitant format was done next, and after all that the 
  removed ID values were then discarded from the genomics.csv data for consistancy. 
After looking through the trimmed genomics.csv data, I continued with the clinical.csv data and created 
  several new variables converting the categorical data into numerical data for graphical examination 
  in looking for trends and connections. 
An examination of the data showed several outliers that were then discarded from the data set. 
I then examined the data graphically using several methods to identify correlations and trends.

Of note are: 
-When there is a primary tumor, it showed a slight correlation to if the person was alive
-The Stage of cancer seemed to increase when the Primary Site was in the Right Lung or Upper Left Lung
-After 36 months of follow up, the amount of people alive increased
-For the Tumor Size at diagnosis was larger than 6 inches, all but one died out of many
-There were less people who recieved radiation treatment, but the percentage of those who recieved treatment
  and died was closer to those who died without treatment vs those who received treatment and lived was a 
  relativly smaller percentage against those who did not receive treatment. 

I chose the features that had the stronget correlation with the Survival Months, Outcome, and each other.
It would have been useful to use the data between the Stage, Grade, and TNM diagnosis to incoporate more 
  data for examination, and to create a map of intensity and if the cancer was spreading from the Primary 
  Site to compare against Survival Months and if they recieved Radiation treatment. 

Using Extra Tree Regression as my algorithm was done due to me using both categorical and numerical data.
  It also allowed for some compensation for data cleaning and analysis that I was unable to get to. 
  I analyzed my model using MSE and R2 values for training and test data to identify the features I chose
  and to test my data cleaning and analysis. There are clear signs for improvment in both and given more 
  time I would have scrubbed through the data more throughly, engineered features better reflecting the 
  data, and created a more true model. 
  
With more data, I would be able to better utilize the other features that I had to discard, and with the 
  help of a subject matter expert, I would have been able to better select which features I should focus
  more time on treating or engineering to create a final data set for analysis and model creation. 
  
