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
![image](https://user-images.githubusercontent.com/120230351/210700426-8e895fa8-995e-48ad-8958-d6866283e98f.png)
![image](https://user-images.githubusercontent.com/120230351/210700461-a63e8322-1a44-4313-9b9c-ffa4d5454109.png)
![image](https://user-images.githubusercontent.com/120230351/210700462-afcdcd1b-8133-4854-877c-d1cbcc805092.png)
![image](https://user-images.githubusercontent.com/120230351/210700481-272b0d83-5e3d-46ae-9051-eb41e048589f.png)
![image](https://user-images.githubusercontent.com/120230351/210700506-e09cfb0b-87c4-4576-baf0-43b4199db732.png)
![image](https://user-images.githubusercontent.com/120230351/210700523-d46fa1a0-e821-4f48-8b6c-a93f0f3cae0d.png)
![image](https://user-images.githubusercontent.com/120230351/210700546-452420ec-5bba-4d38-b518-ff3a85f28678.png)

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



