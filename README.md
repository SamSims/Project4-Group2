# Team Stars and Stats: A Glance at Medicare from Rating to Retention 
Project4-Group2

# Project Brief
Star ratings are synonymous with the world of consumerization, influencing opinions and purchasing behavior – but is the same true in the world of healthcare?  Team Stars & Stats plan to look under the hood of Medicare Plan star ratings – ratings typically aggregated as one overall number but represent individual value of care scores that consumers weigh differently.  

By analyzing and modeling this vast data set, we want to understand if star ratings actually show correlation to enrollment choice, while predicting which plans, or plan benefits, will be popular in the future. 

## Do star ratings drive consumer choice? 
## If they do, which insurer will people predominantly go with the following year?  
## Which sub-category of coverage has the largest impact on a plan's Star Rating or on Enrollment?

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

  > Keras-Tuner: This model was able to find the best model parameters for greatest accuracy

  > Deep Learning Model: Using Epochs to find how well accurate Standardized Enrollment is against the rest of the data
    1.  1st attpempt: 72% accuracy
    2.  2nd attempt: 72% accuracy
    3.  3rd attempt: 73% accuracy

# Final Analysis
Though Consumers tend to weigh heavily on Consumer ratings for everyday items (e.g. Amazon, TripAdvisor, Yelp, etc), it seems that the level of popularity is not the same for Medicare Healthcare star ratings (as of yet).  One of the main reasons is likely because it's not a true Consumer Rating; it's analyzed and weighted by 3rd parties. The other reason(s) could be related to data and time that we didn't have to run further analysis: advertising impact, brand recognition scores, broker outreach, price (premiums/OOP), and disenrollment rates.







