---
{"dg-publish":true,"permalink":"/5-computer-networks/t23-t26/hw-5-q5/"}
---

# Homework
---

### Question 1
Multiple access protocols are needed when the link is \_\_\_\_ (dedicated, shared); in which case the channel is called \_\_\_\_ (wired, wireless, broadcast, unicast).

> [!success]- Solution
> **shared** (more than one use same link), **broadcast** (since they're on the same wire, every message in that link will be a broadcast)

---

### Question 2
IEEE 802.3 frames use a CRC technique with a \_\_\_\_-bit long FCS field and a \_\_\_\_-bit long divisor.

> [!success]- Solution
> 32, 33

---

### Question 3
IEEE 802.3 frames are delineated with 8 bytes: Each of the first 7 bytes is composed of these bits: \_\_\_\_\_\_\_\_, and the last byte is composed of these bits \_\_\_\_\_\_\_\_.

> [!success]- Solution
> 10101010
> 10101011

---

### Question 4
ARP request messages are \_\_\_\_\_\_\_ (unicast, multicast, broadcast), while ARP reply messages are \_\_\_\_\_\_\_ (unicast, multicast, broadcast).

> [!success]- Solution
> broadcast
> unicast

---

### Question 5
AL uses \_\_\_\_ to find the IP address that corresponds to a given host name; while LL uses \_\_\_\_ to find the physical address that corresponds to a given IP address.

> [!success]- Solution
> DNS
> ARP

---

### Question 6
During the journey from the source host to the destination host, the \_\_\_\_ addresses never change but the \_\_\_\_ addresses change from link to link.

> [!success]- Solution
> IP
> MAC

---

### Question 7
Slotted ALOHA is \_\_\_\_ (less, more) efficient than pure ALOHA because the vulnerability time of slotted ALOHA is \_\_\_\_ (less, more) than that of pure ALOHA.

> [!success]- Solution
> more
> less

---

### Question 8
Slotted ALOHA is \_\_\_\_ (less, more) efficient than CSMA/CD because the \_\_\_\_ (former, latter) uses \_\_\_\_ sensing and \_\_\_\_ detection.

> [!success]- Solution
> less, latter, carrier, collision

---

### Question 9
CSMA link efficiency \_\_\_\_ (increases, decreases) when the propagation delay \_\_\_\_ (increases, decreases).

> [!success]- Solution
> decreases, increases

---

### Question 10
LAN host A has payload data **100101111** to send to LAN host B. After using CRC with the divisor **110001**, host A finds a remainder equal to \_\_\_\_\_. Report your answer with the number of bits that fit in the FCS field.

> [!success]- Solution
> ![image-24.png](/img/user/5%20-%20Computer%20Networks/T23-T26/img/image-24.png)

---

### Question 11
<span class="gray-text">LAN host A has payload data **100110011** to send to LAN host B. After using CRC with the divisor **110101**, host A finds a remainder equal to \_\_\_\_\_. Report your answer with the number of bits that fit in the FCS field.</span>

> [!success]- Solution
> 

---

### Question 12
<span class="gray-text">LAN host A has payload data **1000110111** to send to LAN host B. After using CRC with the divisor **1001001**, host A finds a remainder equal to \_\_\_\_\_. Report your answer with the number of bits that fit in the FCS field.</span>

> [!success]- Solution
> 

---

### Question 13
<span class="gray-text">LAN host A has payload data **1000110001** to send to LAN host B. After using CRC with the divisor **1000011**, host A finds a remainder equal to \_\_\_\_\_. Report your answer with the number of bits that fit in the FCS field.</span>

> [!success]- Solution
> 

---

### Question 14
<span class="gray-text">LAN host A has payload data **1000101111** to send to LAN host B. After using CRC with the divisor **1000001**, host A finds a remainder equal to \_\_\_\_\_. Report your answer with the number of bits that fit in the FCS field.</span>

> [!success]- Solution
> 

---

### Question 15
<span class="gray-text">LAN host A has payload data **100100001** to send to LAN host B. After using CRC with the divisor **100011**, host A finds a remainder equal to \_\_\_\_\_. Report your answer with the number of bits that fit in the FCS field.</span>

> [!success]- Solution
> 01101

---

### Question 16
<span class="gray-text">LAN host A has payload data **100110101** to send to LAN host B. After using CRC with the divisor **110111**, host A finds a remainder equal to \_\_\_\_\_. Report your answer with the number of bits that fit in the FCS field.</span>

> [!success]- Solution
> 01010

---

### Question 17
LAN host A receives LL frame **1000110011100000** from LAN host B. After using CRC with the divisor **1000101**, host A finds a remainder equal to \_\_\_\_\_. Report your answer with the number of bits that fit in the FCS field.

> [!success]- Solution
> 

---

### Question 18
<span class="gray-text">LAN host A receives LL frame **1000110001000011** from LAN host B. After using CRC with the divisor **1000011**, host A finds a remainder equal to \_\_\_\_\_. Report your answer with the number of bits that fit in the FCS field.</span>

> [!success]- Solution
> 111011

---

### Question 19
<span class="gray-text">LAN host A receives LL frame **1000101111101000** from LAN host B. After using CRC with the divisor **1000001**, host A finds a remainder equal to \_\_\_\_\_. Report your answer with the number of bits that fit in the FCS field.</span>

> [!success]- Solution
> 001111

---

### Question 20
Consider a wired LAN with a bus topology extending over **140 meters** and running at the bit rate of **12 Mbps**. For CSMA/CD to work in this LAN, the minimum frame size must be \_\_\_\_ bytes.

> [!success]- Solution
> ![image-27.png](/img/user/5%20-%20Computer%20Networks/T23-T26/img/image-27.png)

---

### Question 21
<span class="gray-text">Consider a wired LAN with a bus topology extending over **160 meters** and running at the bit rate of **14 Mbps**. For CSMA/CD to work in this LAN, the minimum frame size must be \_\_\_\_ bytes.</span>

> [!success]- Solution

---

### Question 22

Consider the network with hosts H1–H7, access point AP1, and routers R1, R2, with the following actions:

![image00361158de8.jpg](/img/user/5%20-%20Computer%20Networks/T23-T26/img/image00361158de8.jpg)

| Host/Interface           | MAC address | IP address | Action                        |
| ------------------------ | ----------- | ---------- | ----------------------------- |
| Host H1                  | MAC1        | IP1        | H1 sends pkt-1 to H7          |
| Host H2                  | MAC2        | IP2        | H2 sends pkt-2 to H5          |
| Host H3                  | MAC3        | IP3        | H3 is idle                    |
| Host H4                  | MAC4        | IP4        | H4 is idle                    |
| Host H5                  | MAC5        | IP5        | H5 sends pkt-5 to H2          |
| Host H6                  | MAC6        | IP6        | H6 is idle                    |
| Host H7                  | MAC7        | IP7        | H7 sends pkt-7 to H1          |
| Access Point AP1         | MAC-AP1     | IP-AP1     | AP1 relays pkt-7 from H7      |
| Router R1, Interface R11 | MAC11       | IP11       | Normal routing and forwarding |
| Router R1, Interface R12 | MAC12       | IP12       | Normal routing and forwarding |
| Router R2, Interface R21 | MAC21       | IP21       | Normal routing and forwarding |
| Router R2, Interface R22 | MAC22       | IP22       | Normal routing and forwarding |

Fill in the following blanks:
- The receiver MAC address in pkt-7 when it leaves host H7 is \_\_\_\_.
> [!success]- Solution  
> MAC-AP1  

- The source MAC address when pkt-7 reaches router R2 is \_\_\_\_.
> [!success]- Solution  
> MAC7  

- The destination MAC address when pkt-7 is forwarded by router R1 is \_\_\_\_.
> [!success]- Solution  
> MAC1  

- The destination IP address in pkt-2 when it is forwarded by router R1 is \_\_\_\_.
> [!success]- Solution  
> IP5  

- The source MAC address in pkt-1 when it leaves router R1 is \_\_\_\_.
> [!success]- Solution  
> MAC12  

- The destination MAC address when pkt-1 reaches host H1 is \_\_\_\_.
> [!success]- Solution  
> MAC1

- The source IP address when pkt-7 is forwarded by switch S2 is \_\_\_\_.
> [!success]- Solution  
> IP7  

- The destination IP address when pkt-7 is relayed by access point AP1 is \_\_\_\_.
> [!success]- Solution  
> IP1

- The destination MAC address in pkt-7 when it leaves host H7 is \_\_\_\_.
> [!success]- Solution  
> MAC-AP1

- The source MAC address when pkt-1 reaches router R2 is \_\_\_\_.
> [!success]- Solution  
> MAC12  

- The destination MAC address when pkt-1 is forwarded by router R1 is \_\_\_\_.
> [!success]- Solution  
> MAC21  


---

### Question 25

Consider the network with the following scenario:

![image-23.png](/img/user/5%20-%20Computer%20Networks/T23-T26/img/image-23.png)

![image00361158de8.jpg](/img/user/5%20-%20Computer%20Networks/T23-T26/img/image00361158de8.jpg)

Fill in the following blanks:

- The source MAC address in **pkt-5** when it leaves router R2 is \_\_\_\_.  
- The destination MAC address when **pkt-2** reaches host H1 is \_\_\_\_.  
- The source IP address when **pkt-1** is forwarded by router R2 is \_\_\_\_.  
- The destination IP address when **pkt-1** is forwarded by router R2 is \_\_\_\_.  

> [!success]- Solution
> •       The source MAC address in pkt-5 when it leaves router R2 is MAC21. 
> •       The destination MAC address when pkt-2 reaches host H1 is MAC1. 
> •       The source IP address when pkt-1 is forwarded by router R2 is IP1. 
> •       The destination IP address when pkt-1 is forwarded by router R2 is IP7. 


# Quiz Qs

1) During the journey from the source host to the destination host, the \_\_\_\_\_ addresses never change but the \_\_\_\_\_ addresses change from link to link..

> [!success]- Solution
> IP addresses never change, but MAC addresses change from link to link.

2) CSMA link efficiency \_\_\_\_\_ when the propagation delay \_\_\_\_\_.

> [!success]- Solution
> CSMA link efficiency INCREASE when the propagation delay DECREASE.

3) AL uses \_\_\_\_ to find the IP address that corresponds to a given host name; while LL uses \_\_\_\_ to find the physical address that corresponds to a given IP address.

> [!success]- Solution
> AL uses DNS (Domain name System) while LL uses ARP (Address Resolution Protocol).

4) IEEE 802.3 frames use a CRC technique with a \_\_\_-bit long FCS field and a \_\_\_-bit long divisor.

> [!success]- Solution
> IEEE 802.3 frames use a 32-bit long FCS field and a 33-bit long divisor.

5) Multiple access protocols are needed when the link is \_\_\_\_\_ (dedicated, shared); in which case the channel is called \_\_\_\_\_ (wired, wireless, broadcast, unicast).

> [!success]- Solution
> Multiple access protocols are needed when the link is Shared; in which case
> the channel is called BROADCAST.

6) Slotted ALOHA is \_\_\_\_ (less, more) efficent than pure ALOHA because the vulnerability time of slotted ALOHA is \_\_\_\_ (less, more) than that of pure ALOHA.

> [!success]- Solution
> Slotted ALOHA is more efficent than pure ALOHA because the vulnerability time of
> slotted ALOHA is less than that of pure ALOHA.

7) Slotted ALOHA is \_\_\_\_ (less, more) efficient than CSMA/CD because the \_\_\_\_ (former, latter) uses \_\_\_\_ sensing and \_\_\_\_ detection.

> [!success]- Solution
> Slotted ALOHA is less efficient than CSMA/CD because the latter uses carrier sensing and collision detection.

8) LAN host A receives LL frame 10011101110110 from LAN host B. After using CRC with the divisor 111101, host A finds a remainder equal to \_\_\_\_\_.

> [!success]- Solution
> ![image-25.png](/img/user/5%20-%20Computer%20Networks/T23-T26/img/image-25.png)The remainder is 01000.



