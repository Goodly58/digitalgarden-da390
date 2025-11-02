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
> ![image-56.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-56.png)
> ![image-52.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-52.png)

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

> [!success]- Solution
> ![image-57.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-57.png)
> ![image-53.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-53.png)

![image-36.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-36.png)

![image-58.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-58.png)

> [!success]- Solution
> ![image-59.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-59.png)
> ![image-54.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-54.png)

### Midterm 2020

**Question 1. Decision Tree Overfitting**

[6 points] Consider the training and testing error curves plotted in the figure below, during decision tree learning, as the number of nodes in the decision tree grows. Please answer each of the questions below, and explain/justify your answer **briefly** **in 1 or 2 sentences.**

![image-39.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-39.png)

a. Given the above plot of training and testing error, is the decision tree overfitted when the size of the decision tree is 15 nodes? Explain why or why not?

> [!success]- Solution
> Yes, because it having more errors than when the tree size was 7,8,9,10, while the training data's error rate is lowering (this divergence signals overfitting). While it is not as overfitted as when it approaches 20,21, it still shows a significant degree of overfitting.

b. Given the above plot of training and testing error, what is the ideal number of nodes to use to classify future examples? Why?

> [!success]- Solution
> b) The ideal would be likely be 10 as it has the lowest overfitting and best performance for testing set (which is the dataset that matters more).

c. Is decision trees classifier a parametric or non-parametric method? Why?

> [!success]- Solution
> Non-parametric, because it doesn't have a fixed form (like linear y=mx+b)


**Question 4. Evaluation Measures _(7 points)_**

A team from AUS proposed a method to predict whether an email is Spam or Not Spam. They trained the model on email messages from AUS email. After training the model, they used a dataset of 1000 new emails (also labeled) to test the model. Their model produced the following confusion matrix:

|                    | **Predicted: Spam** | **Predicted: Not Spam** |
| ------------------ | ------------------- | ----------------------- |
| **True: Spam**     | 140                 | 40                      |
| **True: Not Spam** | 160                 | 660                     |

**a.** Compute the **accuracy** of this model.
**b.** In this particular case, do you think that **accuracy is a good measure** of predicting Spam or Not Spam email? Why or why not? _(briefly justify your answer)_
**c.** Compute the **precision and recall** of this model in predicting **Spam** emails.
**d.** What type of users would this classifier more likely **satisfy**? Why? _(briefly justify your answer)_

> [!success]- Solution  
> ![image-61.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-61.png)


**Overfitting:** Increase, decrease, or no effect:
![image-40.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-40.png)

> [!success]- Solution
> ![image-62.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-62.png)



**Question 2. Classification using KNN**

[6 points] As you know, KNN classifier assigns a test sample the majority class associated with its K nearest training instances. Suppose we have the following training set of positive (+) and negative (-) samples and a single test sample (o). All samples have two real-valued features (X and Y). Euclidean distance is considered to measure the distance between samples. Assume that we are using the majority “unweighted” KNN (every nearest neighbor contributes equally to the final majority vote). Answer the following questions:

a. What would be the class assigned to this test sample for K=1  

b. What would be the class assigned to this test sample for K=5

c. If the data you have contains noise samples, which of the following options would you consider in KNN to get better predictions? and Why? (briefly justify your answer in 1 or 2 sentences)  
A) increase the value of k  
B) decrease the value of k  
C) noise cannot affect the value of k  
D) none of these  
Reason?

d. Given this particular training dataset, would you recommend setting K = 11 or more? Why or why not? (briefly justify your answer in 1 or 2 sentences)


![image-63.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-63.png)

> [!success]- Solution
> ![image-64.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-64.png)