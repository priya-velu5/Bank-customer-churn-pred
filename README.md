# Bank-customer-churn-pred

### This project uses ensemble models to predict bank customer churn. We saw that people approaching retirement saw higher churn rates. People with a very low balance and high balance were likely to churn too. 

We used Logistic Regression as the baseline model and compared the ensembles with it. 
### The following methods were used for creating ensembles:
* Bagging
* Boosting
* Stacking 

The ensemble models were aslo tested with different set of features to obtain the best results. A correlation-score based strategy was used to select the features. 
We have performed feature selection by setting a minimum threshold value of the respective attributes with their correlation with the column ‘Exited’(the class variable that indicates customer churn). If the corresponding correlation is greater than the threshold then the attribute will be considered to train the model. 

### Accuracy at different thresholds with logistic regression
![image](https://user-images.githubusercontent.com/55476275/210346278-3d9c3c53-cbdc-4225-a7b2-747c0beaf7cc.png)

### Accuracy at different thresholds with bagged decision tree
![image](https://user-images.githubusercontent.com/55476275/210346458-3f269c22-1ca2-46b5-8a73-019eec8e5075.png)

### Comparison of all models for different thresholds 
![image](https://user-images.githubusercontent.com/55476275/210346492-63333c91-4a5a-43c9-bede-a18d17fd2e4e.png)

