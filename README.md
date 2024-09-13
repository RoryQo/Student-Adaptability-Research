# Student-Adaptability to Online Learning Research

 This project does an in-depth analysis of the student adaptability level of students to online classes/education and aims to predict the adaptability level of the students (high, moderate, or low) given feature data for the student.  Part one focuses on encoding and preparing the data (data wrangling).  Part two focuses on data visualization, displaying the data to view relationships between the features themselves and the target.  Parts three and four implement and compare supervised and unsupervised learning techniques (neural networks, random forests, KNN, etc.) to predict the adaptability level. Part four contains the conclusion for the best model and model applications.

#### Results
Given future feature data, we can predict a student's online learning adaptability level using our non
linear svm or Random Forest model. This model could be used to adjust the teaching style or budget allocation of learning materials to best accommodate the predicted adaptability level of students.  According to the testing data, our nonlinear SVM model and random forest model were accurate in predicting student adaptability levels approximately 93% of the time.  It appears the top four most important factors (from the random forest model) are age, class duration, gender, and education level (in order from most to least important).  The last four important factors (least important to more important) are device type, LMS availability, internet type, and load-shedding.

+ More basic models like Naive Bayes,and regularized regression were not sufficiently accurate (less than 70%), so we continued to fit more advanced models for improved accuracy
+ Nonlinear SVM model and Random forest models were the best (93% Accurate)
+ Neural networks and other unsupervised learning models were all fairly accurate (valid models)



#### Data Description
##### Features
* `Gender:` Gender type of student
* `Age:` Age range of the student
* `Education Level:` Education institution level
* `Institution Type:` Education institution type
* `IT Student:` Studying as IT student or not
* `Location:` whether student is located in town or not
   `Load-shedding:` Level of load shedding
* `Financial Condition:` Financial condition of family
* `Internet Type:` Internet type used mostly in device
* `Network Type:` Network connectivity type
* `Class Duration:` Daily class duration
* `Self LMS:` Institution’s own LMS availability
* `Device:` Device used mostly in class

##### Target
* `Adaptability Level:` Adaptability level of the students
