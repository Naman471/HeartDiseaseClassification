# HeartDiseaseClassification
![heart](https://user-images.githubusercontent.com/62702112/112947370-54262b00-9154-11eb-89b8-7ba6822dcfe9.png)
* This project aims at developing a fundamental machine learning model which can predict the possibility of a heart disease based on a person's medical history
## Introduction
Given the medical history of a patient, such as:
* Chest pain type
* Resting blood pressure
* serum cholestrol
* age/sex <br>
We intend to develop a model which could classify whether the person is having a heart disease or not
## DataSet and EDA(Exploratory Data Analysis)
The original dataset came from the Cleavland data from the UCI Machine Learning repository<br>
There is also a version of it available on kaggle. https://www.kaggle.com/ronitf/heart-disease-uci
<br><br>
Initial EDA suggested 75% women would have chance of having a heart disease  compared to 50% men. Thus, there exists a strong correlation between the target column and sex.
## Model Selection and Evaluation
We've used logistic regression for our data. <br>After running through RandomizedSearchCV and GridSearchCV, our model accuracy stood at 88.5%
Some of the best hyper-parameters we cam up with are: <br>
'C': 0.23357214690901212,<br>
 'dual': False,<br>
 'fit_intercept': True,<br>
 'penalty': 'l2',<br>
 'solver': 'liblinear'<br>
Here's a quick glance at the 5 cross fold evaluation metrics of the model:
![SS-Evaluation-1](https://user-images.githubusercontent.com/62702112/112946848-a0bd3680-9153-11eb-8643-42d294e4f90d.JPG)
## Tools Used
In the completion of this project, I've used tools such as pandas and numpy for data analysis, seaborn and matplotlib for data visualization 
