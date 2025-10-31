---
{"dg-publish":true,"permalink":"/3-machine-learning-notes/quiz-1-intro-to-ml/","tags":["quiz","machine-learning","data-mining"]}
---

Quiz 1: https://tkbs.netlify.app/3-machine-learning-notes/quiz-1-intro-to-ml/
Quiz 2: https://tkbs.netlify.app/3-machine-learning-notes/quiz-2-data/
Quiz 3: https://tkbs.netlify.app/3-machine-learning-notes/quiz-3-kn-ns/

---
# Section 03

## Question 1
**Fill in the blank:**
In clustering, the goal is to group data points into groups based on **\_\_\_\_\_**.

> [!success]- Solution
> similarity

---

## Question 2
**True/False:**
Semi-supervised learning is particularly useful when labeled data is abundant, but unlabeled data is rare.

- [ ] True
- [ ] False

> [!success]- Solution
> False

---

## Question 3
**Multiple Choice:**
Which of the following is true:

- [ ] Artificial Intelligence is broader than Machine Learning
- [ ] Deep Learning is a subset of Machine Learning
- [ ] Deep Learning eliminates the need for feature extraction in many cases
- [ ] All the above
- [ ] None of the above

> [!success]- Solution
> All the above

---

## Question 4
**Fill in the blank:**
Linear regression fits a **\_\_\_\_\_** to the data to predict continuous outcomes.

> [!success]- Solution
> straight line

---

## Question 5
**Multiple Choice:**
*Determine whether this is a ML/DM task and identify the type:*

Estimating the number of likes or shares a post will get based on features like text content, hashtags, posting time, and user engagement history.

- [ ] Clustering
- [ ] Classification
- [ ] Regression
- [ ] Association Rule Mining
- [ ] Not a machine learning or data mining task

> [!success]- Solution
> Regression

---

## Question 6
**Multiple Choice:**
*Determine whether this is a ML/DM task and identify the type:*

Classify students into several groups based on their study habits that they reported to the instructor by answering a survey at the beginning of the semester.

- [ ] Clustering
- [ ] Classification
- [ ] Regression
- [ ] Association Rule Mining
- [ ] Not a machine learning or data mining task

> [!success]- Solution
> Clustering

---

## Question 7
**Multiple Choice:**
*Determine whether this is a ML/DM task and identify the type:*

Categorize players based on play style, in-game purchases, and activity patterns to tune challenges or rewards.

- [ ] Clustering
- [ ] Classification
- [ ] Regression
- [ ] Association Rule Mining
- [ ] Not a machine learning or data mining task

> [!success]- Solution
> Clustering

---

## Question 8
**Multiple Choice:**
*Determine whether this is a ML/DM task and identify the type:*

Predicting the outcome of tossing a coin.

- [ ] Clustering
- [ ] Classification
- [ ] Regression
- [ ] Association Rule Mining
- [ ] Not a machine learning or data mining task

> [!success]- Solution
> Not a machine learning or data mining task

---

## Question 9
**Multiple Choice:**
*Determine whether this is a ML/DM task and identify the type:*

Predicting a patient's cholesterol level in the next check-up based on diet, medication, and exercise history.

- [ ] Clustering
- [ ] Classification
- [ ] Regression
- [ ] Association Rule Mining
- [ ] Not a machine learning or data mining task

> [!success]- Solution
> Regression

---

## Question 10
**Multiple Choice:**
*Determine whether this is a ML/DM task and identify the type:*

Identifying which Data Science-related courses students often enroll in right after completing "Python for Beginners" course.

- [ ] Clustering
- [ ] Classification
- [ ] Regression
- [ ] Association Rule Mining
- [ ] Not a machine learning or data mining task

> [!success]- Solution
> Association Rule Mining


---


# Section 01

---

### **Q1**

Determine whether the following activity is a machine learning and data mining task or not.  
If it is a machine learning and data mining task, indicate if it uses classification, regression, clustering, or association rule mining.

**Grouping students into two groups: females and males, using their student information available on Banner.**

A. Clustering  
B. Classification  
C. Regression  
D. Association Rule Mining  
E. Not a machine learning or data mining task

> [!success]- 💡 **Solution**  
> ✅ Not a machine learning or data mining task
> the gender information is **already explicitly known** (it’s a field in the data). You're simply sorting.

---

### **Q2**

**True/False**  
Semi-supervised learning can be used with regression tasks.

> [!success]- 💡 **Solution**  
> ✅ **True**  
> Suppose you want to predict house prices:
>	- You have 500 houses with known prices (labeled).
>     - You have 5,000 houses with features (size, location, rooms) but no prices (unlabeled).
> A semi-supervised regression model can:
> Use the labeled data to learn the mapping,
> Use the unlabeled data to better understand the structure or distribution of the input space.

---

### **Q3**

Which of the following is true:

A. Machine Learning is broader than Artificial Intelligence.  
B. Deep Learning is a subset of Machine Learning.  
C. Artificial Intelligence is a subset of Deep Learning.  
D. Data Mining and Machine Learning are identical.  
E. All the above.

> [!success]- 💡 **Solution**  
> ✅ **B. Deep Learning is a subset of Machine Learning.**  
> Deep learning is a specific type of machine learning based on neural networks.

---

### **Q4**

Fill in the blank:  
In \_\_\_\_\_\_\_ learning, the training data includes both inputs and known outputs.

> [!success]- 💡 **Solution**  
> ✅ **Supervised**  
> Because supervised learning uses labeled data with both input features and target outputs.

---

### **Q5**

**True/False**  
Semi-supervised learning is particularly useful when labeled data is abundant, but unlabeled data is rare.

> [!success]- 💡 **Solution**  
> ❌ **False**  
> Semi-supervised learning is useful when **labeled data is scarce** but **unlabeled data is abundant**.

---

### **Q6**

Determine whether the following activity is a machine learning and data mining task or not.  
If it is a machine learning and data mining task, indicate if it uses classification, regression, clustering, or association rule mining.

**Grouping those who are satisfied with a purchase based on their reviews.**

A. Clustering  
B. Classification  
C. Regression  
D. Association Rule Mining  
E. Not a machine learning or data mining task

> [!success]- 💡 **Solution**  
> ✅ **Classification**  
> Because satisfaction (“satisfied” vs. “not satisfied”) is a **labeled** category → a supervised classification task.

---

### **Q7**

Determine whether the following activity is a machine learning and data mining task or not.  
If it is a machine learning and data mining task, indicate if it uses classification, regression, clustering, or association rule mining.

**Monitoring the level of vibration and temperature of a machine and predicting if the machine will fail or not.**

A. Clustering  
B. Classification  
C. Regression  
D. Association Rule Mining  
E. Not a machine learning or data mining task

> [!success]- 💡 **Solution**  
> ✅ **Classification**  
> Because the output (“fail” or “not fail”) is a **binary label**, so it’s a **classification problem**, not regression.

---

### **Q8**

Determine whether the following activity is a machine learning and data mining task or not.  
If it is a machine learning and data mining task, indicate if it uses classification, regression, clustering, or association rule mining.

**Grouping customers based on their purchasing patterns.**

A. Clustering  
B. Classification  
C. Regression  
D. Association Rule Mining  
E. Not a machine learning or data mining task

> [!success]- 💡 **Solution**  
> ✅ **Clustering**  
> Because we’re discovering natural **groups** in unlabeled data → **unsupervised learning**.

---

### **Q9**

Determine whether the following activity is a machine learning and data mining task or not.  
If it is a machine learning and data mining task, indicate if it uses classification, regression, clustering, or association rule mining.

**Identifying which courses students often enroll in together to improve course offering planning.**

A. Clustering  
B. Classification  
C. Regression  
D. Association Rule Mining  
E. Not a machine learning or data mining task

> [!success]- 💡 **Solution**  
> ✅ **Association Rule Mining**  
> Because this discovers **relationships** or **co-occurrence patterns** between items (like “students who take X often take Y”).

---

### **Q10**

Determine whether the following activity is a machine learning and data mining task or not.  
If it is a machine learning and data mining task, indicate if it uses classification, regression, clustering, or association rule mining.

**Estimating a future’s value of a building based on information about other buildings in the area.**

A. Clustering  
B. Classification  
C. Regression  
D. Association Rule Mining  
E. Not a machine learning or data mining task

> [!success]- 💡 **Solution**  
> ✅ **Regression**  
> Because the goal is to predict a **continuous numeric value** (building price/value).

---

# Section 2

---

### **Question 1**

**Multiple Choice**  
Which of the following is true:
- Machine Learning is broader than Artificial Intelligence
- Machine Learning is a subset of Deep Learning
- Artificial Intelligence (AI) only refers to robots that mimic human behavior
- Data Mining and Machine Learning are identical
- All the above
    

> [!success]- Solution  
> None of the above

---

### **Question 2**

**Fill in the Blank**  
Fill in the blank:  
In \_\_\_\_\_\_\_\_\_\_\_\_\_ learning, the training data includes input data without labels.

> [!success]- Solution  
> unsupervised

---

### **Question 3**

**Multiple Choice**  
Classify students into several groups based on their available GPA.

- Classification
- Regression
- Clustering
- Association Rule Mining
- Not a machine learning or data mining task
    

> [!success]- Solution  
> Clustering

---

### **Question 4**

**True/False**  
Association rule mining can be considered a supervised learning method.

> [!success]- Solution  
> False

---

### **Question 5**

**Multiple Choice**  
Categorize households based on energy usage patterns to identify typical consumption behaviors.

- Classification
    
- Regression
    
- Clustering
    
- Association Rule Mining
    
- Not a machine learning or data mining task
    

> [!success]- Solution  
> Clustering

---

### **Question 6**

**Multiple Choice**  
Predicting if a student taking CMP 466 will pass or fail based on their grades.

- Clustering
    
- Classification
    
- Regression
    
- Association Rule Mining
    
- Not a machine learning or data mining task
    

> [!success]- Solution  
> Classification

---

### **Question 7**

**Multiple Choice**  
Identifying which Data Science-related courses students often enroll in right after completing "Python for Beginners" course.

- Clustering
    
- Classification
    
- Regression
    
- Association Rule Mining
    
- Not a machine learning or data mining task
    

> [!success]- Solution  
> Association Rule Mining

---

### **Question 8**

**Multiple Choice**  
Predicting a patient’s cholesterol level in the next check-up based on diet, medication, and exercise history.

- Clustering
    
- Classification
    
- Regression
    
- Association Rule Mining
    
- Not a machine learning or data mining task
    

> [!success]- Solution  
> Regression

---

### **Question 9**

**True/False**  
Semi-supervised learning is particularly useful when unlabeled data is abundant, but labeled data is rare.

> [!success]- Solution  
> True

---

### **Question 10**

**Multiple Choice**  
Predicting if a comment is positive, negative, or neutral.

- Clustering
    
- Classification
    
- Regression
    
- Association Rule Mining
    
- Not a machine learning or data mining task
    

> [!success]- Solution  
> Classification

---
