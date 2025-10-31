---
{"dg-publish":true,"permalink":"/3-machine-learning-notes/quiz-2-data/"}
---

# Section 03


### **Question 1**

What would be the resulting array after running the following code?

```python
#Impute:
import numpy as np
from sklearn.impute import SimpleImputer

#Create the object
imp = SimpleImputer(missing_values=np.nan, strategy='constant', fill_value=0)
X = [[np.nan, 8],
     [4, np.nan],
     [6, 10]]
X_new = imp.fit_transform(X)
X_new
```

**Option A**
```
[[ 5.,  8.],
 [ 4.,  9.],
 [ 6., 10.]]
```

**Option B**
```
[[ 0.,  8.],
 [ 4.,  0.],
 [ 6., 10.]]
```

**Option C**
```
[[ 4.,  8.],
 [ 4.,  8.],
 [ 6., 10.]]
```

**Option D**
```
[[nan, 8], 
 [4, nan], 
 [6, 10]]
```

>[!success]- Solution
>![image-1.png|325x414](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-1.png)


***
### **Question 2**

What would be the resulting array after running the following code?

```python
#Discretization
from sklearn.preprocessing import KBinsDiscretizer

X = [[1, 4],
     [2, 3],
     [5, 2],
     [6, 1]]

est = KBinsDiscretizer(n_bins=2, encode='ordinal', strategy='quantile')
est.fit(X)
Xt = est.transform(X)
Xt
```

**Option A**
```
[[1., 1.],
 [1., 1.],
 [0., 0.],
 [0., 0.]]
```

**Option B**
```
[[0., 0.],
 [0., 0.],
 [1., 1.],
 [1., 1.]]
```

**Option C**
```
[[0., 1.],
 [0., 1.],
 [1., 0.],
 [1., 0.]]
```

**Option D**
```
[[1., 1.],
 [0., 1.],
 [1., 0.],
 [0., 0.]]
```

> [!success]- Solution
> uniform: divide range into bins
> quantile: equal width bins
> kmeans: cluster centers (each bin = values nearest to centroid)
> ![image-29.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-29.png)
> ![image-2.png|402x579](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-2.png)

---
### **Question 3: Scaling**

You provided the following code and formula and asked for the resulting array.

**Code:**
```python
from sklearn.preprocessing import MinMaxScaler, StandardScaler
import numpy as np

X = np.array([[ 10., 25.],
              [ 10., -25.],
              [ 20, 0]])

min_max_scaler = MinMaxScaler()
X_new = min_max_scaler.fit_transform(X)
X_new
```

**Formula:**
$$X_{\text{scaled}} = \frac{X - X_{\text{min}}}{X_{\text{max}} - X_{\text{min}}} $$

**Question:** What is the resulting `X_new` array?

> [!success]- Solution
> ![image-3.png|377x376](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-3.png)

***

### **Question 4: Data Aggregation**

You provided the following dataset and asked to show the table after aggregation.

**Original Data:**
<table>
  <thead>
    <tr>
      <th>Student_ID</th>
      <th>School</th>
      <th>Subject</th>
      <th>Term</th>
      <th>Score</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>S001</td><td>School A</td><td>Math</td><td>Term 1</td><td>78</td></tr>
    <tr><td>S001</td><td>School A</td><td>Science</td><td>Term 2</td><td>81</td></tr>
    <tr><td>S001</td><td>School A</td><td>Math</td><td>Term 3</td><td>84</td></tr>
    <tr><td>S002</td><td>School A</td><td>Science</td><td>Term 1</td><td>65</td></tr>
    <tr><td>S002</td><td>School A</td><td>Math</td><td>Term 2</td><td>70</td></tr>
    <tr><td>S002</td><td>School A</td><td>Science</td><td>Term 3</td><td>75</td></tr>
    <tr><td>S003</td><td>School B</td><td>Math</td><td>Term 1</td><td>90</td></tr>
    <tr><td>S003</td><td>School B</td><td>Science</td><td>Term 2</td><td>92</td></tr>
    <tr><td>S003</td><td>School B</td><td>Math</td><td>Term 3</td><td>94</td></tr>
  </tbody>
</table>


**Task:** Aggregate scores per student across the three terms to compute the **average annual score for each subject**.

**Question:** Show how the table would look after this aggregation.

>[!success]- Solution
>![image-4.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-4.png)

***
### **Question 5: Encoding**

You provided the following code and multiple-choice options and asked for the resulting array.

**Code:**
```python
#Encoding
import numpy as np
from sklearn.preprocessing import OrdinalEncoder

#Create the object
enc = OrdinalEncoder()

X1 = [['Male', 'Satisfied', 'CMP466'], ['Female', 'Very Satisfied', 'CMP340']]
X2 = [['Female', 'Very Satisfied', 'CMP466'], ['Male', 'Very Satisfied', 'CMP466']]

enc.fit(X1)
enc.fit_transform(X2)
```

**Options:**
*   **Option A:** `[[0., 1., 0.], [1., 0., 1.]]`
*   **Option B:** `[[0., 0., 0.], [1., 0., 0.]]`
*   **Option C:** `[[1., 0., 0.], [0., 0., 0.]]`
*   **Option D:** `[[1., 0., 1.], [0., 1., 0.]]`

**Question:** What would be the resulting array after running the code?

>[!success]- Solution
>![image-5.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-5.png)


---


# Section 02

### **Q1**

Consider the following matrix representing a feature **"Age"** with the values of 4 observations.  
Apply **Min-Max Scaling** to the feature, where the minimum value will be scaled to 0 and the maximum to 1.

Formula:   
$$X_{scaled} = \frac{X - X_{min}}{X_{max} - X_{min}}$$

| Observation | Age |
| ----------- | --- |
| 1           | 25  |
| 2           | 30  |
| 3           | 40  |
| 4           | 50  |

What is the Min-Max-scaled version of this matrix?

> [!success]- 💡 **Solution**  
> ✅ **Scaled Age values:**
> 
|Observation|Scaled Age|Fraction|
|---|---|---|
|1|0.0||
|2|0.2|1/5|
|3|0.6|3/5|
|4|1.0||
> 
> **Reasoning:**  
> $X_{min}=25,\ X_{max}=50$  

---

### **Q2**

Consider the following matrix representing a categorical feature **"Customer Satisfaction"** with five possible values:  
“Very Unsatisfied”, “Unsatisfied”, “Neutral”, “Satisfied”, “Very Satisfied”.

This feature is **ordinal**, meaning categories have a natural ranking.  
Encoding scheme:

- Very Unsatisfied = 1
- Unsatisfied = 2
- Neutral = 3
- Satisfied = 4
- Very Satisfied = 5

|Observation|Customer Satisfaction|
|---|---|
|1|Neutral|
|2|Very Satisfied|
|3|Unsatisfied|
|4|Satisfied|
|5|Very Unsatisfied|
|6|Neutral|
|7|Satisfied|

What is the **ordinal encoded version** of this matrix?

> [!success]- 💡 **Solution**  
> ✅ **Encoded values:**
> 
> |Observation|Encoded Satisfaction|
> |---|---|
> |1|3|
> |2|5|
> |3|2|
> |4|4|
> |5|1|
> |6|3|
> |7|4|

---

### **Q3**

State the **type of the attribute** as categorical, numerical, or unstructured.  
Then specify:
- If categorical, specify if it is nominal or ordinal
- If numerical, specify if it is interval or ratio
- If unstructured, specify if it is text, images, etc.

Example: Age in years → **numerical (ratio)**

| Attribute                                                             | Type |
| --------------------------------------------------------------------- | ---- |
| Airline (e.g., Emirates, Qatar Airways)                               | ?    |
| Rural-Urban Code (Completely rural, mostly rural, urban center, etc.) | ?    |
| Post on LinkedIn                                                      | ?    |
| Bank Account Balance                                                  | ?    |

> [!success]- 💡 **Solution**  
> ✅ Correct classifications:
> 
> |Attribute|Type|
> |---|---|
> |Airline|**Categorical (nominal)**|
> |Rural-Urban Code|**Categorical (ordinal)**|
> |Post on LinkedIn|**Unstructured (text, images, and/or videos)**|
> |Bank Account Balance|**Numerical (ratio)**|
> 
> **Explanation:**
> 
> - _Nominal_ → no inherent order (Airline names).
>     
> - _Ordinal_ → ranked categories (rural → urban).
>     
> - _Unstructured_ → text/media data.
>     
> - _Ratio_ → numeric values with a true zero (money, weight, etc.).
>     

---

### **Q4**

Consider the following matrix representing a categorical feature **"Color"** with values “Red”, “Blue”, and “Green.”  
What is the **one-hot encoded** version?

|Observation|Color|
|---|---|
|1|Red|
|2|Blue|
|3|Green|
|4|Red|
|5|Blue|

> [!success]- 💡 **Solution**  
> ✅ **One-Hot Encoded Matrix**
> 
> |Observation|Red|Blue|Green|
> |---|---|---|---|
> |1|1|0|0|
> |2|0|1|0|
> |3|0|0|1|
> |4|1|0|0|
> |5|0|1|0|
> 
> **Explanation:**  
> Each unique category gets its own binary column (1 = present, 0 = absent).

---

# Section 1

---

## **Quiz 2**

---

### **Question 1**

**Multiple Choice**  
What would be the resulting array after running the following code:

```python
# Encoding
import numpy as np
# Import the class
from sklearn.preprocessing import OneHotEncoder
# Create the object
enc = OneHotEncoder()
X1 = [['Male', 'Blue Eyes', 'L'], ['Female', 'Grey Eyes', 'XL']]
X2 = [['Female', 'Grey Eyes', 'XL'], ['Male', 'Blue Eyes', 'L']]
enc.fit(X1)
enc.fit_transform(X2).toarray()
```

Options:

```
[[1., 0., 0., 1., 0., 1.],
 [1., 0., 0., 1., 0., 1.]]
[[1., 0., 0., 1., 0., 1.],
 [0., 1., 1., 0., 0., 1.]]
[[1., 0., 0., 1., 0., 1.],
 [0., 1., 1., 0., 1., 0.]]
[[0., 1., 1., 0., 1., 0.],
 [1., 0., 0., 1., 0., 1.]]
```

> [!success]- Solution
> 
> ```python
> [[1., 0., 0., 1., 0., 1.],
>  [0., 1., 1., 0., 1., 0.]]
> ```

---

### **Question 2**

**Multiple Choice**  
What would be the resulting array after running the following code:

```python
# Impute
import numpy as np
# Import the class
from sklearn.impute import SimpleImputer
# Create the object
imp = SimpleImputer(missing_values=np.nan, strategy='mean', fill_value=0)
X = [[np.nan, 8],
     [4, np.nan],
     [6, 10]]
X_new = imp.fit_transform(X)
X_new
```

Options:

```
[[nan, 8],
 [4, nan],
 [6, 10]]
[[ 0., 8.],
 [ 4., 0.],
 [ 6., 10.]]
[[ 4., 8.],
 [ 4., 8.],
 [ 6., 10.]]
[[ 5., 8.],
 [ 4., 9.],
 [ 6., 10.]]
```

> [!success]- Solution
> 
> ```python
> [[ 5., 8.],
>  [ 4., 9.],
>  [ 6., 10.]]
> ```

---

### **Question 3**

**Fill in the Blank**  
The formula for **Min-Max Scaling** is:

Where:

- ( x ) is the original value
    
- ( x_{min} ) is the minimum value of the feature
    
- ( x_{max} ) is the maximum value of the feature
    

The resulting array is: `[[0.444, 0], [0, 0.5], [1, 1]]`

> [!success]- Solution  
> `[[0.4, 0.], [0., 0.5], [1., 1.]]`

---

### **Question 4**

**Multiple Choice**  
What would be the resulting array after running the following code:

```python
# Discretization
from sklearn.preprocessing import KBinsDiscretizer
X = [[1, 1],
     [5, 2],
     [2, 3],
     [6, 4]]
est = KBinsDiscretizer(n_bins=2, encode='ordinal', strategy='quantile')
est.fit(X)
Xt = est.transform(X)
Xt
```

Options:

```
[[1., 0.],
 [1., 0.],
 [0., 1.],
 [0., 1.]]
[[0., 0.],
 [1., 0.],
 [0., 1.],
 [1., 1.]]
[[1., 0.],
 [0., 0.],
 [1., 1.],
 [0., 1.]]
[[0., 0.],
 [0., 0.],
 [1., 1.],
 [1., 1.]]
```

> [!success]- Solution
> 
> ```python
> [[0., 0.],
>  [1., 0.],
>  [0., 1.],
>  [1., 1.]]
> ```

---

### **Question 5**

**Essay**  
You are working with a dataset containing daily sales data from 100 retail stores across multiple cities in the UAE.  
The dataset contains the following attributes:

|Date|Store_ID|City|Product_ID|Units_Sold|Revenue (AED)|
|---|---|---|---|---|---|
|2023-Jan-01|101|Dubai|A123|10|150.00|
|2023-Feb-02|101|Dubai|B234|5|80.00|
|2023-Jan-01|102|Abu Dhabi|B234|12|180.00|
|2023-Jan-03|102|Abu Dhabi|A123|6|90.00|
|2023-Aug-01|103|Sharjah|C345|7|105.00|
|2023-July-04|103|Sharjah|B234|5|75.00|

You are asked to **aggregate the dataset to reduce granularity** and prepare it for higher-level trend analysis.  
**Task:**
- Group by `Store_ID` and the **month** extracted from `Date`.
- Compute total `Units_Sold` and total `Revenue` for each store per month.
- Show how the data would look after aggregation.
    

> [!success]- Solution  
> **Aggregated Table:**
> 
> |Month|Store_ID|Units_Sold|Revenue (AED)|
> |---|---|---|---|
> |2023-Jan|101|10|150|
> |2023-Feb|101|5|80|
> |2023-Jan|102|18|270|
> |2023-Aug|103|7|105|
> |2023-July|103|5|75|

---