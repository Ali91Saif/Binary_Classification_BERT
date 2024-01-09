# Binary_Classification_BERT
Prediction of Classes of Emails, if  it is spam or not. Used Pre-Trained BERT Transformer Model for class prediction.
In this Project, I am going to perform FineTuning the Pre-Trained BERT Transformer from Hugging-face library and implementing it into Binary Class Classification Problem.

DataFrame Consists of 5572 data Instances (ROWS) accross 2 COLUMNS [Text, label].
Data contains Emails and the classes in which they belongs.
Cloumn Named label contains Binary values, label = 1 signifies that perticular email is a spam,
and label = 0 signifies that the perticular email is not-spam.

label data is heavily imbalanced,containd around 85% data instances belonging to class = 0 [NOT - SPAM].
However, around 15% of Data instances belong to class = 1 [SPAM].
I have used the method 'Compute_Class_Weights' from sklearn library for balancing the  classes.

Data set is splitted into training set and validation set, and this validation set is further sub-devided
into test set.

Loss_Function used is 'Cross_Entropy'
Optimizer used is 'AdamW'
learning_rate is kept at 1e-3
Number_of_Epochs is set to 10

Model_Performance:
1) Precision for Class=0 is ----- 99%
2) Precision for Class=1 is-----  88%

3) Recall  for Class=0 is-----  98%
4) Recall  for Class=1 is-----  92%

5) Model Accuracy is 97%
