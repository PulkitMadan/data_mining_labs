# data_mining_labs
Source code for CSCI 4150: Data Mining Labs at Ontario Tech University


# Tasks 

## Lab 2

### Part I 

- [x] For each continuous attribute, calculate its average, standard deviation, minimum, and maximum values.

- [x] For the discrete attribute, count the frequency for each of its distinct values.

- [x] For each diagram describe your interpretation and insight.

- [x] Draw histogram of the class variable

- [x] Draw the distribution of values for a continuous attribute using a histogram.

- [x] Draw some scatter plots for a couple of attribute pairs.

- [ ] Draw a parallel diagram for some attributes in the data set

### Part II 

- Identify which attributes have missing values and address the issue by: 

- [x] Replacing missing values by the average or mod of the attribute (based on attribute types)

- [x] Replace missing values by the average or mode of the attribute in the particular class to which the instance belongs  

- [x] Draw a histogram of the attribute before and after replacing missing values in the previous step 1 and 2


## Lab 3

### Part I 
- Build a decision tree model and evaluate the model using:

  - Holdout
    - [ ] Use 90% of data set for train and 10 % for the test, and perform it 5 times, the final results are the average of performance trials
    - [ ] You should report the Accuracy, Precision and F-measure for each trial as well as their final average (use a table and then a bar chart)
  - Cross-validation 
    - [ ] Perform 10-fold cross-validation for evaluating the model 
    - [ ] You should report the Accuracy, Precision and F-measure for each trial as well as their final average ((use a table and then a bar chart))


### Part II
- Select the Entropy as the impurity measure and repeat Part I 
- Compare the final Accuracy of cross-validation of Part I and II using some figures 

### Part III
- [ ] Use the holdout method (train: 90 % data set, test: 10 % set) 
    - [ ] Investigate the effect of tree depth on the accuracy of the model (see the tutorial)
      - [ ] Change the tree depth (e.g, 2, 5, 8, ..., 50) and draw training and test accuracy 
      - [ ] Explain your observation 

## Lab 4

### Part I (inference efficiency):

- Build a k-NN model and compare its efficiency with another model:

  - [ ] Perform preprocessing (normalization) if it is necessary
  - [ ] Build k-NN classifier for k = 5:  
    - [ ] Use 90% of data set for the train and 10 % for the test, and perform evaluation 5 times, the final results are the average of trails performance
    - [ ] You should report the final average F-measure, and average test time (the time that model spends to predict labels for the test dataset instances). Use bar charts.
  - [ ] Repeat (2) for building a decision tree classifier (use default parameters). 
  - [ ] Compare results of part (2) and (3) using appropriate charts

### Part II (Model Selection): 
- Perform model selection for the k-NN and decision tree:

  - [ ] Perform preprocessing (normalization) if it is necessary
  - [ ] Build k-NN classifier for different k (1, 2, 3, 4, 5) and select the best k: 
      - [ ] Use 90% of data set for train and 10 % for the test,  and 10% of the train for validation
      - [ ] Build the k-NN model using the train data set and select the best k based on F-measure on the validation set
  - [ ] Build the decision tree model using the train data set and select the best tree:
      - [ ] Change the tree depth (3, 4...10) and calculate F-measure on the validation set
      - [ ] Compare results of part (2) and (3) using the appropriate charts



## Lab 5 

**Note:** In this lab, you have the freedom of choosing different models (at least 3 models), evaluation methodologies  (e.g., cross-validation), performance metrics, and you can perform model selection, before evaluation the model on the test data set. Try your best!

**Instructions:**
- You are working as a data mining scientist, and now you have a case from a dating site. The site has been complained for its terrible recommendations, which simply match the locations and ages. Now, it intends to improve its recommendation system, using data mining techniques. After a survey on the recommendation, the site realizes that a specific customer often categorizes other customers into three types:
    1. People he/she didn’t like;
    2. People he/she liked in small doses;
    3. People he/she liked in large doses.
  
- It also realizes that the following features are highly related to the choices of customers:
    1. Number of frequent flyer miles earned per year;
    2. Percentage of time spent playing video games;
    3. Liters of ice cream consumed per week.


- Finally, you accept the case and the site also passes you the data from its survey.  

**NOTE:** In your report, you should analyze the cases and provide at least three solutions, and validate your solutions. 

- The data (datingData_training/test.txt) contains four columns. Each row contains the information of a specific customer. The first column denotes the number of frequent flyer miles earned per year; the second column indicates the percentage of time spent playing video games; the third column is the liters of ice cream consumed per week. The fourth column indicates the types of people, which is labeled by some other customers. 

