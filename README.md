# Data-Science-and-Machine-Learning

**Student Name: Qadeer Hussain**

**Student ID: C00270632**

**Lecture: Greg Doyle**

**K Nearest Neighbour**

# Project Description
The purpose of this project is to predict the classifcation of a car based on multiple factors.

# Data Source
The dataset that was used for this project can be downloaded from https://archive.ics.uci.edu/dataset/19/car+evaluation

# Data
Attributes
- buying       v-high, high, med, low
- maint        v-high, high, med, low
- doors        2, 3, 4, 5-more
- persons      2, 4, more
- lug_boot     small, med, big
- safety       low, med, high

Classes
- unacc
- acc
- good
- vgood

# Processing
After downloading this dataset, a test print was conducted using the following code ```data.head()```. The loaded data was then displayed. A check was done to find missing values in the dataframe using the following code ```missing_values = data.isnull().sum()```, ```print(missing_values)```. This found no missing values in the dataset. One hot encoding was then done on the following columns ```buying```,	```maint```,	```doors```,	```persons```, ```lug_boot```, ```safety```. The data was then split into features and target variable. The target variable was ```class```. Data was then split into training and testing set 70%  training and 30% testing. SMOTE was applied to help the class imbalance as ```unacc``` and ```acc``` had much more samples. After this finding the best number of neighbours for KNN using F1 score. 

# Data Understanding and Visualisation 
After processing the data and finding the best neighbours which was 11 the model was fit

1. Classfication report

   ![image](https://github.com/user-attachments/assets/2d9140ce-d940-47ac-9fc0-56d39123a562)

2. Confusion Matrix
   
   ![image](https://github.com/user-attachments/assets/1c24a5b2-b351-4330-bb71-39f87efa85f9)

3. Model in use

   ![image](https://github.com/user-attachments/assets/33a72fbd-431f-4c4e-8032-e67a479714df)

# Algorithims:
K Nearest Neighbour: This is a supervised machine learning algorithm which uses proximity to make classifications or predictions about the grouping of data point. In this project the classification of cars based multple factors was done.

# Online Sources:
1. Mmdatainfo. (2020, April 21). K-Nearest Neighbors. Kaggle. https://www.kaggle.com/code/mmdatainfo/k-nearest-neighbors
2. User guide# (2025) User Guide - pandas 2.2.3 documentation. Available at: https://pandas.pydata.org/docs/user_guide/index.html (Accessed: Feb 2025).
3. Matplotlib 3.9.2 documentation# (2025) Matplotlib documentation - Matplotlib 3.9.2 documentation. Available at: https://matplotlib.org/stable/ (Accessed: Feb 2025).
4. User guide (2025) scikit. Available at: https://scikit-learn.org/stable/user_guide.html (Accessed: Feb 2025).
5. Comment, info, M., kartik, kartik Follow, Kartik, & Follow. (2025). K-Nearest Neighbor(KNN) algorithm. GeeksforGeeks. https://www.geeksforgeeks.org/k-nearest-neighbours/ 

# Tools and Tech Used: 
1. K Nearest Neighbours
2. Jupter Notebook
3. Pandas Library - Loading the data and analysing it
4. Matplotlib - Plotting and Visualising the graph 
5. Scikit Learn(Sklearn) - Implementing K Nearest Neighbours.
6. ipywdigets
7. imblearn
