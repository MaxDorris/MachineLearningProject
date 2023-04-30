# Water Quality, Crime, and Rent in Los Angeles County

    A Data Analysis Project Created by Kayla Brown, Max Dorris, and Matthew Peach

# Deliverable One
### Project Idea
*Project Idea:*
*Dataset:* We are using a set of crime data that we found on Kaggle as well as Water Quality Data from California.gov.  We are also using rent data from ___.  We combined the csv datasets into a database and used their postal ZIP codes as the common link for their locations.
*Problem Solving:* We are going to look at the connection between cost of living (i.e. rent), the quality of water, and crime in the different areas of Los Angeles County.
*Predictive Problem to Be Solved:* We are going to make a linear regression model to estimate increases in rent in Los Angeles County based on water quality and crime.

### ERD Diagram

### Outline of Visualization Dashboard

### Mockup of Machine Learning Model


#### Deliverable requirements via Brett:
- Finalized project idea including what is your dataset, what are the problems you solving, and what will be the predictive problem you will solve.
- Create an ER diagram and setup database for your data (if applicable)
- Create an rough outline of your visualization dashboard.
- Create a paper based mockup of your machine learning model.
- Continue to use Github for all the data


# Introduction

# Methods

# Results

# Conclusion:

One drawback of the Great-Circle Distance used in the pgeocode.haversine_distance(x,y) method for categorizing coordinates by their zipcode is that zipcode boundary-lines are non-circular and non-uniform, meaning that coordinates contained within a particularly irregular polygon may in fact be closer to the identifying "central" coordinate of another zipcode's polygon than they are to their own. Since we applied this method to each of our datasets before combining them, our data is only able to make predictions based on the approximate region.

