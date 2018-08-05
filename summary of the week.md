
# weekely summary from chapter one to four


chapter one 


### concept of machine learning
     Machne learning intorduce the concept of learning the data, analyse and then make prediction acconding to dataset can result to the accurancy of prediction 
     
     
   Through algorithms of machine learning we can solve different problems like 
     >failture of students to meet standard mark to pass on year
     >Predict the number of students of high education will get loarn from loarn board 
     many probelms that can be solving by machine learning using supervised learning algorithmns 

#### challenges
  In oder to solve problem by machine learning, must have dataset about our problem and we must know the best model that can be applied  to get accurate result.

#### Applications of machine learning to the realy world
    >Classifications
    ML can classify species into their classes according to the dataset and new data that obtain from the spaces
    
    first analys dataseet by using tools like numpy and pandas then make visuallsion by using matplotlib library
    
    then we build machine learning model in order to predict the accurancy of espected result.
    

#### codes used to build model  
using example of iris datasets


```python
from sklearn.datasets import load_iris
iris_dataset = load_iris()
```

#### Explaintions
   build of machine learning model we must have training sets and test set.
   data will splited into train set and test set .train set used to build model and test set used for make generalition


```python
#before apply algorithmn we must split dataset use the following codes 
#X_train, X_test, y_train, y_test = train_test_split(
#iris_dataset['data'], iris_dataset['target'], random_state=0)
#above code using iris datasets after that we can apply algorithmn of ML
```

#### CHAPTER TWO



##### Supervised Learning


#####  starting with what is Supervised Learning
   is one of types of machine learning that can be used predict a certain
outcome from a given input, this model tkaes input/output pairs to build a model that predict the accurancy of new before seen the data.

#####  two types of supervised learning
    >classification 
    >Regresssion

classification
    can be applied on the non-continues data and when predict one answer can not 
predict others on certain problem somtime call binary classification
    classification can predict problem where target can be 1 or 0
  

regression
can be applied in continues data. 

####  Supervised machine learning algorithms
    the algorithms that can learn from data and make prediction. there eight algorithms 
       >k-nearest neighbor 
       >linear models
       >naive bayes
       >decision trees
       >random forests
       >gradient boosted decision trees
       >suport vector machines
       >neural network
       


### K-nearest algorithm
 k-nearest neighbors (K-NN) 
   In K-NN generalize to the training point by predict the kth-nearest neighbors points
   this model can be applied for small datasets,good as a  baseline, easy to explain.
k-NN divided into two categories
  >k-NN classificatioon
  
  >k-N regression

##### k-NN classifcataion
  it is simplest version. 
  it using one or more trainig data point to the point we want to  make prediction 
   it have application to the many fields in the world because through
   k-NN we can classfier different kinds of diseases according to their features.
   also we can help to get accurate class of certain animal by classifier ithem into classes
example using sklearn to show methods and library for classification


```python
from sklearn.neighbors import KNeighborsClassifier
dc = KNeighborsClassifier(n_neighbors=5)
```

####  k-N regression
  this algorithm use data inform of waves. Due to that fact it can be term into algorithms which use continue data
    also in this algorithm can predict use only one nearest point or more than one point
    

##### by using only one nearest point


```python

#mglearn.plots.plot_knn_regression(n_neighbors=1)
```

##### by using more than one nearest neighbor point
   mglearn.plots.plot_knn_regression(n_neighbors=3)

#####  k-nearest neighbors algorithm for regression
 The k-nearest neighbors algorithm for regression is implemented in the KNeighbors
Regressor class in scikit-learn. It’s used similarly to KNeighborsClassifier:

    from sklearn.neighbors import KNeighborsRegressor

#### Linear Models

   lnear models learn data and make prediction by using linear function

#####   linear models for regression
  
  the linear function used by this is like this
  
  ŷ = w[0] * x[0] + b
  
 the above function is like linear equstion in school mathematics topic of coordinate
  

#####  types of  linear models for regression
   
   >linear regression
   
   import the linera ragression library to the codes
   
    from sklearn.linear_model import LinearRegression
   
   >ridge regression
   
    Ridge regression is implemented in linear_model.Ridge.
    
  from sklearn.linear_model import RidgeRegression
