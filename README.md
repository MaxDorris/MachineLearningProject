# Determining Factors of Stroke

### A Data Analysis Project Created by Kayla Brown, Max Dorris, and Matthew Peach

# Deliverable One
### Project Idea
**Problem Solving:** We are examining determining factors of stroke based on health and environmental factors. 

**Dataset:** We are using a set of data collected on over 5,000 patients that includes sex, age, hypertension, heart-disease, marital status, work type, type of residence, average blood glucose level (diabetes), body mass index, and historical smoking data.

**Predictive Problem to Be Solved:** We are making a linear regression model to estimate key factors leading to a stroke by comparing the factors mentioned in the dataset with whether the patient had a stroke or not in order to see which factors align most closely with those who have experienced a stroke.

### ERD Diagram
We are working with a single dataset, so we are still working out how a database will function in our project.  We made an ERD for the data we have.
![ERD Version 1](https://github.com/MaxDorris/MachineLearningProject/blob/main/images/ERD_1.png)

### Outline of Visualization Dashboard
Our plan for our dashboard is to use charts to show factors individually and as a group in order to display different risk factors for strokes.
Here are some initial ideas:
![sample visualizations](https://github.com/MaxDorris/MachineLearningProject/blob/main/images/Data_Visualization_Mockup.png)

### Mockup of Machine Learning Model
![Machine Learning Visualization](https://github.com/MaxDorris/MachineLearningProject/blob/main/images/Machine_Learning_Mockup.png)
Prior to creating our model, we plan to create a pairplot, PCA, and correlation heatmap to determine the relationships between our input variables. We will then create a binary classification model with all features except **id** (dropped) and **stroke**, which will be our target. We will record differences in accuracy and sensitivity between supervised ML models and a Tensorflow-based neural network. Finally, we will optimize the neural network to determine the best activation functions and number of dense layers.




#### Deliverable 1 requirements:
- Finalized project idea including what is your dataset, what are the problems you solving, and what will be the predictive problem you will solve.
- Create an ER diagram and setup database for your data (if applicable)
- Create an rough outline of your visualization dashboard.
- Create a paper based mockup of your machine learning model.
- Continue to use Github for all the data

# Deliverable 2

### Project Status
**Machine Learning Status:**  

**Working Dashboard Status:**

**Database Status:**

**Presentation Draft:**

#### Deliverable 2 requirements:
- A detailed README.md file that includes the project status, images, descriptions, and results
- First attempt of a machine learning model, including a confusion matrix and accuracy score (20 points)
- First attempt of a working dashboard
- Database that stores data for the project (if applicable)
- Draft of presentation (edited) 
