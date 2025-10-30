---
{"dg-publish":true,"permalink":"/3-machine-learning-notes/previous-midterm/"}
---

![image-30.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-30.png)


> [!success]- Solution
> ![image-31.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-31.png)


![WhatsApp Image 2025-10-30 at 18.58.48_215a66b8.jpg](/img/user/3%20-%20Machine%20Learning%20Notes/img/WhatsApp%20Image%202025-10-30%20at%2018.58.48_215a66b8.jpg)

> [!success]- Solution
> 
> | Parameter        | Likelihood of overfitting the data (increase, decrease, no effect)                                                                                                                                                                                              |
> | ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
> | min_samples_leaf | **Decrease** <br>By increasing the number of samples for leaf nodes to exist, this indirectly acts similar to when you lower `max_depth`, as the more you increase it, the more likely you are to stop splitting earlier (which, in turn, reduces overfitting). |
> | ccp_alpha (α)    | **Decrease**<br>This parameter penalizes more complex trees _(ones with more leaf nodes)_ so choosing simpler trees _(ones with less leaf nodes)_ results in a simpler model (more branches pruned → smaller tree → less overfitting).                          |
> | n_neighbors      | **Decrease**<br>In KNNs, the smaller the number of neighbors, the more overfitted the data is _because the model memorizes based on few neighbors and now more susceptible to noise_. Therefore, having more neighbors would have the opposite effect.          |
> | random_state     | **No effect**<br>Having a random estimator does not increase or decrease the likelihood of data being overfitted, this is because the tree size (or number of branches) is not affected                                                                         |
> 

![Q3_aligned_upright_v2.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/Q3_aligned_upright_v2.png)

> [!success]- Solution
> ![image-32.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-32.png)

![Q4_aligned_upright.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/Q4_aligned_upright.png)

> [!success]- Solution
> 
> | Model                    | Results will vary? | Reason                                                                                                                                                                                                                                                                                                                                               |
> | ------------------------ | ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
> | KNN                      | Yes                | KNN needs to apply normalization here as otherwise data with bigger ranges (ex. annual income) will dominate smaller ranges (ex. age). Therefore, there will be a difference in value as experiment 1 will consider age, while experiment 2 age's effect will be minimal (as it will be overshadowed by annual income).                              |
> | Decision Tree Classifier | No                 | No because the deciding splits (and thus the resulting tree) would **not change**. This is because the tree is built depending on the order of values (_order of values is still the same: `22 < 25 < 35 < 50` → `0.0 < 0.08 < 0.33 < 0.78`_), impurity formulas, and error estimates, rather than the specific values of the attributes themselves. |
> | Decision Tree Regressor  | No                 | Similar reason to decision tree classifier. Rescaling doesn’t alter which samples fall left/right at each split, so predictions remain identical                                                                                                                                                                                                     |
> | Naive Bayes              | No                 | Naive bayes handles noise and differences in the range of attributes well (since it looks at probability), so the results will not vary significantly.                                                                                                                                                                                               |
> 

![aligned_1_upright.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/aligned_1_upright.png)

> [!success]- Solution
> 
> | Dataset     | Suitable? | Why?                                                                                                                                                                                                                                                        |
> | ----------- | --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
> | KNN         | No        | KNN is not suitable because it must store the entire dataset and compute distances to every record when predicting. With a very large dataset, both the memory requirement and distance computations (O(Nd)) become impractical.                            |
> | Naive Bayes | Yes       | Naive Bayes is suitable because it only stores a few summary statistics (class priors, means, variances, or counts) instead of the entire dataset. These can be computed in a single pass, making it memory-efficient and scalable for very large datasets. |
> 

![aligned_2_upright.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/aligned_2_upright.png)

> [!success]- Solution
> ![image-33.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/image-33.png)