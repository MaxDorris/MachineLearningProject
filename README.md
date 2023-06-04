# Determining Factors of Stroke

*** NOTE: This project is not yet updated and was cut short due to time constraints. After finding a better dataset a simialr analysis will be conducted to further this investigation with shallow and deep learning models.

## A Data Analysis Project Created by Kayla Brown, Max Dorris, and Matthew Peach

### Project Overview
**Problem Statment:** What are the determining factors for strokes?

**Dataset:** We are using a set of data collected on over 5,000 patients that includes sex, age, hypertension, heart-disease, marital status, work type, type of residence, average blood glucose level (diabetes), body mass index, and historical smoking data.  Each patient was also evaluated for whether they had a stroke.  

**Predictive Problem to Be Solved:** We are making a classification model to estimate key factors leading to a stroke by comparing the factors mentioned in the dataset with whether the patient had a stroke or not in order to see which factors align most closely with those who have experienced a stroke.  The model we plan to use will be a random forest.

**Materials:** The data was gathered from a group on Kaggle which used this data to determine similar factors for stroke victims compared to other patients.  To complete our project, we have used Tableau for our visualizations, Amazon Web Services to house our data in a database, pgAdmin, and Python as the language for our machine learning model.  Within the model we have used several dependencies, including Pandas, Numpy, Matplotlib, and sklearn.

### Project Components
#### Database
To prepare the database, we first created an Entity Relationship Diagram (ERD) in order to plan our our data.  
![ERD Version 1](https://github.com/MaxDorris/MachineLearningProject/blob/main/images/ERD_1.png)
We then created a pipeline to connect our dataset from a simple spreadsheet to the AWS RDS instance and then load it into PGAdmin.  From there, we used this as the place from which we could create our machine learning model.

#### Machine Learning Model
The dataset as we first encountered it required some cleaning to remove null data and to remove superfluous fields from the data set.  We then ran an initial classification model, specifically a random forest classification model, to get a baseline for accuracy before boosting the dataset. 
![First attempt at random forest](https://github.com/MaxDorris/MachineLearningProject/blob/main/images/First_Run_Random_Forest.png)
These initial results were overwhelmingly correct because of the unbalanced nature of our dataset.  A visualization of our data when comparing patients who had experienced a stroke versus those who had not revealed that nearly 96% of the patients in our dataset had not experienced a stroke.

![Unbalanced Data Ratio](https://github.com/MaxDorris/MachineLearningProject/blob/main/Unbalanced_Data_Pie_Chart.png)

This meant that the model could guess "0" every time and be correct with tremendous accuracy.  To overcome this overfitting of the data, we used imblearn to create more data points of patients with strokes in order to improve our model.

#### Data Visualizations
For our data visualizations, we used Tableau to delineate between patients who had experienced a stroke and those who had not, and then created our dashboard, which can be viewed [here](https://public.tableau.com/views/MachineLearning_16838699374380/StrokeData?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link).

### Conclusions

The **slides** for our final presentation can be found [here](https://docs.google.com/presentation/d/19WnwId6o2BqmmcGkq_VHWOdAGJx_eTl9xma43RCzPBA/edit?usp=sharing).

In the end, the limitations of the dataset left us with more questions when comparing data sets.  Had we collected the data, we would have asked more specific questions to clarify several of these columns to help determine the data.  We also would have conducted further research on stroke patients themselves to expand the study and create a more naturally balanced dataset.
