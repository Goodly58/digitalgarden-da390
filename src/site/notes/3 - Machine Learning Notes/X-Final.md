---
{"dg-publish":true,"permalink":"/3-machine-learning-notes/x-final/"}
---

> [!info]- Exam details
> **Thursday December 4 at 11:00 AM - 1:00 PM**
> 
> The following specific questions will not be asked in the final exam:
> - Apply data preprocessing such as encoding and normalization to a dataset.
> - Construct Decision Trees and make predictions using Decision tree.
> - Make predictions using KNN.
> - Questions on the evaluation of the supervised classification methods (Confusion matrix, precision, recall, etc.).
> - Questions on hyperparameter tuning for decision trees and KNN.

# Midterm

<span class="neon-highlight">KNNs</span>

![image-120.png|200](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-120.png)

1. Calculate Euclidean distance for one record (*without* min-max scaling)
2. Calculate Euclidean distance for one record (*with* min-max scaling)
3. Calculate $gain_{split}$ for Record#
> [!success]- Solution
> ![image-121.png|400x230](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-121.png)

![image-122.png|cosine similarity|400x99](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-122.png)
<span class="neon-highlight">Decision Trees</span>

| **Hyperparameter**          | **Effect of INCREASING the value**                                          | **Result (Risk)** |
| --------------------------- | --------------------------------------------------------------------------- | ----------------- |
| **`max_depth`**             | Allows the tree to grow deeper and more complex.                            | **Overfitting**   |
| **`min_samples_split`**     | Requires _more_ data to allow a split (makes it harder to split).           | **Underfitting**  |
| **`min_samples_leaf`**      | Requires _more_ data to remain in a leaf (prevents small, specific leaves). | **Underfitting**  |
| **`max_leaf_nodes`**        | Allows the tree to have _more_ total terminal nodes (more complexity).      | **Overfitting**   |
| **`min_impurity_decrease`** | Requires a _bigger_ improvement to justify a split (stricter rules).        | **Underfitting**  |
| **`ccp_alpha`**             | Increases the penalty for complexity (prunes more aggressively).            | **Underfitting**  |

<span class="neon-highlight">Model Overfitting</span>

| Type                | Description                           | Training Error | Test Error |
| ------------------- | ------------------------------------- | -------------- | ---------- |
| 🔹 **Underfitting** | Model too simple; fails to generalize | ⬆️ High        | ⬆️ High    |
| 🔸 **Overfitting**  | Model too complex; memorizes data     | ⬇️ Low         | ⬆️ High    
**Pre-pruning**
from hyperparameters → reaching `maxdepth`,`min_impurity_decrease` limit.

**Post-Pruning**
Keep if $\text{err}_{\text{gen}}(\text{after}) < \text{err}_{\text{gen}}(\text{before})$. Otherwise, prune (cut) the split.

![image-123.png|You compare averages across models to help with model selection|400x272](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-123.png)

<span class="neon-highlight">Class Imbalance</span>

| Method            | Description                | Pros                 | Cons                                |
| ----------------- | -------------------------- | -------------------- | ----------------------------------- |
| **Oversampling**  | Replicate minority samples | No info loss         | Risk overfitting (minority repeats) |
| **Undersampling** | Reduce majority samples    | Faster, less storage | Risk info loss                      |
<span class="neon-highlight">Bias Variance Tradeoff</span>

| Model Complexity | Bias        | Variance    | Behavior            |
| ---------------- | ----------- | ----------- | ------------------- |
| Simple model     | 🔺 High     | 🔻 Low      | Underfitting        |
| Complex model    | 🔻 Low      | 🔺 High     | Overfitting         |
| Moderate model   | ⚖️ Balanced | ⚖️ Balanced | Good generalization |

Practice:
Previous Midterm

# Final

![image-141.png|400x202](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-141.png)

**Q1. Answer the following questions using Bayes Theorem.**
(a) Suppose the fraction of undergraduate students who smoke is 15% and the
fraction of graduate students who smoke is 23%. If one-fifth of the college
students are graduate students and the rest are undergraduates, what is the
probability that a student who smokes is a graduate student?

(b) Given the information in part (a), is a randomly chosen college student more
likely to be a graduate or undergraduate student?

(c) Repeat part (b) assuming that the student is a smoker.

(d) Suppose 30% of the graduate students live in a dorm but only 10% of the
undergraduate students live in a dorm. If a student smokes and lives in the
dorm, is he or she more likely to be a graduate or undergraduate student?
You can assume independence between students who live in a dorm and
those who smoke

> [!success]- Solution
> a)
> $\text{P(smoke|undergraduate)}=0.15$
> $P(\text{smoke|graduate})=0.23$
> $P(graduate)=0.2$
> $\text{P(undergraduate)}=0.8$
> 
> $\text{P(smoke)}=0.15\times{}0.8+0.23\times{}0.2=\mathbf{0.166}$
> 
> $\text{P(graduate|smoke)}=\frac{\text{p(smoke|graduate)}\times{}\text{p(graduate)}}{\text{p(smoke)}}=\frac{0.23\times{}0.2}{0.166}=\mathbf{27.7\%}$
> 
> b)
> $P(graduate)=0.2$
> $\text{P(undergraduate)}=0.8$
> 
> Therefore, undergraduate has a higher probability of being selected.
> 
> c)
> $\text{P(undergraduate|smoke)}=\frac{\text{p(smoke|undergraduate)}\times{}\text{p(undergraduate)}}{p(smoke)}=\frac{0.15\times{}0.8}{0.166}=72.3\%$
> 
> More likely to be undergraduate.
> 
> d) 
> $\text{p(dorm|graduate)}=0.3$
> $\text{p(dorm|undergraduate)}=0.1$
> 
> $\text{P(dorm)}=0.3\times{}0.2+0.1\times{}0.8=0.14$
> 
> $\text{p(graduate|smoke,dorm)}=\frac{\text{p(smoke,dorm|graduate)}\times{}\text{p(graduate)}}{\text{p(smoke,dorm)}}=\frac{\text{p(smoke|graduate)}\times{}\text{p(dorm|graduate)}\times{}\text{p(graduate)}}{\text{p(smoke,dorm|grad)}\times{}\text{p(grad)}+\text{p(smoke,dorm|undergrad)}\times{}\text{p(undergrad)}}$
> $=\frac{0.23\times{}0.3\times{}0.2}{(0.23\times{}0.3\times{}0.2)+(0.15\times{}0.1\times{}0.8)}=53.5\%$

![image-144.png|400x330](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-144.png)

> [!success]- Solution
> ![image-145.png|400x238](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-145.png)
> ![image-146.png|400x347](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-146.png)

![image-147.png|400x346](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-147.png)

> [!success]- Solution
> ![image-148.png|400x528](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-148.png)

Q2. Total SSE is the sum of the SSE for each separate attribute. What does it mean if:
a) the SSE for one variable is low for all clusters?
b) Low for just one cluster?
c) High for all clusters?
d) High for just one cluster?
> [!success]- Solution
> ![image-149.png|400x329](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-149.png)

![image-151.png|400x294](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-151.png)
> [!success]- Solution
> ![image-150.png|400x485](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-150.png)


> [!success]- Solution
> ![image-152.png|400x251](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-152.png)
> ![image-153.png|400x303](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-153.png)
> The second algorithm is better because it has a higher SSB (18.18>12.17) and lower SSE (1.833<7.83), which should be maximized and minimized respectively. Higher SSB means there is a bigger distance from the cluster and the global mean (external), and lower SSE means there is less distance between the points and the centroid (internal)

Find textbook problems for concepts that aren't included in the practice problems (based on the formula sheet). Maybe gradient descent

<span class="neon-highlight">Friday</span>
- [[3 - Machine Learning Notes/4. Naive Bayes\|Naive Bayes]]
- [[3 - Machine Learning Notes/4. SVM\|SVM]]
---
<span class="neon-highlight">Saturday</span>
- Regression
- Clustering


<span class="neon-highlight">Clustering</span>

| **Metric** | **Type**     | **Measures**                                                   | **Good Result**              |
| ---------- | ------------ | -------------------------------------------------------------- | ---------------------------- |
| **SSE**    | **Internal** | **Compactness:** How close points are to their **Centroid**.   | **Low** (Tight clusters)     |
| **SSB**    | **External** | **Separation:** How far clusters are from the **Global Mean**. | **High** (Distinct clusters) |

SSE+SSB=TSS (Total Sum of Squares), which is the max possible score for either metric.

> [!success]- One algorithm yields SSE=10 and SSB=5, what is the hypothetical best value if this algorithm was ideal?
> SSE+SSB=TSS
> TSS=10+5
> TSS=15
> **$\therefore$ Best values:**
> SSE=0
> SSB=15

