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



![aligned_1_upright.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/aligned_1_upright.png)

![aligned_2_upright.png](/img/user/3%20-%20Machine%20Learning%20Notes/img/aligned_2_upright.png)
