---
{"dg-publish":true,"permalink":"/3-machine-learning-notes/thani-s-ml-final/"}
---


# Bias-Variance Tradeoff

![image-190.png|Graphs A,B,C|400x92](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-190.png)
Say whether graphs A,B,C are high👆/low👇 in **Bias**, **Variance**, and **Overfitting**.  

> [!success]- Solution
> ![image-221.png|400x219](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-221.png)
> ![image-191.png|400x115](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-191.png)

Draw: 
1. the bias-variance graph
2. Model complexity (x-axis) vs prediction error (y-axis) graph. Mention where the optimal model complexity is. 

BONUS: Finding the point of optimal model complexity is called \_\_\_?

> [!success]- Solution
> ![image-192.png|400x253](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-192.png)
> ![image-222.png|400x284](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-222.png)

![unnamed-10.jpg|400x303](/img/user/3%20-%20Machine%20Learning%20Notes/img/unnamed-10.jpg)
a) Which diagram accurately represents what happens the more you add features? 
b) Draw the point on the part of the graph with the most optimal number of features.

> [!success]- Solution
> ![image-194.png|400x253](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-194.png)

![image-195.png|400x323](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-195.png)
a) What is the error produced on training data (high/low)?
b) What is the error produced on testing data (high/low)?

> [!success]- Solution
> underfit:
> high error in both training data and testing data

**DIMENSIONALITY REDUCTION AND FEATURE SELECTION: INCREASES/REDUCES:**
1. overfitting
2. accuracy
3. training time

> [!success]- Solution
> reduces
> increases
> reduces

![fc55ebe5-1226-4f06-a2bb-5ccd4abeff49.png|400x100](/img/user/3%20-%20Machine%20Learning%20Notes/img/fc55ebe5-1226-4f06-a2bb-5ccd4abeff49.png)

> [!success]- Solution
> - **Number of features in `X_new`:**  
>     10% of 100 = **10 features**.
> - **Criterion:**  
>     It keeps the **top 10% of features with the highest chi-square (χ²) scores** with respect to the target `y` (i.e., features most statistically associated with the class labels).

# Naive Bayes

![image-197.png|400x263](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-197.png)
Why?

> [!success]- Solution
> Conditional independence of attributes is violated.
> 

**True or false**:
- Naïve Bayes is generally easy to implement and efficient to run.
- Naïve Bayes usually performs worse than SVM on text classification tasks with many features.
- Naïve Bayes can handle very large feature spaces.
- In Naïve Bayes, missing attribute values can be handled by simply ignoring that attribute when estimating probabilities.
- Naïve Bayes is robust to isolated noise points and irrelevant attributes.
- A core assumption of Naïve Bayes is that features are conditionally independent given the class.
- When many attributes are highly correlated or redundant, they still perfectly satisfy Naïve Bayes’ conditional independence assumption.
- Naïve Bayes is good at modeling phrases such as “AUS student” as a single combined feature.
- Treating each word independently in Naïve Bayes can cause it to miss important phrase-level meaning (e.g., “AUS student”)
- One weakness of Naïve Bayes is that the independence assumption may not hold for real data, which can hurt accuracy.
- Naïve Bayes can handle redundant attributes
- Naïve Bayes can handle correlated attributes

> [!success]- Solution
> ![image-223.png|400x293](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-223.png)

# Regression I & II

![unnamed-7.jpg|400x218](/img/user/3%20-%20Machine%20Learning%20Notes/img/unnamed-7.jpg)

> [!success]- Solution
> ![image-198.png|400x356](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-198.png)

![a06cb589-114d-4d4a-92a4-2c4ae04a8f2d.jpg|400x218](/img/user/3%20-%20Machine%20Learning%20Notes/img/a06cb589-114d-4d4a-92a4-2c4ae04a8f2d.jpg)
> [!success]- Solution
> ![image-199.png|400x152](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-199.png)

![image-200.png|400x104](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-200.png)
Which model has a lower $R^2$ value? Which has a higher?
> [!success]- Solution
> Model A ⇒ lower $R^2$.
> Model B ⇒ higher $R^2$

![image-201.png|400x124](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-201.png)
![image-224.png|400x219](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-224.png)
Calculate $R^2$
> [!success]- Solution
> ![image-225.png|400x158](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-225.png)

For each metric, specify:
a) **type**: classification or regression?
b) **output type**: discrete or continuous?
c) **purpose**: Which has the goal of evaluating decision boundary? Which is best fit line/curve?
- Accuracy
- $R^2$
- MSE
> [!success]- Solution
> ![image-204.png|400x157](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-204.png)

In gradient descent, what will happen if:
a) you increase $\alpha$
b) you lower $\alpha$
c) set $\alpha$=0?
d) set $\alpha$=1?

> [!success]- Solution
> ![image-203.png|400x246](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-203.png)

Which one works better with many features (>1000)?
- Gradient Descent
- Ordinary Least Squares

> [!success]- Solution
> Gradient Descent

![image-227.png|400x569](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-227.png)

> [!success]- Solution
> ![image-206.png|400x393](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-206.png)
> ![image-207.png|400x397](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-207.png)


![image-208.png|400x188](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-208.png)
Which has a large learning rate ($\alpha$)? What adjustments would you make to that graph?

> [!success]- Solution
> - The learning rate is **too large in Graph B** (the red curve is diverging).
> - To fix it, **decrease α** — e.g. **divide it by 10** so the steps are smaller and J can converge.

![unnamed-8.jpg|400x221](/img/user/3%20-%20Machine%20Learning%20Notes/img/unnamed-8.jpg)
> [!success]- Solution
> ![image-209.png|400x110](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-209.png)
> ![image-210.png|400x177](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-210.png)
> ![image-211.png|400x182](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-211.png)

![unnamed-9.jpg|400x193](/img/user/3%20-%20Machine%20Learning%20Notes/img/unnamed-9.jpg)
> [!success]- Solution
> ![image-213.png|400x88](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-213.png)
> ![image-214.png|400x256](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-214.png)

# Clustering I

Which one should you maximize? which should you minimize?
- intra-cluster distances
- inter-cluster distances
> [!success]- Solution
> minimize
> maximize

![image-215.png|400x258](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-215.png)
Represent as a dendrogram
> [!success]- Solution
> ![image-216.png|400x379](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-216.png)


Answer **“clustering”** or **“not clustering”** 👇
A. Dividing students into registration groups **alphabetically by last name** (A–D, E–H, …).
B. Running a **SQL query** `WHERE major = 'CS'` and looking at the returned CS students.
C. Grouping customers based on their **spending patterns and visit frequency**, with no labels given.
D. Training a **decision tree** to predict whether an email is **spam / not spam** using labeled examples.
E. Using a similarity measure on documents and applying **hierarchical clustering** to group similar articles together.
F. Assigning patients to “high risk / low risk” groups **based on a doctor’s manual rules** (e.g., if age>60 and BP>140 → high risk).
> [!success]- Solution
> 

![image-217.png|400x341](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-217.png)


3D dataset

| Point | x  | y | z |
| ----- | -- | - | - |
| P1    | 0  | 0 | 0 |
| P2    | 0  | 1 | 0 |
| P3    | 5  | 5 | 5 |
| P4    | 6  | 5 | 5 |
| P5    | 10 | 0 | 0 |
| P6    | 10 | 1 | 0 |

Use **bisecting k-means** to partition these 6 points into **K = 3 clusters**:


**Question (multiple can be selected):**  
In which of the following situations is **standard K-means likely to perform poorly** (i.e., this _is_ a problem for K-means)?
A. Clusters have **very different sizes** (one huge cluster, one tiny cluster).
B. Clusters have **very different densities** (one tight, one very spread out).
C. Clusters are **non-globular shapes** (e.g., long moons, concentric rings).
D. The dataset contains **strong outliers** far away from the main groups.
E. Features are on **very different scales** (e.g., one in meters, one in dollars) and you do **not** scale/standardize them.
F. Clusters are **spherical, similar size and density**, data is well-scaled, and there are **no outliers**.
For each option, answer: **“Problem for K-means”** or **“Not a problem for K-means.”**


# Clustering II

A student Hamdan decides to use K-means with K=30. His friend, Thani decides to use K-means with K=3. Who has the higher SSE? Why?
> [!success]- Solution
> The student with the higher SSE is **Thani**. 
> Small k: The clusters are big and loose → High SSE.
> Large k: The clusters are tight and small → Low SSE.

With the same dataset, one method results in scenario A. Another method results in scenario B. Which scenario has a larger SSE?
![image-189.png|400x218](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-189.png)
> [!success]- Solution
> **Scenario A (few clusters):**
> Each centroid has to “cover” a big region → points are, on average, farther from their centroid → larger SSE.
> 
> **Scenario B (many clusters):**
> More centroids, each serving a smaller region → points are closer to their centroid → smaller SSE.

Would DBSCAN work here? why/why not?
![image-220.png|400x182](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-220.png)

> [!success]- Solution
> DBSCAN isn't good with varying densities.

![image-219.png|400x305](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-219.png)
- How many **clusters** DBSCAN will find.
- Which points belong to each cluster.
- Which points are **noise**, if any.