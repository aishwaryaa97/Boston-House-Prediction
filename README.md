# Boston-House-Prediction
In this project, we will evaluate the performance and predictive power of a model that has been trained and tested on data collected from homes in suburbs of Boston, Massachusetts. A model trained on this data that is seen as a good fit could then be used to make certain predictions about a home’s monetary value.

The dataset for this project originates from the Kaggle dataset. The Boston housing data was collected in 1978 and each of the 506 entries represent aggregated data about 14 features for homes from various suburbs in Boston, Massachusetts.

## Data Exploration
In this section, we will make a cursory investigation about the Boston housing data.

Since the main goal of this project is to construct a working model which has the capability of predicting the value of houses, we have separated the dataset into features and the target variable. The features, 'RM', 'LSTAT', and 'PTRATIO', give us quantitative information about each data point. The target variable, 'MEDV', will be the variable we seek to predict. These are stored in features and prices, respectively.

To dive a bit deeper int our data, we are using three features from the Boston housing dataset: 'RM', 'LSTAT', and 'PTRATIO'. For each data point (neighborhood):

'RM' is the average number of rooms among homes in the neighborhood.
'LSTAT' is the percentage of homeowners in the neighborhood considered “lower class” (working poor).
'PTRATIO' is the ratio of students to teachers in primary and secondary schools in the neighborhood.
Without building a model, let’s try to figure out if an increase in the value of a feature would lead to an increase in the value of 'MEDV' or a decrease in the value of 'MEDV'.

‘RM’: An increase in the value of this feature will lead to an increase in the value of ‘MEDV’. This is because for you’d expect a home with a higher number of rooms to be more expensive that a home with lower number of rooms.
‘LSTAT’: An increase in the value of this feature will lead to a decrease in the value of ‘MEDV’. A lower class homeowner might not be able to afford expensive houses, so you’d expect them to leave in a cheaper home. A higher percentage of such people could correlate to cheaper homes in an area, and thus, a lower ‘MEDV’ value.
‘PTRATIO’: An increase in the value of this feature will lead to an decrease in the value of ‘MEDV’. A low student to teacher ration is typically associated with better education level of a school, as a teacher is able to focus on individual students better (than if there were more students). So, due to the presence of better quality schools, people might be willing to pay more to live in those areas, to provide their children with better education, and the prices might be higher.
