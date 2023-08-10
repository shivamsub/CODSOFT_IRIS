# IRIS
Data Science Project for Iris Flower Classification

1. Importing Modules
    - We first import the various modules that are required for the project.
    - The pandas module helps us provide structured dataframes to store and maintain datasets.
    - The train_test_split module helps us to split a dataset into training and testing subsets.
    - The RandomForestClassifier helps us create a classification tree for our dataset.
    - The accuracy_score helps us to calculate the accuracy score of the model's predictions.
      
2. Basic Dataset Functions
    - We read the dataset using read_csv function followed by the dataset name.
    - The head() helps us fetch the 1st 5 rows of the dataset.
    - shape helps get the number of rows and columns in a dataset.
    - info() gives us the details of the dataset such as null/non-null values, datatype of column, column names, memory usage etc.
    - The isna() checks if value is null or not and the sum returns the count of null values.
      
3. Data Preprocessing
    - We first encode the categorical data - Species using mapping.
    - We set setosa as 0, versicolor as 1, and virginica as 2.
    - After this we again invoke the head() function to get the new values of the 1st 5 rows after encoding is done.
    - We then create 2 variables named X and Y.
    - X stores all values except the 'Species' column values whereas Y stores the 'Species' column values.
    - We then create the training and testing subset with a test size of 0.2 which means 20% of dataset will be used for training and 80% for testing.
      
4. Training and Evaluating the Model
    - We then create a model that uses Random Forest Classifier as the algorithm for classification.
    - We then fit the training dataset to the model.
    - We then create a variable that stores the prediction of the testing subset.
    - The accuracy score is then used on the testing subset and predicted variable.
      
5. Function for Manual Testing
    - We create a function named classify_iris() which takes the sepal length, width, petal width, length from the user.
    - We then create an array of the data received from the user and store the predicted value in a result variable.
    - If the result is 0 it is classified as setosa, if 1 classified as versicolor, and if it is 2 then it is classified as virginica.
    - We then call the function for execution.
   
