# Water Quality, Crime, and Rent in Los Angeles County

### A Data Analysis Project Created by Kayla Brown, Max Dorris, and Matthew Peach

# Deliverable One
### Project Idea
**Problem Solving:** We are going to look at the connection between cost of living (i.e. rent), the quality of water, and crime in the different areas of Los Angeles County.

**Dataset:** We are using a set of crime data that we found on Kaggle as well as Water Quality Data from California.gov.  We are also using rent data from .  We combined the csv datasets into a database and used their postal ZIP codes as the common link for their locations.

**Predictive Problem to Be Solved:** We are going to make a linear regression model to estimate increases in rent in Los Angeles County based on water quality and crime.

### ERD Diagram

### Outline of Visualization Dashboard
Our plan for our dashboard is to use JavaScript to use geoapi in Python to create overlays in a map of Los Angeles County to use show rent, water quality, and crime across the whole area.

### Mockup of Machine Learning Model

Type: linear regression. Confusion matrix: 

#### Deliverable requirements via Brett:
- Finalized project idea including what is your dataset, what are the problems you solving, and what will be the predictive problem you will solve.
- Create an ER diagram and setup database for your data (if applicable)
- Create an rough outline of your visualization dashboard.
- Create a paper based mockup of your machine learning model.
- Continue to use Github for all the data

#### Deliverable 2 requirements:
- A detailed README.md file that includes the project status, images, descriptions, and results
- First attempt of a machine learning model, including a confusion matrix and accuracy score (20 points)
- First attempt of a working dashboard
- Database that stores data for the project (if applicable)
- Draft of presentation (edited) 


# Introduction

# Methods

# Results

# Conclusion:

One drawback of the Great-Circle Distance used in the pgeocode.haversine_distance(x,y) method for categorizing coordinates by their zipcode is that zipcode boundary-lines are non-circular and non-uniform, meaning that coordinates contained within a particularly irregular polygon may in fact be closer to the identifying "central" coordinate of another zipcode's polygon than they are to their own. Since we applied this method to each of our datasets before combining them, our data is only able to make predictions based on the approximate region.

