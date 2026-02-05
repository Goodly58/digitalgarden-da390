---
{"dg-publish":true,"permalink":"/1-tr-cmp-340/w3-ii/"}
---

Lecture 6
slides.pptx

Exam Q:
Show execution. track all calls.

$\sum^\infty_{i=1} \frac{1}{i!}=e$


---

![image-29.png|400x216](/img/user/1%20-%20TR%20CMP340/img/image-29.png)

> [!success]- Solution
> Controlling variable is n (because stop condition depends on that variable)
> ![WIN_20260129_12_45_16_Pro.jpg|400x225](/img/user/1%20-%20TR%20CMP340/img/WIN_20260129_12_45_16_Pro.jpg)
> ![WIN_20260129_12_51_53_Pro.jpg|400x225](/img/user/1%20-%20TR%20CMP340/img/WIN_20260129_12_51_53_Pro.jpg)
> ![WIN_20260129_12_54_19_Pro.jpg|400x225](/img/user/1%20-%20TR%20CMP340/img/WIN_20260129_12_54_19_Pro.jpg)
> There was a tree drawn that helps you visualize why n(n-1)(n-2)...

![image-30.png|400x241](/img/user/1%20-%20TR%20CMP340/img/image-30.png)


Sequential search o(n) → unsorted array
Binary search o(log n) → sorted array 

![image-31.png|400x243](/img/user/1%20-%20TR%20CMP340/img/image-31.png)

![image-32.png|400x241](/img/user/1%20-%20TR%20CMP340/img/image-32.png)

- s = start index
- e = end index 

midpoint formula = (s+e)/2 OR $s+\frac{e-s}{2}$

s=e if start and end same (one element array)
s\<e if more than one element in array

> [!success]- Solution
> ![WIN_20260129_13_10_39_Pro.jpg|400x225](/img/user/1%20-%20TR%20CMP340/img/WIN_20260129_13_10_39_Pro.jpg)

Best case $\Omega 1$ time & space when?
> [!success]- Solution
> if A\[$\frac{s+e}2$\]=key
> i.e.
> if A\[$\frac{n-1}{2}$\]=key

Worst case?
> [!success]- Solution
> ![image-34.png|400x92](/img/user/1%20-%20TR%20CMP340/img/image-34.png)
> ![image-33.png|400x255](/img/user/1%20-%20TR%20CMP340/img/image-33.png)
> ![image-35.png|400x300](/img/user/1%20-%20TR%20CMP340/img/image-35.png)
> Dont forget to do both s_stack(n) s(n)

![image-36.png|400x200](/img/user/1%20-%20TR%20CMP340/img/image-36.png)

AA pattern
> [!success]- Solution
> 2 iterations only

AAB pattern

> [!success]- Solution
> Worst case
> ![image-37.png|400x296](/img/user/1%20-%20TR%20CMP340/img/image-37.png)

> Example
![image-38.png|400x286](/img/user/1%20-%20TR%20CMP340/img/image-38.png)


Time/space complexity

Worst?
> [!success]- Solution
> ![image-39.png|400x521](/img/user/1%20-%20TR%20CMP340/img/image-39.png)
> we take mn instead of $m^2$ because m\<n (also u can see m^2 = m x m)

Best?
> [!success]- Solution
> ![image-40.png|400x225](/img/user/1%20-%20TR%20CMP340/img/image-40.png)

Proof using Table?
> [!success]- Solution
> No space stack (non-recursive)
> ![image-41.png|400x711](/img/user/1%20-%20TR%20CMP340/img/image-41.png)

