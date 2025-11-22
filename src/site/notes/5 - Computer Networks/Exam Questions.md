---
{"dg-publish":true,"permalink":"/5-computer-networks/exam-questions/"}
---



### **Scenario Data & Givens**
These values apply to the problems listed below:

* **Transmission Data:**
    * **MTU:** 400 bytes
    * **Total Data:** 10,000 bits (from Application Layer to send to Host H2)
    * **TCP Flavor:** Host H1 is running **TCP Tahoe** in **Congestion Avoidance**.
    * **Current Congestion Window:** $cwnd = 20 \text{ MSS}$
* **Packet Header Hex Values (Constant over time):**
    Host H1 receives a TCP segment from H2 with the following fields:
    * $A = AA01$
    * $B = BB02$
    * $C = 0012$
    * $D = DD13$
    * $E = A010$
    * $F = 333C$
    * $G = 10B2$
    * $H = 0000$
    * $I = 0ABC$
    * $J = 02BC$

![89180af3-a9f5-484a-b39d-6d958248ed23.png|400x345](/img/user/5%20-%20Computer%20Networks/img/89180af3-a9f5-484a-b39d-6d958248ed23.png)

**Questions:**
- **How many bytes of TCP _options_ are present in the header?**  
- **What is the Maximum Segment Size (MSS) used when Host H1 sends data to Host H2?**  
- **How many transmission rounds are required for H1 to send all bits of data to H2?**

> [!success]- Solution
> ![image-18.png|400x288](/img/user/5%20-%20Computer%20Networks/img/image-18.png)
> ![image-19.png|400x211](/img/user/5%20-%20Computer%20Networks/img/image-19.png)

---

### **Question 1: RTT Deviation Calculation**
TCP senders use the EWMA (Exponential Weighted Moving Average) algorithm with weight $\beta = 0.25$ to compute the average deviation at every transmission round.

**Given:**
* $\Delta_{inst} = 350\text{ ms}$ (Instantaneous/Sample Deviation)
* $\Delta_{prev\_dev} = 36\text{ ms}$ (Previous Average Deviation)

**Question:**
* **Current average deviation?**

---

### **Question 2: Sequence & ACK Numbers**
**Context:** A timeline diagram (bottom left) showing data transfer between Host A and Host B. Store-and-forward

**Sequence of Events:**
1.  Host A sends Data (10 bytes).
2.  Host A sends Data (11 bytes).
3.  Host A sends Data (12 bytes) with **Seq = 80**.
4.  Host A sends Data (13 bytes).
5.  Host B sends three Acknowledgments ($Ack_1, Ack_2, Ack_3$).

![image-16.png|400x491](/img/user/5%20-%20Computer%20Networks/img/image-16.png)

**Question:**
* **Ack 1, 2, 3 ?**
* **Seq 1, 2, 4 ?**

---

### **Additional Fragments/Notes**
* "app 20 pkt 4 routers" "pay attention to formula"


### **Problem Statement & Parameters**
* **Scenario:** "Consider TCP delay model."
* **Total Data:** "total = 45 segments to host B."
* **Transmission Time:** $T_{tr} = 2\text{ ms}$.
* **Process:** "Host A goes through Slow Start and Congestion Avoidance phases without any loss events."
* **Constraint 1 (Threshold):** "uses an initial threshold = 8 MSS."
* **Constraint 2 (RTT):** "an average RTT equal to 7 ms"

"Calculate total time in ms, needed to deliver all segments to B."

![image-17.png|400x449](/img/user/5%20-%20Computer%20Networks/img/image-17.png)

**Visual Layout:**
* **Vertical Axes:** Represent time for **Host A** (left) and **Host B** (right).
* **Arrows:** Diagonal arrows represent the transmission of segments from A to B.

**Round 1:**
* **Data:** 1 MSS sent.
* **Host A Time Cost:** $T_{tr} + RTT$
* **Host B Time Cost:** $T_{tr}$

**Round 2:**
* **Data:** 2 MSS sent.
* **Host A Time Cost:** $2 T_{tr} + RTT$
* **Host B Time Cost:** $2 T_{tr}$ (Written as $2T_r$)

**Round 3:**
* **Data:** 4 MSS sent.
* **Host A Time Cost:** $4 T_{tr} + RTT$ (Note: The number '4' is scribbled over a previous number, indicating the doubling pattern of Slow Start).
* **Host B Time Cost:** $4 T_{tr}$