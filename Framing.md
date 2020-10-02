# Framing

Supervised Machine learning -
     ML Systems learn how to combine input to produce useful predictions on never before seen data.
     
     
## Labels
   A __label__ or the -y variable is the thing we are predicting in simple linear regression. The label could be the future price of wheat, the kind of animal shown in a picture, the meaning of an audio clip, or just about anything.
   
## Feature
   A feature is an input variable—the x variable in simple linear regression. A simple machine learning project might use a single feature, while a more sophisticated machine learning project could use millions of features, specified as:

```
                         X1,X2,X3,... Xn
```


In a spam detector the examples for features could be:
* words in the email text
* senders email address
* contains text to click link
* time of the day email was sent


# Examples

An __example__ is a particular instance of data __x__ wher __x__ is a vector. An example could be divided into two types

* labeled example
* unlabeled example

A labeled example includes both feature(s) and label and is used to train a model

```
  labeled examples: {features, label}: (x, y)
```
In the spam detector example an email marked explicitly as spam or not spam is an example for a label

Following example demonstrates a labeled example with 5 labeled examples

| car model <br> feature | no of owners <br> feature| distance covered(mi) <br> feature | price $ <br> label|
| ------------------- | --------------------- | -------------------------- | ------------- |
| 2005 | 1 | 200000 | 65000 |
| 2010 | 2 | 325000 | 45000 |
| 2008 | 1 | 276500 | 42500 |
| 2010 | 1 | 199000 | 25200 |
| 2012 | 3 | 299250 | 55000 |


An __unlabeled__ example contains fetures but no labels, it can be labeled by a trained model on a labeled example

```
unlabeled examples: {features, ?}: (x, ?)
```
Here is an example without the label(price) on the same set of features

| car model <br> feature | no of owners <br> feature| distance covered(mi) <br> feature |
| ------------------- | --------------------- | -------------------------- |
| 2005 | 1 | 200000 |
| 2010 | 2 | 325000 |
| 2008 | 1 | 276500 |

We use the labeled examples to train a model and use it mark the label of an unlabeled example dataset.

# Models

A model defines the relationship between features and label, as an example of spam detector certain features of the email might associate strongly as spam
The two phases of a model are
 * __Training__ means creating or learning the model. That is you show the model labeled example and then gradually derive a relationship between different features and the label.
 * __Inference__ means applying the learning on an unlabeled example. That is you used the trained model to make meaningfuly predictions of (`y).
 
# Regression vs Classification

A __Regression__ model predicts continuous values. For example, regression makes predictions to answer questions like
* What is value of a car in bangalore?
* What is the probability a user will view an ad

A __Classification__ model predicts discrete values. For example, classification makes predictions to answer questions like
* Is the email spam or not
* Is the given image is of a dog/cat/mouse.

 
