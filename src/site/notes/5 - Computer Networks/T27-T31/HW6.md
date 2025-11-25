---
{"dg-publish":true,"permalink":"/5-computer-networks/t27-t31/hw-6/"}
---


Consider the network security scenario below. Describe the security objective it attempts to achieve and comment on whether the implementation is in fact going to meet the said objective.
![image-22.png|400x140](/img/user/5%20-%20Computer%20Networks/T27-T31/img/image-22.png)
> [!success]- Solution
> It's attempting to achieve confidentiality. However, she locked it with KA+ **rather than using Bob's public key (KB+)**. This is problematic since now it can't be unlocked by Bob. Bob also attempts to unlock it using KB- (Bob's private key), which is wrong as he cannot unlock it with his own key, since the only accepted key would be Alice's private key (but that's only known to her). Therefore, this diagram implementation will not meet the said objective.


### **Symmetric Key Cryptography (SKC) - No KDC**

1. In a network with **16 users** that implements SKC for secure communications, the total number of keys needed is <span class="gray-text">_______</span>.

> [!success]- Solution
> 
> $\frac{16\times15}2$ = 120

2. <span class="gray-text">In a network with **15 users** that implements SKC for secure communications, the total number of keys needed is _______.</span>
    <span class="gray-text"></span>
3. <span class="gray-text">In a network with **14 users** that implements SKC for secure communications, the total number of keys needed is _______.</span>
    <span class="gray-text"></span>
4. <span class="gray-text">In a network with **18 users** that implements SKC for secure communications, the total number of keys needed is _______.</span>
    <span class="gray-text"></span>
5. <span class="gray-text">In a network with **12 users** that implements SKC for secure communications, the total number of keys needed is _______.</span>
    <span class="gray-text"></span>

> [!success]- Solution
> 

### **Symmetric Key Cryptography (SKC) - With KDC**

6. In a network, with **20 users**, that implements SKC for secure communications and uses **KDC** for key distribution, the total number of keys needed is <span class="gray-text">_______</span>.

> [!success]- Solution
> $\frac{20\times19}{2}+20$
> = 210

7. <span class="gray-text">In a network, with **16 users**, that implements SKC for secure communications and uses **KDC** for key distribution, the total number of keys needed is _______.</span>
    <span class="gray-text"></span>
8. <span class="gray-text">In a network, with **15 users**, that implements SKC for secure communications and uses **KDC** for key distribution, the total number of keys needed is _______.</span>
    <span class="gray-text"></span>
9. <span class="gray-text">In a network, with **14 users**, that implements SKC for secure communications and uses **KDC** for key distribution, the total number of keys needed is _______.</span>
    <span class="gray-text"></span>
10. <span class="gray-text">In a network, with **12 users**, that implements SKC for secure communications and uses **KDC** for key distribution, the total number of keys needed is _______.</span>
    

### **Public Key Cryptography (PKC)**_

11. In a network with **26 users** that implements PKC for secure communications, the total number of keys needed is <span class="gray-text">_______</span>.

> [!success]- Solution
> $26\times2$=52

12. <span class="gray-text">In a network with **29 users** that implements PKC for secure communications, the total number of keys needed is _______.</span>
    <span class="gray-text"></span>
13. <span class="gray-text">In a network with **28 users** that implements PKC for secure communications, the total number of keys needed is _______.</span>
    <span class="gray-text"></span>
14. <span class="gray-text">In a network with **27 users** that implements PKC for secure communications, the total number of keys needed is _______.</span>
    <span class="gray-text"></span>
15. <span class="gray-text">In a network with **25 users** that implements PKC for secure communications, the total number of keys needed is _______.</span>
    

### **RSA Algorithm**

16. Using the RSA algorithm with $p = 3$, $q = 7$, and $e = d = 5$, if the plaintext is **BID**:
    - $n$ is \_\_\_\_.
    - $z$ is \_\_\_\_.
    - The ciphertext is \_\_\_\_.

> [!success]- Solution
> $n=p\times q$=3x7=21
> $z=(p-1)(q-1)$=12
> $c=M^e\mod n$=KRP
> 

17. <span class="gray-text">Using the RSA algorithm with $p = 3$, $q = 7$, and $e = d = 5$, if the plaintext is **GAS**:</span>
    <span class="gray-text"></span>
    - <span class="gray-text"> $n$ is ____.</span>
        <span class="gray-text"></span>
    - <span class="gray-text"> $z$ is ____.</span>
        <span class="gray-text"></span>
    - <span class="gray-text">The ciphertext is ____.</span>
        <span class="gray-text"></span>
18. <span class="gray-text">Using the RSA algorithm with $p = 5$, $q = 7$, and $e = d = 5$, if the plaintext is **POP**:</span>
    <span class="gray-text"></span>
    - <span class="gray-text"> $n$ is ____.</span>
        <span class="gray-text"></span>
    - <span class="gray-text"> $z$ is ____.</span>
        <span class="gray-text"></span>
    - <span class="gray-text">The ciphertext is ____.</span>
        

### **Polyalphabetic Ciphers (Standard Shift)**

_Condition: Key A = 0 shift, Key B = 1 shift._

19. Key **APT**. The ciphertext that corresponds to the plaintext **GENEVANS** is \_\_\_\_\_\_\_.

> [!success]- Solution
> ![image-24.png|400x293](/img/user/5%20-%20Computer%20Networks/T27-T31/img/image-24.png)

20. <span class="gray-text">Key **ART**. The ciphertext that corresponds to the plaintext **AMERICAN** is _______.</span>
21. <span class="gray-text">Key **GEL**. The ciphertext that corresponds to the plaintext **SPARTANS** is _______.</span>
22. <span class="gray-text">Key **ARM**. The ciphertext that corresponds to the plaintext **SPARTANS** is _______.</span>

### **Polyalphabetic Ciphers (Modified Shift)**

_Condition: Key A = 1 shift, Key B = 2 shift._

23. Key **CAD**. The plaintext **BENCH** becomes the ciphertext \_\_\_\_\_\_\_.

> [!success]- Solution
> ![image-25.png|400x295](/img/user/5%20-%20Computer%20Networks/T27-T31/img/image-25.png)

24. <span class="gray-text">Key **LEG**. The plaintext **CRAMP** becomes the ciphertext _______.</span>
    <span class="gray-text"></span>
25. <span class="gray-text">Key **GEL**. The plaintext **EAGER** becomes the ciphertext _______.</span>
    <span class="gray-text"></span>
26. <span class="gray-text">Key **HAD**. The plaintext **FAINT** becomes the ciphertext _______.</span>

### **Elliptic Curve Cryptography**

![image-23.png|400x297](/img/user/5%20-%20Computer%20Networks/T27-T31/img/image-23.png)

27. Which point on the elliptic curve shown below correspond to the following point addition/multiplications:
    - $A+B =$
    - $2A+B =$
    - $3A+B =$

> [!success]- Solution
> G
> C
> H

---
