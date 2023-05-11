# Determining Factors of Stroke

### A Data Analysis Project Created by Kayla Brown, Max Dorris, and Matthew Peach

# Deliverable One
### Project Idea
**Problem Solving:** We are examining determining factors of stroke based on health and environmental factors. 

**Dataset:** We are using a set of data collected on over 5,000 patients that includes sex, age, hypertension, heart-disease, marital status, work type, type of residence, average blood glucose level (diabetes), body mass index, and historical smoking data.

**Predictive Problem to Be Solved:** We are making a classification model to estimate key factors leading to a stroke by comparing the factors mentioned in the dataset with whether the patient had a stroke or not in order to see which factors align most closely with those who have experienced a stroke.  The model we plan to use will be a random forest.

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
After extensive cleaning of the data to remove null data, we realized that in order to get any true accuracy with our model, we would need to balance the dataset in order to have an appropriate number of data points representing patients who have had a stroke.  We have also run an early version of a random forest classification model to get a baseline for accuracy before boosting the dataset.  The results were about as we expected:
![First attempt at random forest](https://github.com/MaxDorris/MachineLearningProject/blob/main/images/First_Run_Random_Forest.png)

As is, the data is overfitted such that guessing a 0 every time presents the score of 95% acccuracy.  We plan to use imblearn to create more data points of patients with strokes in order to improve our model.

**Working Dashboard Status:**

**Database Status:**
We started working on loading our data into Postgres this week, as can be seen in this repository, but this was completed before we created our plan for loading the database into AWS.

**Presentation Draft:**
We have started a draft of our presentation slides [here](https://docs.google.com/presentation/d/19WnwId6o2BqmmcGkq_VHWOdAGJx_eTl9xma43RCzPBA/edit?usp=sharing). These draft slides were made pretty early in the process of this project, so we know they need to be updated between now and next week when we present.

#### Deliverable 2 requirements:
- A detailed README.md file that includes the project status, images, descriptions, and results
- First attempt of a machine learning model, including a confusion matrix and accuracy score (20 points)
- First attempt of a working dashboard
- Database that stores data for the project (if applicable)
- Draft of presentation (edited) 

# Deliverable 3:

















**Draft ideas**
.
.
.
Conclusion:
  1. Major imbalance in dataset.
  2. The model's predictive ability is extremely limited, despite _____ accuracy. We believe stress may be measured with hormone (ex: cortisol) levels more accurately than through self-reported answers to questions on previous environmental factors. While stressful events like a previous stroke, being overworked, living in crowded areas, and smoking may contribute to the likelihood of a future stroke event, predicting WHEN or IF someone will have a stroke is futile with this data. Pairing stress history with realtime stress-related measurements may be a stronger approach to predicting stroke risk at the time of measurement more accurately. Results would be most precise at the time of testing, and would deviate with time. An model which accurately predicts these deviations in risk using current estimated heartbeat and blood oxygen, chemical metrics from the most recent evaluation, and trends in evaluation history could be used to estimate realtime risk a with non-invasive wearable device (ex: smartwatch) for a limited time after an evaluation.
