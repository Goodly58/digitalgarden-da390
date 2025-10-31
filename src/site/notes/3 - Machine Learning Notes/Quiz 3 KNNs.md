---
{"dg-publish":true,"permalink":"/3-machine-learning-notes/quiz-3-kn-ns/"}
---

# Section 01

### **Question 1**

We are using the K-Nearest Neighbors (**KNN**) algorithm for a **regression** task.  
The dataset consists of two features `X1` and `X2` and a target variable `Y`:

|X1|X2|Y|
|:-:|:-:|:-:|
|5|7|8|
|3.3|2|6|
|6|4.5|7.5|

We are given a new query point:  
Q = (3, 4)  

We are using:
- (k = 2) (two nearest neighbors)
- **Manhattan distance (L1)**
- **Arithmetic mean** as the aggregation function

**Question:**  
The predicted target value for the query point (Q) using the KNN regression method is **\_\_\_\_\_\_\_\_\_\_**


> [!success]- Solution  
> 
| Attribute Differences              | Target |     |
| ---------------------------------- | ------ | --- |
| $\sqrt{\|(5-3)+(7-4)\|}$ = √5      | 8      |     |
| $\sqrt{\|(3.3-3)+(2-4)\|}$ = √ 1.7 | 6      | ✔   |
| $\sqrt{\|(6-3)+(4.5-4)\|}$ = √ 3.5 | 7.5    | ✔   |
(6+7.5)/2
= 6.75


---

### **Question 2**

Given a large dataset with 60 000 samples, assume a KNN classifier is used with different values of _k_.  
When making a prediction for a test sample, how does the time taken to calculate distances compare when using _k = 100_ versus _k = 1000_?

(a) None of the options is correct  
(b) The time taken with k = 100 is less than with k = 1000  
(c) The time taken with k = 1000 is less than with k = 100  
(d) The time taken with k = 100 is about the same as with k = 1000

> [!success]- Solution  
> The most time-consuming part is computing distances between test sample and every training sample. Both have same time complexity O(N × d)
> 	- N = # of training samples
> 	- d = # of features
> 
> **(d) The time taken with k = 100 is about the same as with k = 1000**

---

### **Question 3**

In KNN, when you use a bigger value of _k_, how does it impact the decision boundaries of the classifier?

(a) The decision boundaries become more complex and overfit the training data  
(b) The decision boundaries remain unchanged regardless of the value of k  
(c) The decision boundaries become smoother

> [!success]- Solution  
> **(c) The decision boundaries become smoother**
> This is because it overcomes the noise/outliers

---

### **Question 4**

Consider the following training set of samples.  
All samples have two real-valued features (`X1`, `X2`).  
Euclidean distance is used to measure the distance between samples.  
We are using **basic unweighted KNN**, where each nearest neighbor contributes equally to the final majority vote.

![image-19.png|94x147](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-19.png)

Given this training dataset (shown in the figure above), we want to evaluate different positive, nonzero integer values of k to find the optimal value that maximizes model performance.

**Question:**  
Which of the following represents a useful range of _k_ values to iterate through?

(a) k ∈ [6, 17] only  
(b) k ∈ [6, 23] only  
(c) k ∈ [1, 23] only  
(d) k ∈ [1, 11] only  
(e) k ∈ [1, 6] only  
(f) k ∈ [6, 11] only

> [!success]- Solution  
> **(d) k values in the range [1, 11] only**
> 7,8,9,10,11 can still make star the final majority vote.
> Anything beyond that will always make circle the majority vote.
> When it's 12, best case is 6 stars vs 6 circles → tie (stars can't win)

---

### **Question 5**

Given the following dataset. Assume KNN will be used for **classification**:

|Point|x|y|Class|
|:-:|:-:|:-:|:-:|
|A|1|1|−1|
|B|1|2|−1|
|C|2|2|+1|
|D|8|7|+1|
|E|10|10|+1|

We will run KNN with _k = 3_ and then with _k = 5_.  
Predict the class of the following point Q = (3, 4), assuming **Euclidean distance**.

(a) With k = 3, Q → +1; with k = 5, Q → −1  
(b) With both k = 3 and k = 5, Q → +1  
(c) With both k = 3 and k = 5, Q → −1  
(d) With k = 3, Q → −1; with k = 5, Q → +1

> [!success]- Solution
> 
> | Atts Difference                   | Target | k=3 | k=5 |
> | --------------------------------- | ------ | --- | --- |
> | $\sqrt{(1-3)^2+(1-4)^2}$ = 3.6    | -1     | ✔   | ✔   |
> | $\sqrt{(1-3)^2+(2-4)^2}$ = 2.82   | -1     | ✔   | ✔   |
> | $\sqrt{(2-3)^2+(2-4)^2}$ = 2.24   | +1     | ✔   | ✔   |
> | $\sqrt{(8-3)^2+(7-4)^2}$ = 5.83   | +1     |     | ✔   |
> | $\sqrt{(10-3)^2+(10-4)^2}$ = 9.22 | +1     |     | ✔   |
> **When k=3:** -1 is majority(2v1). So target is -1.
> **When k=5:** 1 is majority (3v2). So target is 1.
> 
> Therefore: **(d) With k = 3, Q → −1; with k = 5, Q → +1**




---


# Section 03


---

### **Q1**

When applying **K-Nearest Neighbors (KNN)** to datasets with very high dimensionality (e.g., 1000+ features), how does increasing dimensionality typically affect the **choice of K**?

A. K should always remain the same regardless of dimensionality.  
B. A smaller K becomes more effective due to sharper distance distinctions.  
C. A larger K is often required because distances between points become less discriminative.  
D. The choice of K has no significant effect as dimensionality increases.

> [!success]- 💡 **Solution**  
> ✅ **C. A larger K is often required because distances between points become less discriminative.**
> 
> **Explanation:**  
> In high-dimensional spaces, all points become similarly distant (“curse of dimensionality”).  
> Larger K smooths out noise and helps generalize better.

---

### **Q2**

Consider the following training set with two features (X1, X2).  
We use basic **unweighted KNN** with Euclidean distance.

If the data contains **noise samples**, which K value adjustment would help improve predictions?

A. Noise cannot affect the value of K  
B. None of the options  
C. Increase the value of K  
D. Decrease the value of K

> [!success]- 💡 **Solution**  
> ✅ **C. Increase the value of K**
> 
> **Explanation:**  
> Higher K reduces sensitivity to random noisy points — the decision boundary becomes smoother and more stable.

---

### **Q3**

When using KNN, if **K = 1**, what is the likely outcome on the model’s performance?

A. The model will underfit because the classifier is too simplistic.  
B. The model is likely to overfit because the classifier will be overly sensitive to the nearest neighbor in the data.  
C. There is no effect of choosing K = 1.  
D. The model will perform well as K = 1 captures fine details.

> [!success]- 💡 **Solution**  
> ✅ **B. The model is likely to overfit because it is overly sensitive to the nearest neighbor.**
> 
> **Explanation:**  
> K=1 memorizes the training data, leading to high variance and poor generalization.

---

### **Q4**

**True/False**  
In KNN, the distance metric used to measure similarity between data points does **not** affect the algorithm’s performance.

> [!success]- 💡 **Solution**  
> ❌ **False**
> 
> **Explanation:**  
> The **distance metric matters** — Euclidean, Manhattan, or cosine distance can yield very different neighbor relationships.

---

### **Q5**

Given the following dataset, assume KNN will be used for classification:

|Point|X|Y|Class|
|---|---|---|---|
|A|1|1|0|
|B|1|2|0|
|C|2|2|1|
|D|10|10|1|

Assume KNN is run for **k = 2** and **k = 3**.  
Predict the class of point **Q = (1.5, 1.5)** (Euclidean distance).

A. With both k=2 and k=3, Q will belong to class 0  
B. With k=2, Q will belong to class 1, and with k=3, Q will belong to class 0  
C. With k=2, Q will belong to class 0, and with k=3, Q will belong to class 1  
D. With both k=2 and k=3, Q will belong to class 1

> [!success]- 💡 **Solution**  
> ✅ **A. With both k=2 and k=3, Q will belong to class 0.**
> 
> **Explanation:**  
> Nearest points A and B (both class 0) dominate votes; D is too far away.  
> So both k=2 and k=3 predict class 0.

---

> [!info]- **Mini Summary:**
>
| Concept           | Small K | Large K |
| ----------------- | ------- | ------- |
| Bias              | Low     | High    |
| Variance          | High    | Low     |
| Decision Boundary | Complex | Smooth  |
| Overfitting Risk  | High    | Low     |
| Robust to Noise   | ❌ No    | ✅ Yes   |

