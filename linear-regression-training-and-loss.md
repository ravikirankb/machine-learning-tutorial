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
                                        
