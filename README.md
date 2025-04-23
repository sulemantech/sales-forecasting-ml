# SuperStore Sales
This is a project where I  I want to find :

1. What is the overall trend of the sales?
2. What are the top 10 products by sales?
3. Which is the most performing Segment?
4. What is the most preferred Ship Mode?
5. Which are the most profitable category and Sub-category?
 
And predict my future sales.

### Data Collection: 
This Data is collected from Kaggle Website. (https://www.kaggle.com/rohitsahoo/sales-forecasting)

### Data Exploration and Cleaning:

1. We drop the following columns : 'Row ID', 'Customer Name', 'Country', 'Product Name',Order ID' and 'Customer ID'.
2. Date is converted from character to Date format.
3. For using few of the categorical values , I have used them by implementing onehot_encode technique. 

### Data Visualization and Analysis:
1. We extract the month and year from the date column to independent columns.
2. Investigating and study the trend of the sale and grouping the data to get monthly sales.Sales per month for each year is plotted.
![image](https://user-images.githubusercontent.com/92235451/151744404-073818d0-aa03-41ee-83f8-935704ef1efa.png)

3. Top 10 products getting higher sales.
![image](https://user-images.githubusercontent.com/92235451/151744540-711c648a-30eb-408e-8273-f71c38d8f932.png)

4. Plot most performing segments.

![image](https://user-images.githubusercontent.com/92235451/151744588-332006e7-3171-46a6-8c4d-214aca8cad65.png)

5.Plot most prefered Shipment mode.

![image](https://user-images.githubusercontent.com/92235451/151744761-b48c7897-81be-4d23-8ae6-7a5957a0e6b6.png)

6.Most sold products per state.

![image](https://user-images.githubusercontent.com/92235451/151744820-8bbac1b9-a252-464e-a8a5-3378a8b45d55.png)

7. Most profitable categories and sub categories.

![image](https://user-images.githubusercontent.com/92235451/151744911-ada9413c-39bb-4212-8050-f8d355521366.png)


### Developing Model:
1. Split and scale the dataset into 4 data frame of : X_train, X_test,Y_train, Y_test.
2. We have used 2 Input layers of keras tensor (Neural Network) to train the model and predict the Sales value.


## Results:
The value of prediction is near to the observed value.
The value of coefficient of determination(i.e how much disperse the data is there in our dataset) is greater than 0 , this indicates that the prediction has not failed, but it is not the best. 

# Key Learnings:
1. Keras , one of the efficient library to build and train models.
2. Our model can be improved by increasing the number of neurons that can increase the value of coefficient of determination.
3. Use of Standard Scaler to scale the dataset while building the model.
