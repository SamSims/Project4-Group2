# Team Stars and Stats: A Glance at Medicare from Rating to Retention 
Project4-Group2

# Project Brief
Star ratings are synonymous with the world of consumerization, influencing opinions and purchasing behavior – but is the same true in the world of healthcare?  Team Stars & Stats plan to look under the hood of Medicare Plan star ratings – ratings typically aggregated as one overall number but represent individual value of care scores that consumers weigh differently.  

By analyzing and modeling this vast data set, we want to understand if star ratings actually show correlation to enrollment choice, while predicting which plans, or plan benefits, will be popular in the future. 

## Do star ratings drive consumer choice? 
## If they do, which insurer will people predominantly go with the following year?  
## Which sub-category of coverage is ranked highest?

# Scope
CMS Medicare Data (Star Rating and Enrollment Data) 2013-2023

# Data
1. CMS Medicare Star Ratings by plan 
2. Medicare Monthly Enrollments
3. Census Data (Pop 65+ by FIPS)

## Data Key Takeaways
CMS Medicare Star Rating File format changed in 2020; a few notable changes:
  > Removal of separate Spring and Fall files; combined into one file moving forward
  > Additional data included (disenrollment & disenrollment reason data)
  > Difference in number of total sub-categories year by year (between 30 and 34 total), with discrepancies such as the inclusion of a foreign call center
  > Column naming varies year by year depending on number of columns

CMS Medicare Enrollment Data 
  > Files missing for March, April, May, June, November 2017, and August 2018
  > Data organized differently 2013-2016 vs. 2020 and after.

Only a few years of Medicare Disenrollment is publicized in the CMS files.  It did not become a mandatory reporting requirement until the passing of the 21st Century Cures Act, starting in 2020 so we excluded this data from the modeling.

# Models Used
  > Linear Regression: Though this rendered a high level of accuracy for predicting overall star ratings (98% accuracy), it was not as successful doing the same for enrollment (73% accuracy)
  > Random Forest: This was able to calculate feature importance for both Star Rating and Enrollment in order for us to understand how much each feature contributes to making accurate predictions.
  > Keras-Tuner







