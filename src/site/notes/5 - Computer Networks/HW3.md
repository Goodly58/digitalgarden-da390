---
{"dg-publish":true,"permalink":"/5-computer-networks/hw-3/"}
---


### Network layer & service model

- The network layer that follows the __ service model gives a best-effort, connectionless service to the transport layer.

> [!success]- Solution
> Datagram

- The network layer ensures that two hosts, even on __ networks, can still exchange packets.

> [!success]- Solution
> different


### SDN and control/data planes

- Routing is a control plane function whereas forwarding is a __ plane function.

> [!success]- Solution
> data

- Routing is a __ plane function whereas forwarding is a data plane function.

> [!success]- Solution
> control

- In the SDN approach, remote controllers, instead of the routers, implement the __ plane functions.

> [!success]- Solution
> CP

### Router roles, architecture, and functions

- The main functions of IP routers are __ and forwarding.

> [!success]- Solution
> routing

- The main functions of IP routers are routing and \_\_.

> [!success]- Solution
> forwarding
    
- A typical IP router architecture comprises a routing processor, several I/O ports, and a switch \_\_.

> [!success]- Solution
> fabric

- A typical IP router architecture comprises a __ processor, several I/O ports, and a switch fabric.

> [!success]- Solution
> routing

- The devices that implement the network layer inside the internet core are called \_\_.

> [!success]- Solution
> routers

### IPv4 header fields, flags, and first-byte hex

- The __ field in the header of an IPv4 datagram can be used to provide different classes of service inside the network. Your answer must be an acronym.

> [!success]- Solution
> TOS

- The __ flag in the header of an IPv4 datagram is set to 1 in the first of many fragments.

> [!success]- Solution
> 

- The M flag in the header of an IPv4 datagram is set to __ in the last of many fragments.

> [!success]- Solution
> 0
    
- The __ flag in the header of an IPv4 datagram is set to 1 if the datagram is not to be fragmented. 

> [!success]- Solution
> D

- In an IPv4 datagram with a 24-byte header, the HEX representation of the first 8 bits in the header is __.

> [!success]- Solution
> HLEN = 24/4 = 6
> 46

- <span class="gray-text">In an IPv4 datagram with a 32-byte header, the HEX representation of the first 8 bits in the header is __.</span>

- <span class="gray-text">In an IPv4 datagram with a 36-byte header, the HEX representation of the first 8 bits in the header is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">In an IPv4 datagram with a 40-byte header, the HEX representation of the first 8 bits in the header is __.</span>

- <span class="gray-text">In an IPv4 datagram with a 44-byte header, the HEX representation of the first 8 bits in the header is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">In an IPv4 datagram with a 60-byte header, the HEX representation of the first 8 bits in the header is __.</span>

### DHCP

- In the first step of the DHCP process, the client sends a DHCP __ message, to which the server replies with a DHCP offer message.

> [!success]- Solution
> discover

- In the first step of the DHCP process, the client sends a DHCP discover message, to which the server replies with a DHCP __ message.

> [!success]- Solution
> offer

- In the DHCP discover message, the source IP address is __ and the destination IP address is \_\_

> [!success]- Solution
> Source: 0.0.0.0
> Destination: 255.255.255.255


### IPv6 addressing: expansion & compression

- The full length IPv6 address obtained from the shortened notation AABB::A00:B10:E11 is the following: . Use the colon-separated HEX notation.

> [!success]- Solution
> AABB:0000:0000:0000:0000:0A00:0B10:0E11

- The full length IPv6 address obtained from the shortened notation AABB:0:0:AB11::E11 is the following: . Use the colon-separated HEX notation.

> [!success]- Solution
> AABB:0000:0000:AB11:0000:0000:0000:0E11

- <span class="gray-text">The full length IPv6 address obtained from the shortened notation AABB:0:0:AB11::E11 is the following: __. Use the colon-separated HEX notation.</span>
    
- The shortest notation of the IPv6 address AB11:0:BB11:0:0:0:0:EE11 is the following: . Use the colon-separated HEX notation.

> [!success]- Solution
> AB11:0:BB11::EE11

- <span class="gray-text">The shortest notation of the IPv6 address AB11:0:0:BB11:0:0:0:EE11 is the following: __. Use the colon-separated HEX notation.</span>
    <span class="gray-text"></span>
- <span class="gray-text">The shortest notation of the IPv6 address AB11:0:BB11:0:0:0:0:EE11 is the following: __. Use the colon-separated HEX notation.</span>
    <span class="gray-text"></span>
- The three important types of IPv6 addresses are the __ addresses, the anycast addresses, and the multicast addresses.

> [!success]- Solution
> unicast

- The three important types of IPv6 addresses are the unicast addresses, the ___ addresses, and the multicast addresses.

> [!success]- Solution
> anycast

- IPv4 addresses are 32-bit long whereas IPv6 addresses are __-bit long.

> [!success]- Solution
> 128

- IPv4 addresses are __-bit long whereas IPv6 addresses are 128-bit long.

> [!success]- Solution
> 32

### Classful IPv4 default masks (CIDR)

- In the classful IPv4 addressing, the default subnet mask for the address 45.3.2.1 is /. Use the CIDR notation.

> [!success]- Solution
> 

- <span class="gray-text">In the classful IPv4 addressing, the default subnet mask for the address 45.3.2.1 is /__. Use the CIDR notation.</span>
    <span class="gray-text"></span>
- <span class="gray-text">In the classful IPv4 addressing, the default subnet mask for the address 193.3.2.1 is /__. Use the CIDR notation.</span>
    <span class="gray-text"></span>
- <span class="gray-text">In the classful IPv4 addressing, the default subnet mask for the address 193.3.2.1 is /__. Use the CIDR notation.</span>

### NAT / private addressing

- If the address block 10.x.y.z/24 is used by an organization, a __ router must be used before any IP packets originating from within this organization is forwarded into the public internet.

> [!success]- Solution
> NAT

### ICMP and NL troubleshooting tools

- **__ is an application that uses on ICMP Echo Request and Echo Reply messages to check the NL connectivity between two nodes.**

> [!success]- Solution
> Ping

- **__ is an application that uses ICMP error-reporting messages to determine the number of routers between a source and a destination.**

> [!success]- Solution
> traceroute

- <span class="gray-text">__ is an application that uses ICMP error-reporting messages to determine the number of routers between a source and a destination.</span>
    
- **__ is a protocol used for query messaging and error reporting by the network layer. It runs directly over IP. Your answer must be an acronym.**

> [!success]- Solution
> ICMP

### Routing protocols & algorithms

- **In a network that runs __ routing protocol, the link cost is inversely proportional to its bit rate. Your answer must be an acronym.**

> [!success]- Solution
> OSPF

- In a network that runs __ routing protocol, the maximum number of hops is 15. Your answer must be an acronym.

> [!success]- Solution
> RIP

- **__ is a routing protocol that uses a composite metric that is based on delay, bandwidth, reliability, and load. Your answer must be an acronym.**

> [!success]- Solution
> EIGRP

- **__ is a Cisco proprietary routing protocol that uses DV algorithm to find the LCPs in a network. Your answer must be an acronym.**

> [!success]- Solution
> EIGRP

- __ algorithm is used by global routing protocols. It requires that every node be aware of the entire network topology and the cost of its links. Your answer must be an acronym.

> [!success]- Solution
> LS

- __ algorithm is used by decentralized routing protocols. The nodes need not be aware of the entire network topology. They simply rely on updates from their immediate neighbors. Your answer must be an acronym.

> [!success]- Solution
> DV

- **__ is a two-node instability problem that networks running RIP protocol can suffer from. Your answer must be an acronym.**

> [!success]- Solution
> CTI

- **Like split horizon, __ is a technique that could be used to mitigate the CTI instability problem.**

> [!success]- Solution
> Poisoned reverse

- **Like poisoned reverse, __ is a technique that could be used to mitigate the CTI instability problem.**

> [!success]- Solution
> Split Horizon

- In DV routing, if a node X receives an update about a cost from the same neighbor, then X takes the __ value of the cost. Choose either "oldest", "latest", "smallest", or "highest".

> [!success]- Solution
> latest

- In DV routing, if a node X receives an update about a cost from a different neighbor, then X takes the __ value of the cost. Choose either "oldest", "latest", "smallest", or "highest".

> [!success]- Solution
> smallest

### IPv4 fragmentation (number of fragments)

- A standard IPv4 datagram with a total length equal to 5800 bytes arrives to a router output port whose MTU is 1220 bytes. The number of fragments leaving this router port is equal to __.

> [!success]- Solution
> $\lceil(5800-20)/(1220-20)\rceil=\lceil4.81\rceil$=5 fragments
> 

- <span class="gray-text">A standard IPv4 datagram with a total length equal to 4800 bytes arrives to a router output port whose MTU is 660 bytes. The number of fragments leaving this router port is equal to __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">A standard IPv4 datagram with a total length equal to 7800 bytes arrives to a router output port whose MTU is 2940 bytes. The number of fragments leaving this router port is equal to __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">A standard IPv4 datagram with a total length equal to 6800 bytes arrives to a router output port whose MTU is 2020 bytes. The number of fragments leaving this router port is equal to __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">A standard IPv4 datagram with a total length equal to 5800 bytes arrives to a router output port whose MTU is 1380 bytes. The number of fragments leaving this router port is equal to __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">A standard IPv4 datagram with a total length equal to 5800 bytes arrives to a router output port whose MTU is 2180 bytes. The number of fragments leaving this router port is equal to __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">A standard IPv4 datagram with a total length equal to 6800 bytes arrives to a router output port whose MTU is 1420 bytes. The number of fragments leaving this router port is equal to __.</span>

### Subnetting: network & broadcast addresses

- Consider a LAN interface with the IPv4 address 188.165.250.245/19. The network address in this LAN is \_\_.

> [!success]- Solution
> 188.165.224.0

- <span class="gray-text">Consider a LAN interface with the IPv4 address 125.125.175.3/18. The network address in this LAN is __.</span>
    
- Consider a LAN interface with the IPv4 address 60.33.12.1/26. The broadcast address in this LAN is \_\_.

> [!success]- Solution
> network 60.33.12.0000 0001
> subnet 255.255.255.1100 0000
> max = 255-128-64 = 63
> 60.33.12.63

- <span class="gray-text">Consider a LAN interface with the IPv4 address 188.165.250.245/21. The network address in this LAN is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">Consider a LAN interface with the IPv4 address 168.255.255.245/23. The network address in this LAN is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">Consider a LAN interface with the IPv4 address 60.33.12.1/25. The broadcast address in this LAN is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">Consider a LAN interface with the IPv4 address 33.60.250.1/22. The broadcast address in this LAN is __.</span>
    
- <span class="gray-text">Consider a LAN interface with the IPv4 address 12.6.128.25/19. The broadcast address in this LAN is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">Consider a LAN interface with the IPv4 address 12.6.128.25/20. The broadcast address in this LAN is __.</span>

### EIGRP metrics (bandwidth & delay)

- A network path, composed of many links, has a minimum bit rate of 10 Mbps and a total delay of 10 milliseconds. Compute the EIGRP bandwidth and delay metrics for this path.  
    • EIGRP bandwidth metric is __.  
    • EIGRP delay metric is __.

> [!success]- Solution
> $\frac{10^7}{10x10^3kbps} = 10^3 = 1000$ bandwidth
> $D=T_{tot}/10=\frac{10,000 (microseconds)}{10}=1000$ delay
> If he asked for M
> $M=256(B+D) = 256(1000+1000)=512000$

- <span class="gray-text">A network path, composed of many links, has a minimum bit rate of 10 Mbps and a total delay of 6 milliseconds. Compute the EIGRP bandwidth and delay metrics for this path.  </span>
    <span class="gray-text">• EIGRP bandwidth metric is __.  </span>
    <span class="gray-text">• EIGRP delay metric is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">A network path, composed of many links, has a minimum bit rate of 10 Mbps and a total delay of 5 milliseconds. Compute the EIGRP bandwidth and delay metrics for this path.  </span>
    <span class="gray-text">• EIGRP bandwidth metric is __.  </span>
    <span class="gray-text">• EIGRP delay metric is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">A network path, composed of many links, has a minimum bit rate of 16 Mbps and a total delay of 13 milliseconds. Compute the EIGRP bandwidth and delay metrics for this path.  </span>
    <span class="gray-text">• EIGRP bandwidth metric is __.  </span>
    <span class="gray-text">• EIGRP delay metric is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">A network path, composed of many links, has a minimum bit rate of 16 Mbps and a total delay of 14 milliseconds. Compute the EIGRP bandwidth and delay metrics for this path.  </span>
    <span class="gray-text">• EIGRP bandwidth metric is __.  </span>
    <span class="gray-text">• EIGRP delay metric is __.</span>
    <span class="gray-text"></span>

### Distance-Vector (DV) routing scenarios

![image-14.png](/img/user/5%20-%20Computer%20Networks/img/image-14.png)

- Consider the DV routing scenario shown below with the costs Cxu = 5, Cxv = 10, and Cxw = 5. The respective minimum distance vectors from (u, v, w) to (a, b) are: Du(a, b) = (9, 8), Dv(a, b) = (8, 8), and Dw(a, b) = (8, 7). Compute the least cost from node x to node a and the least cost from node x to node b.  
    • The least cost from node x to node a is \_\_.  
    • The least cost from node x to node b is \_\_.

> [!success]- Solution
> 5+9 10+8 **5+8** → lowest 13
> 5+8 10+8 **5+7** → lowest 12

- <span class="gray-text">Consider the DV routing scenario shown below with the costs Cxu = 11, Cxv = 3, and Cxw = 7. The respective minimum distance vectors from (u, v, w) to (a, b) are: Du(a, b) = (4, 6), Dv(a, b) = (6, 6), and Dw(a, b) = (11, 8). Compute the least cost from node x to node a and the least cost from node x to node b.  </span>
    <span class="gray-text">`image018642558fc.jpg`  </span>
    <span class="gray-text">• The least cost from node x to node a is __.  </span>
    <span class="gray-text">• The least cost from node x to node b is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">Consider the DV routing scenario shown below with the costs Cxu = 11, Cxv = 6, and Cxw = 8. The respective minimum distance vectors from (u, v, w) to (a, b) are: Du(a, b) = (5, 6), Dv(a, b) = (6, 7), and Dw(a, b) = (5, 3). Compute the least cost from node x to node a and the least cost from node x to node b.  </span>
    <span class="gray-text">`image021642558fc.jpg`  </span>
    <span class="gray-text">• The least cost from node x to node a is 12.  </span>
    <span class="gray-text">• The least cost from node x to node b is 11.</span>
    <span class="gray-text"></span>
- <span class="gray-text">Consider the DV routing scenario shown below with the costs Cxu = 5, Cxv = 10, and Cxw = 5. The respective minimum distance vectors from (u, v, w) to (a, b) are: Du(a, b) = (9, 8), Dv(a, b) = (8, 8), and Dw(a, b) = (8, 7). Compute the least cost from node x to node a and the least cost from node x to node b.  </span>
    <span class="gray-text">`image016642558fc.jpg`  </span>
    <span class="gray-text">• The least cost from node x to node a is 13.  </span>
    <span class="gray-text">• The least cost from node x to node b is 12.</span>
    <span class="gray-text"></span>
- <span class="gray-text">Consider the DV routing scenario shown below with the costs Cxu = 3, Cxv = 10, and Cxw = 10. The respective minimum distance vectors from (u, v, w) to (a, b) are: Du(a, b) = (9, 4), Dv(a, b) = (9, 11), and Dw(a, b) = (10, 6). Compute the least cost from node x to node a and the least cost from node x to node b.  </span>
    <span class="gray-text">`image016642558fc.jpg`  </span>
    <span class="gray-text">• The least cost from node x to node a is 12.  </span>
    <span class="gray-text">• The least cost from node x to node b is 7.</span>
    <span class="gray-text"></span>
- <span class="gray-text">Consider the DV routing scenario shown below with the costs Cxu = 10, Cxv = 8, and Cxw = 3. The respective minimum distance vectors from (u, v, w) to (a, b) are: Du(a, b) = (5, 10), Dv(a, b) = (11, 6), and Dw(a, b) = (9, 6). Compute the least cost from node x to node a and the least cost from node x to node b.  </span>
    <span class="gray-text">`image018642558fc.jpg`  </span>
    <span class="gray-text">• The least cost from node x to node a is __.  </span>
    <span class="gray-text">• The least cost from node x to node b is __.</span>
    


---



### SDN, control/data planes

- **In the SDN approach, modern routers implement the __ plane functions. Your answer must be an acronym.**

> [!success]- Solution
> DP (because they handle the forwarding). 

- **In the SDN approach, remote controllers, instead of the routers, implement the __ plane functions. Your answer must be an acronym.**

> [!success]- Solution
> CP

- In the SDN approach, modern routers only implement the __ plane function.

> [!success]- Solution
> data

- Routing is a control plane function whereas forwarding is a __ plane function.

> [!success]- Solution
> data


### IPv4 header: rows, fields, flags & first-byte HEX

- **The second row of an IPv4 datagram header is dedicated to the process of \_\_.**

> [!success]- Solution
> fragmentation

- The M flag in the header of an IPv4 datagram is set to 1 in the __ of many fragments.

> [!success]- Solution
> first
    
- The M flag in the header of an IPv4 datagram is set to 0 in the __ of many fragments.

> [!success]- Solution
> last

- The __ flag in the header of an IPv4 datagram is set to 1 if the datagram is not to be fragmented.

> [!success]- Solution
> D

- <span class="gray-text">In an IPv4 datagram with a 32-byte header, the HEX representation of the first 8 bits in the header is __.</span>

- <span class="gray-text">In an IPv4 datagram with a 20-byte header, the HEX representation of the first 8 bits in the header is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">In an IPv4 datagram with a 60-byte header, the HEX representation of the first 8 bits in the header is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">In an IPv4 datagram with a 40-byte header, the HEX representation of the first 8 bits in the header is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">In an IPv4 datagram with a 36-byte header, the HEX representation of the first 8 bits in the header is __.</span>
    
<span class="neon-highlight">- The __ header field in an IPv4 datagram is used to prevent lost packets from staying inside the network indefinitely. Your answer must be an acronym</span>

> [!success]- Solution
> TTL

<span class="neon-highlight">- The \_\_ field in the header of an IPv4 datagram can be used to provide different classes of service inside the network.</span>

> [!success]- Solution
> TOS
    
- **In an IPv4 network that does not use priority classes, if a datagram has a 60-byte header and a total length of 515 bytes, then the HEX representation of the fields of the first header row is \_\_.**

> [!success]- Solution
> 1️⃣ Version = 4, HLEN=60/4=15(F)
> 2️⃣ No priority classes → DSCP/ECN (TOS) = 0000 0000 (bin) = 00 (hex) when no QoS 
> 3️⃣ Length = 515 to hex is 0203
> `4F 00 0203`

### Addressing (IPv4 & IPv6)

- <span class="gray-text">IPv4 addresses are 32-bit long whereas IPv6 addresses are __-bit long. Your answer must be an acronym.</span>
    <span class="gray-text"></span>
- <span class="gray-text">IPv4 addresses are 32-bit long whereas IPv6 addresses are __-bit long.</span>

- The three important types of IPv6 addresses are __ addresses, __ addresses, and __ addresses.

> [!success]- Solution
> unicast, anycast, multicast
    
    
- In the classful IPv4 addressing, the default subnet mask for the address 45.3.2.1 is /__.

> [!success]- Solution
> /8

- In the classful IPv4 addressing, the default subnet mask for the address 193.3.2.1 is /__.

> [!success]- Solution
> /24

- <span class="gray-text">The full length IPv6 address obtained from the shortened notation AABB::A00:B10 is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">The full length IPv6 address obtained from the shortened notation AABB::A00:B10:E11 is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">The shortest notation of the IPv6 address AB11:0:0:BB11:0:0:0:EE11 is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">The shortest notation of the IPv6 address AABB:CCDD:EEFF:0:0:0:AAAA is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">The shortest notation of the IPv6 address AABB:CCDD:EEFF:0:0:0:AAAA:BBBB is __.</span>
    

### DHCP

- In the first step of the DHCP process, the client sends a DHCP __ message, to which the server replies with a DHCP offer message.

> [!success]- Solution
> discover

- In the DHCP discover message, the source IP address is __ and the destination IP address is __.

> [!success]- Solution
> 0.0.0.0
> 255.255.255.255

### NAT / private addressing

- If the address block 10.x.y.z/24 is used by an organization, a __ router must be used before any IP packets originating from within this organization are forwarded into the public internet.

> [!success]- Solution
> NAT

### ICMP & troubleshooting tools

- __ is an application that uses ICMP Echo Request and Echo Reply messages to check the NL connectivity between two nodes.

> [!success]- Solution
> ping

- __ is a protocol used for query messaging and error reporting by the network layer.

> [!success]- Solution
> ICMP
    
- __ is a protocol used for query messaging and error reporting by the network layer. It runs directly over IP. Your answer must be an acronym.

> [!success]- Solution
> 

- __ is an application that uses ICMP error-reporting messages to determine the number of routers between a source and a destination.

> [!success]- Solution
> traceroute

### Service model

- The network layer that follows the __ service model gives a best-effort, connectionless service to the transport layer.

> [!success]- Solution
> datagram

### Routing protocols & algorithms (DV/LS/OSPF/RIP/EIGRP) + stability

- __ is a standard IETF routing protocol that uses the DV algorithm to find the Least Cost Paths (LCPs) in a network.

> [!success]- Solution
> RIP

- __ algorithm is used by decentralized routing protocols. The nodes need not be aware of the entire network topology. They simply rely on updates from their immediate neighbors. Your answer must be an acronym.

> [!success]- Solution
> DV

- __ algorithm is used by global routing protocols. It requires that every node be aware of the entire network topology and the cost of its links. Your answer must be an acronym.

> [!success]- Solution
> LS
    
- __ is a routing protocol that uses a composite metric that is based on delay, bandwidth, reliability, and load. Your answer must be an acronym.

> [!success]- Solution
> EIGRP

- __ is a Cisco proprietary routing protocol that uses DV algorithm to find the LCPs in a network. Your answer must be an acronym.

> [!success]- Solution
> EIGRP

- __ is a two-node instability problem that networks running RIP protocol can suffer from. Your answer must be an acronym.

> [!success]- Solution
> CTI

- In a network that runs __ routing protocol, the link cost is inversely proportional to its bit rate.

> [!success]- Solution
> OSPF

- In a network that runs __ routing protocol, the maximum number of hops is 15.
    
> [!success]- Solution
> RIP

### Subnetting: network & broadcast addresses

<span class="neon-highlight">Consider a LAN interface with the IPv4 address 10.128.1.2/12. The last usable host address in this LAN is \_\_</span>

> [!success]- Solution
> 10.1000 0000
> 255.1111
> max = 1000 1111 = 143
> 10.143.255.255 (broadcast)
> **Therefore:
> 10.143.255.254 (last usable host) **

### IPv4 fragmentation: counts & payload size

- <span class="gray-text">A standard IPv4 datagram with a total length equal to 7800 bytes arrives at a router output port whose MTU is 940 bytes. The number of fragments leaving this router port is equal to __.</span>
    <span class="gray-text"></span>
<span class="neon-highlight">- A standard IPv4 datagram with a total length equal to 12800 bytes arrives at a router output port whose MTU is 1220 bytes. The payload size of the last fragment leaving this router port is equal to __ bytes.</span>

- <span class="gray-text">A standard IPv4 datagram with a total length equal to 4800 bytes arrives to a router output port whose MTU is 820 bytes. The number of fragments leaving this router port is equal to __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">A standard IPv4 datagram with a total length equal to 7800 bytes arrives to a router output port whose MTU is 2940 bytes. The number of fragments leaving this router port is equal to __.</span>
    

### EIGRP metrics

- <span class="gray-text">A network path, composed of many links, has a minimum bit rate of 10 Mbps and a total delay of 10 milliseconds. Compute the EIGRP metrics.  </span>
    <span class="gray-text">• EIGRP bandwidth metric is __.  </span>
    <span class="gray-text">• EIGRP delay metric is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">A network path, composed of many links, has a minimum bit rate of 10 Mbps and a total delay of 8 milliseconds. Compute the EIGRP metrics.  </span>
    <span class="gray-text">• EIGRP bandwidth metric is __.  </span>
    <span class="gray-text">• EIGRP delay metric is __.</span>
    

### Distance-Vector (DV) routing scenarios

![image-14.png](/img/user/5%20-%20Computer%20Networks/img/image-14.png)


- <span class="gray-text">Consider the DV routing scenario with costs Cxu = 10, Cxv = 9, Cxw = 9 and vectors Du(a,b)=(7,7), Dv(a,b)=(5,9), Dw(a,b)=(7,5).  </span>
    <span class="gray-text">• The least cost from node x to node a is __.  </span>
    <span class="gray-text">• The least cost from node x to node b is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">Consider the DV routing scenario with costs Cxu = 3, Cxv = 10, Cxw = 10 and vectors Du(a,b)=(9,4), Dv(a,b)=(9,11), Dw(a,b)=(10,6).  </span>
    <span class="gray-text">• The least cost from node x to node a is __.  </span>
    <span class="gray-text">• The least cost from node x to node b is __.</span>
    <span class="gray-text"></span>
- <span class="gray-text">Consider the DV routing scenario with costs Cxu = 9, Cxv = 3, Cxw = 9 and vectors Du(a,b)=(9,7), Dv(a,b)=(6,4), Dw(a,b)=(4,4).  </span>
    <span class="gray-text">• The LCP from node x to node a is through node __.</span>

