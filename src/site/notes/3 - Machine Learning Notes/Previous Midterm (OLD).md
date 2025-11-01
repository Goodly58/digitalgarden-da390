---
{"dg-publish":true,"permalink":"/3-machine-learning-notes/previous-midterm-old/"}
---

### **Midterm 2019**

**Question 1. Introduction**
(8 points) Determine whether or not each of the following activities is a machine learning and data mining task and explain why. Machine learning and data mining tasks include supervised learning, unsupervised learning, and association rules mining.
1. Grouping the customers of a company according to their gender.
2. Computing the total sales of a company.
3. Monitoring the heart rate of a patient and predicting abnormalities.
4. Sorting a student database based on student identification numbers.
5. Predicting the future stock price of a company using historical records.
6. Predicting the outcomes of tossing a (fair) pair of dice.
7. Monitoring seismic waves and predicting earthquake activities.
8. Extracting the frequencies of a sound wave.

> [!success]- Solution
> 1. 

**Question 2. Data**
[7 points] Classify the following attributes as **discrete or continuous**. Also, classify them as **Categorical (nominal or ordinal)** or **Numerical (interval or ratio)**. Some cases may have more than one interpretation, so briefly indicate your reasoning if you think there may be some ambiguity.

_Example:_ Age in years. _Answer:_ Discrete, numerical (ratio)

1. Angles as measured in degrees between 0° and 360°.
2. Bronze, Silver, and Gold medals as awarded at the Olympics.
3. Height above sea level.
4. Number of patients in a hospital.
5. ISBN numbers for books. (Look up the format on the Web.)
6. Ability to pass light in terms of the following values: opaque, translucent, transparent.
7. Bag check number. (When you attend an event, you can often give your bag to someone who, in turn, gives you a number that you can use to claim your bag when you leave.)


![image-36.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-36.png)


### Midterm 2020

**Question 1. Decision Tree Overfitting**

[6 points] Consider the training and testing error curves plotted in the figure below, during decision tree learning, as the number of nodes in the decision tree grows. Please answer each of the questions below, and explain/justify your answer **briefly** **in 1 or 2 sentences.**

![image-39.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-39.png)

a. Given the above plot of training and testing error, is the decision tree overfitted when the size of the decision tree is 15 nodes? Explain why or why not?

> [!success]- Solution
> Overfitted,  because the testing error increases and the decreases on the number of nodes

b. Given the above plot of training and testing error, what is the ideal number of nodes to use to classify future examples? Why?

> [!success]- Solution
> 9, because the testing error and training are the same, and it has the lowest number of nodes therefore, the tree is less complex.

c. Is decision trees classifier a parametric or non-parametric method? Why?

> [!success]- Solution
> Non-parametric, because its not using the max number of nodes


**Question 4. Evaluation Measures _(7 points)_**

A team from AUS proposed a method to predict whether an email is Spam or Not Spam. They trained the model on email messages from AUS email. After training the model, they used a dataset of 1000 new emails (also labeled) to test the model. Their model produced the following confusion matrix:

|                    | **Predicted: Spam** | **Predicted: Not Spam** |
| ------------------ | ------------------- | ----------------------- |
| **True: Spam**     | 140                 | 40                      |
| **True: Not Spam** | 160                 | 660                     |

**a.** Compute the **accuracy** of this model.

> [!success]- Solution  
> Accuracy (=\frac{TP+TN}{N}=\frac{140+660}{1000}=0.80=80%).

**b.** In this particular case, do you think that **accuracy is a good measure** of predicting Spam or Not Spam email? Why or why not? _(briefly justify your answer)_

> [!success]- Solution  
> **No.** The classes are **imbalanced** and accuracy **hides the trade-off** between false positives and false negatives; precision/recall are more informative.

**c.** Compute the **precision and recall** of this model in predicting **Spam** emails.

> [!success]- Solution  
> Precision (=\frac{TP}{TP+FP}=\frac{140}{140+160}=0.4667=46.67%).  
> Recall (=\frac{TP}{TP+FN}=\frac{140}{140+40}=0.7778=77.78%).

**d.** What type of users would this classifier more likely **satisfy**? Why? _(briefly justify your answer)_

> [!success]- Solution  
> Users who **prioritize catching spam** (high **recall**) and **accept more false positives**—i.e., they prefer a cleaner inbox and don’t mind checking the spam folder for mistakenly filtered legitimate emails (low precision).



(???)
![image-38.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-38.png)


---
Increase overfitting, decrease, or no effect:
![image-40.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-40.png)