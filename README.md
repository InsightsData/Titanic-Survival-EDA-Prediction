# Titanic-Survival-EDA-Prediction

Python | EDA | Prediction
-

Overview
-
  - Various visualizations were used to illustrate who and why people were survived or didn't survive
  - Feature engineering was introduced throughout the project
  - Random Forest was carefully selected out with the help of cross validation and confusion matrix
  - After fine tuning, the Random Forest model reached an accuracy of 87.3%

Packages
-
  - NumPy, Pandas, Matplotlib, Seaborn, Sklearn

Data source
-
  - Titanic - Machine Learning from Disaster
  - https://www.kaggle.com/competitions/titanic
  
Data cleaning
-
  - Check data types
  - Deal with missing values using three different methods, i.e. replace nulls in "Age" with mean age according to titles extracted from "Name"
  
 
EDA
- 
<img width="956" alt="image" src="https://user-images.githubusercontent.com/120230351/210700391-c656edbe-b0ff-4831-a88b-af635fd7e6e6.png">
<img width="693" alt="image" src="https://user-images.githubusercontent.com/120230351/210701471-98e11e55-21a2-4377-87a9-8c7647ad07fd.png">
<img width="689" alt="image" src="https://user-images.githubusercontent.com/120230351/210701529-59b79aa2-69ad-460d-af7f-1d79a5e7e4ef.png">
<img width="695" alt="image" src="https://user-images.githubusercontent.com/120230351/210701583-075b1668-dd21-4f75-ba31-c835adb97136.png">
<img width="385" alt="image" src="https://user-images.githubusercontent.com/120230351/210701638-99e78135-93c2-4eaa-86e7-097813dab11c.png">
<img width="394" alt="image" src="https://user-images.githubusercontent.com/120230351/210701679-f46cd672-54f7-47b6-9747-17997bff4379.png">
<img width="379" alt="image" src="https://user-images.githubusercontent.com/120230351/210701719-691cd828-3b8d-42d8-8288-c21187aaf534.png">
<img width="400" alt="image" src="https://user-images.githubusercontent.com/120230351/210701751-790ac5b4-5a95-4c8d-b317-4445142d6250.png">

  - Who survived and who did not?
 1. People in the first class had the highest survival rate(0.63), compared to the second class(0.47) and the 
    third class(0.24).
 2. Over 70% women on board got rescued.
 3. Most passengers were the young and the middle-aged, but children had the highest chance of survial, 
    and middle-aged as well as senior passengers had the lowest survial rate.
 4. Small family size (under 3) had higher chances of survival, and passengers with 1 sibling/spouse or 
    parent/child had the highest chance of survival.
 5. The more people paid for the tickets, the more likely they would survive.
 6. Over half of the passengers embarked at Cherbourg survived, while passengers who embarked at Southampton 
    survived the least.
  - Why?
  
[Money secured safety.]
1. The first class tickets were more expensive on average.
2. People who paid for the highest price got rescued. Even though two of them were men.

[Women and children were given the first priority during the rescue.]
1. Mean ages for men and women were similar.
2. In each class on the Titanic, more women and children were rescued.
3. Different class type did have different impact on women and children's survival rate. For in the first and second 
   class, women's survival rate reached around 0.9, compared to about 0.5 in the third class; All children were saved 
   in the second class! 
4. The youngest kid got rescued, though the child was in the third class.

[The highest survival rate for passengers boarded at Cherbourg was due to a fairly large proportion of passengers 
with high socio-economic status.]

Feature engineering
-
  - Add features of "Age_group", "Fare_range" and "Title"
  - Transform categorical features to numeric ones
 
Prediction
-
![image](https://user-images.githubusercontent.com/120230351/210700572-f0bdcd1f-9f75-49dc-86a9-81730e9aa24b.png)
![image](https://user-images.githubusercontent.com/120230351/210700585-fe910eb1-a352-4a8d-84c1-ce2514ca5752.png)
![image](https://user-images.githubusercontent.com/120230351/210700594-518b4446-3e3d-4bd9-a18a-cc97f41fcc38.png)

  - Check correlation
  - Split data
  - Choose classification algorithmns
  - Cross validation
  - Tune Random Forest

Random Forest
Accuracy: 87.3%



