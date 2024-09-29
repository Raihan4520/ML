1. Dataset containing 10,000 samples was loaded from a csv file using pandas builtin function read_csv and stored in a pandas DataFrame. 
2. Shape, size, count of the attributes and rows with null values (NaN) were printed before preprocessing. 
3. Data was preprocessed to remove all rows which contained any null value (NaN) and 'ID' was set as the index column of the DataFrame. 
4. Again shape, size, count of the attributes and rows with null values (NaN) were printed after preprocessing. 
5. All the column names in the DataFrame were printed and from here columns for feature DataFrame were extracted. 
6. Numpy array was created using features columns which was stored in 'X' variable. 
7. Numpy array was created using target column ('Result') which was stored in 'y' variable. 
8. Using Matplotlib Pyplot library a 3D scatter plot of the dataset was plotted for visualization. Where, red point represents covid positive and green point represents covid negative. 
9. To split the data k-fold cross validation was used. 10 folds were used which lead to 1000 data points in each fold. From here 1000 was used for testing and rest of the 9000 was used for training in each iteration. 
10. The model was created using scikit-learn's svm function. 4 different kernels, 'linear', 'poly', 'rbf' and 'sigmoid' and 4 different values of C parameter, 1, 2, 5 and 10 was used to create different models. 
11. All the models were evaluated to get the best model with highest accuracy. 
12. Using 'rbf' kernel and value of C=10 highest accuracy of 94.36% was achieved. 