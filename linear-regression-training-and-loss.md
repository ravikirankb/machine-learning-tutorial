# Linear Regression

A relationship between two parameters is linear if with the increase of one the other parameter increases linearly. 


Using the equation of a line, the relationship could be written as

                                         
                                          y = mx + b

where:
 * y is the University GPA
 * x is the High school GPA
 * m - slope of the line
 * b is the y - intercept
 
 The convention is slightly different for a machine learning mode:
     
   The same equation is represented as y' = b + w<sub>1</sub>x<sub>1</sub>

   where
   * y' is the predicted label
   * b is the bias, refered as w<sub>0</sub>
   * w<sub>1</sub> is the weight of feature 1, which is the same as slope in traditional linear equation
   * x<sub>1</sub> is a feature or a known input

   To predict the y' university GPA for a new x<sub>1</sub> High school GPA, just substitute the x<sub>1</sub> to the model.

   This model uses only one feature, but a sophisticated model used more than one feature for making an accurate prediction, in such a case the
   equation will look something like this, the following equation uses 3 different features, which could be even more depending on the number of feature set available.

   y' = b + w<sub>1</sub>x<sub>1</sub> + w<sub>2</sub>x<sub>2</sub> + w<sub>3</sub>x<sub>3</sub>
                                        

# Training and Loss

__Training__ a model simply means learning good values for all the weights and bias from labeled examples. In __supervised learning__, a machine learning algorithm builds a model by examining many examples and attempting to find a model that minimizes loss; this process is called __empirical risk minimization__.

Loss is the penalty for a bad prediction. That is, __loss__ is a number indicates how bad the prediction was on a single example. A loss of 0 value indicates a good model, anything above 0 is not an ideal model. The goal is therefore to keep a loss to minimum.

# Squared Loss: a popular loss function

The squared loss for a single example is as follows

```
  = the square of the difference between the label and its prediction
  = (observation - (prediction of x))<super>2</super>
  = (y - y')<super>2</super>
```

__Mean square error(MSE)__ s the average squared loss per example over the whole dataset. To calculate MSE, sum up all the squared losses for individual examples and then divide by the number of examples:

 ```math
    MSE =   1/N \[ \sum_{(x,y)} (y - prediction(x))^2 \]
 ```

where
 * (x,y) is an example in which
    * x is the set of features (for example, chirps/minute, age, gender) that the model uses to make predictions.
    * y is the example's label (for example, temperature).
 * prediction(x) s a function of the weights and bias in combination with the set of features x.
 * D is a data set containing many labeled examples,(x,y) which are  pairs.
 * N is the number of examples in D.
 
 Although MSE is commonly-used in machine learning, it is neither the only practical loss function nor the best loss function for all circumstances.
