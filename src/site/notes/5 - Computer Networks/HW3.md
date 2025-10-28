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
> data

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



- The __ flag in the header of an IPv4 datagram is set to 1 in the first of many fragments.
    
- The M flag in the header of an IPv4 datagram is set to __ in the last of many fragments.
    
- The __ flag in the header of an IPv4 datagram is set to 1 if the datagram is not to be fragmented.
    
- In an IPv4 datagram with a 24-byte header, the HEX representation of the first 8 bits in the header is __.
    
- In an IPv4 datagram with a 32-byte header, the HEX representation of the first 8 bits in the header is __.
    
- In an IPv4 datagram with a 36-byte header, the HEX representation of the first 8 bits in the header is __.
    
- In an IPv4 datagram with a 40-byte header, the HEX representation of the first 8 bits in the header is __.
    
- In an IPv4 datagram with a 44-byte header, the HEX representation of the first 8 bits in the header is __.
    
- In an IPv4 datagram with a 60-byte header, the HEX representation of the first 8 bits in the header is __.
    

### DHCP

- In the first step of the DHCP process, the client sends a DHCP __ message, to which the server replies with a DHCP offer message.
    
- In the first step of the DHCP process, the client sends a DHCP discover message, to which the server replies with a DHCP __ message.
    
- In the DHCP discover message, the source IP address is __ and the destination IP address is 255.255.255.255
    

### IPv6 addressing: expansion & compression

- The full length IPv6 address obtained from the shortened notation AABB::A00:B10:E11 is the following: __. Use the colon-separated HEX notation.
    
- The full length IPv6 address obtained from the shortened notation AABB:0:0:AB11::E11 is the following: __. Use the colon-separated HEX notation.
    
- <span class="gray-text">The full length IPv6 address obtained from the shortened notation AABB:0:0:AB11::E11 is the following: __. Use the colon-separated HEX notation.</span>
    
- The shortest notation of the IPv6 address AB11:0:BB11:0:0:0:0:EE11 is the following: __. Use the colon-separated HEX notation.
    
- <span class="gray-text">The shortest notation of the IPv6 address AB11:0:0:BB11:0:0:0:EE11 is the following: __. Use the colon-separated HEX notation.</span>
    <span class="gray-text"></span>
- <span class="gray-text">The shortest notation of the IPv6 address AB11:0:BB11:0:0:0:0:EE11 is the following: __. Use the colon-separated HEX notation.</span>
    <span class="gray-text"></span>
- The three important types of IPv6 addresses are the __ addresses, the anycast addresses, and the multicast addresses.
    
- The three important types of IPv6 addresses are the unicast addresses, the anycast addresses, and the __ addresses.
    
- IPv4 addresses are 32-bit long whereas IPv6 addresses are __-bit long.
    
- IPv4 addresses are __-bit long whereas IPv6 addresses are 128-bit long.
    

### Classful IPv4 default masks (CIDR)

- In the classful IPv4 addressing, the default subnet mask for the address 45.3.2.1 is /__. Use the CIDR notation.
    
- <span class="gray-text">In the classful IPv4 addressing, the default subnet mask for the address 45.3.2.1 is /__. Use the CIDR notation.</span>
    
- In the classful IPv4 addressing, the default subnet mask for the address 193.3.2.1 is /__. Use the CIDR notation.
    
- <span class="gray-text">In the classful IPv4 addressing, the default subnet mask for the address 193.3.2.1 is /__. Use the CIDR notation.</span>
    

### NAT / private addressing

- If the address block 10.x.y.z/24 is used by an organization, a __ router must be used before any IP packets originating from within this organization is forwarded into the public internet.
    

### ICMP and NL troubleshooting tools

- __ is an application that uses on ICMP Echo Request and Echo Reply messages to check the NL connectivity between two nodes.
    
- __ is an application that uses ICMP error-reporting messages to determine the number of routers between a source and a destination.
    
- __ is an application that uses ICMP error-reporting messages to determine the number of routers between a source and a destination.
    
- __ is a protocol used for query messaging and error reporting by the network layer. It runs directly over IP. Your answer must be an acronym.
    

### Routing protocols & algorithms (DV/LS/instability/mitigation)

- In a network that runs __ routing protocol, the link cost is inversely proportional to its bit rate. Your answer must be an acronym.
    
- In a network that runs __ routing protocol, the maximum number of hops is 15. Your answer must be an acronym.
    
- __ is a routing protocol that uses a composite metric that is based on delay, bandwidth, reliability, and load. Your answer must be an acronym.
    
- __ is a Cisco proprietary routing protocol that uses DV algorithm to find the LCPs in a network. Your answer must be an acronym.
    
- __ algorithm is used by global routing protocols. It requires that every node be aware of the entire network topology and the cost of its links. Your answer must be an acronym.
    
- __ algorithm is used by decentralized routing protocols. The nodes need not be aware of the entire network topology. They simply rely on updates from their immediate neighbors. Your answer must be an acronym.
    
- __ is a two-node instability problem that networks running RIP protocol can suffer from. Your answer must be an acronym.
    
- Like split horizon, __ is a technique that could be used to mitigate the CTI instability problem.
    
- Like poisoned reverse, __ is a technique that could be used to mitigate the CTI instability problem.
    
- In DV routing, if a node X receives an update about a cost from the same neighbor, then X takes the __ value of the cost. Choose either "oldest", "latest", "smallest", or "highest".
    

### IPv4 fragmentation (number of fragments)

- A standard IPv4 datagram with a total length equal to 5800 bytes arrives to a router output port whose MTU is 1220 bytes. The number of fragments leaving this router port is equal to __.
    
- A standard IPv4 datagram with a total length equal to 4800 bytes arrives to a router output port whose MTU is 660 bytes. The number of fragments leaving this router port is equal to __.
    
- A standard IPv4 datagram with a total length equal to 7800 bytes arrives to a router output port whose MTU is 2940 bytes. The number of fragments leaving this router port is equal to __.
    
- A standard IPv4 datagram with a total length equal to 6800 bytes arrives to a router output port whose MTU is 2020 bytes. The number of fragments leaving this router port is equal to __.
    
- A standard IPv4 datagram with a total length equal to 5800 bytes arrives to a router output port whose MTU is 1380 bytes. The number of fragments leaving this router port is equal to __.
    
- A standard IPv4 datagram with a total length equal to 5800 bytes arrives to a router output port whose MTU is 2180 bytes. The number of fragments leaving this router port is equal to __.
    
- A standard IPv4 datagram with a total length equal to 6800 bytes arrives to a router output port whose MTU is 1420 bytes. The number of fragments leaving this router port is equal to __.
    

### Subnetting: network & broadcast addresses

- Consider a LAN interface with the IPv4 address 188.165.250.245/19. The network address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 125.125.175.3/18. The network address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 60.33.12.1/26. The broadcast address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 188.165.250.245/21. The network address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 168.255.255.245/23. The network address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 60.33.12.1/25. The broadcast address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 33.60.250.1/22. The broadcast address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 12.6.128.25/19. The broadcast address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 12.6.128.25/20. The broadcast address in this LAN is __.
    

### EIGRP metrics (bandwidth & delay)

- A network path, composed of many links, has a minimum bit rate of 10 Mbps and a total delay of 10 milliseconds. Compute the EIGRP bandwidth and delay metrics for this path.  
    • EIGRP bandwidth metric is __.  
    • EIGRP delay metric is __.
    
- A network path, composed of many links, has a minimum bit rate of 10 Mbps and a total delay of 6 milliseconds. Compute the EIGRP bandwidth and delay metrics for this path.  
    • EIGRP bandwidth metric is __.  
    • EIGRP delay metric is __.
    
- A network path, composed of many links, has a minimum bit rate of 10 Mbps and a total delay of 5 milliseconds. Compute the EIGRP bandwidth and delay metrics for this path.  
    • EIGRP bandwidth metric is __.  
    • EIGRP delay metric is __.
    
- A network path, composed of many links, has a minimum bit rate of 16 Mbps and a total delay of 13 milliseconds. Compute the EIGRP bandwidth and delay metrics for this path.  
    • EIGRP bandwidth metric is __.  
    • EIGRP delay metric is __.
    
- A network path, composed of many links, has a minimum bit rate of 16 Mbps and a total delay of 14 milliseconds. Compute the EIGRP bandwidth and delay metrics for this path.  
    • EIGRP bandwidth metric is __.  
    • EIGRP delay metric is __.
    

### Distance-Vector (DV) routing scenarios

- Consider the DV routing scenario shown below with the costs Cxu = 5, Cxv = 10, and Cxw = 5. The respective minimum distance vectors from (u, v, w) to (a, b) are: Du(a, b) = (9, 8), Dv(a, b) = (8, 8), and Dw(a, b) = (8, 7). Compute the least cost from node x to node a and the least cost from node x to node b.  
    `image016642558fc.jpg`  
    • The least cost from node x to node a is __.  
    • The least cost from node x to node b is __.
    
- Consider the DV routing scenario shown below with the costs Cxu = 11, Cxv = 3, and Cxw = 7. The respective minimum distance vectors from (u, v, w) to (a, b) are: Du(a, b) = (4, 6), Dv(a, b) = (6, 6), and Dw(a, b) = (11, 8). Compute the least cost from node x to node a and the least cost from node x to node b.  
    `image018642558fc.jpg`  
    • The least cost from node x to node a is __.  
    • The least cost from node x to node b is __.
    
- Consider the DV routing scenario shown below with the costs Cxu = 11, Cxv = 6, and Cxw = 8. The respective minimum distance vectors from (u, v, w) to (a, b) are: Du(a, b) = (5, 6), Dv(a, b) = (6, 7), and Dw(a, b) = (5, 3). Compute the least cost from node x to node a and the least cost from node x to node b.  
    `image021642558fc.jpg`  
    • The least cost from node x to node a is 12.  
    • The least cost from node x to node b is 11.
    
- Consider the DV routing scenario shown below with the costs Cxu = 5, Cxv = 10, and Cxw = 5. The respective minimum distance vectors from (u, v, w) to (a, b) are: Du(a, b) = (9, 8), Dv(a, b) = (8, 8), and Dw(a, b) = (8, 7). Compute the least cost from node x to node a and the least cost from node x to node b.  
    `image016642558fc.jpg`  
    • The least cost from node x to node a is 13.  
    • The least cost from node x to node b is 12.
    
- Consider the DV routing scenario shown below with the costs Cxu = 3, Cxv = 10, and Cxw = 10. The respective minimum distance vectors from (u, v, w) to (a, b) are: Du(a, b) = (9, 4), Dv(a, b) = (9, 11), and Dw(a, b) = (10, 6). Compute the least cost from node x to node a and the least cost from node x to node b.  
    `image016642558fc.jpg`  
    • The least cost from node x to node a is 12.  
    • The least cost from node x to node b is 7.
    
- Consider the DV routing scenario shown below with the costs Cxu = 10, Cxv = 8, and Cxw = 3. The respective minimum distance vectors from (u, v, w) to (a, b) are: Du(a, b) = (5, 10), Dv(a, b) = (11, 6), and Dw(a, b) = (9, 6). Compute the least cost from node x to node a and the least cost from node x to node b.  
    `image018642558fc.jpg`  
    • The least cost from node x to node a is __.  
    • The least cost from node x to node b is __.
    


---



here you go—everything you pasted is included (even the repeats), grouped and with every answer spot replaced by `__` underlines for Obsidian.

### Router architecture & roles

- A typical IP router architecture comprises a routing processor, several I/O ports, and a switch __.
    
- A typical IP router architecture comprises a routing processor, several I/O ports, and a switch __.
    
- The main functions of IP routers are __ and forwarding.
    
- The devices that implement the network layer inside the internet core are called __.
    
- The devices that implement the network layer inside the internet core are called __.
    

### SDN, control/data planes

- In the SDN approach, modern routers implement the __ plane functions. Your answer must be an acronym.
    
- In the SDN approach, remote controllers, instead of the routers, implement the __ plane functions. Your answer must be an acronym.
    
- In the SDN approach, modern routers only implement the __ plane function.
    
- Routing is a control plane function whereas forwarding is a __ plane function.
    
- In the SDN (Software-Defined Network) approach, remote controllers implement the __ plane functions.
    

### IPv4 header: rows, fields, flags & first-byte HEX

- The second row of an IPv4 datagram header is dedicated to the process of __.
    
- The M flag in the header of an IPv4 datagram is set to 1 in the __ of many fragments.
    
- The M flag in the header of an IPv4 datagram is set to 0 in the __ of many fragments.
    
- The __ flag in the header of an IPv4 datagram is set to 1 if the datagram is not to be fragmented.
    
- In an IPv4 datagram with a 32-byte header, the HEX representation of the first 8 bits in the header is __.
    
- In an IPv4 datagram with a 20-byte header, the HEX representation of the first 8 bits in the header is __.
    
- In an IPv4 datagram with a 60-byte header, the HEX representation of the first 8 bits in the header is __.
    
- In an IPv4 datagram with a 40-byte header, the HEX representation of the first 8 bits in the header is __.
    
- In an IPv4 datagram with a 36-byte header, the HEX representation of the first 8 bits in the header is __.
    
- The TTL header field in an IPv4 datagram is used to prevent lost packets from staying inside the network indefinitely. Your answer must be an acronym: __.
    
- The TOS field in the header of an IPv4 datagram can be used to provide different classes of service inside the network. (Answer: __)
    
- In an IPv4 network that does not use priority classes, if a datagram has a 60-byte header and a total length of 515 bytes, then the HEX representation of the fields of the first header row is __.
    

### Addressing (IPv4 & IPv6)

- IPv4 addresses are 32-bit long whereas IPv6 addresses are __-bit long. Your answer must be an acronym.
    
- IPv4 addresses are 32-bit long whereas IPv6 addresses are __-bit long.
    
- The three important types of IPv6 addresses are the __ addresses, the anycast addresses, and the multicast addresses.
    
- The three important types of IPv6 addresses are __ addresses, __ addresses, and __ addresses.
    
- The full length IPv6 address obtained from the shortened notation __ is __.
    
- The shortest notation of the IPv6 address __ is __.
    
- The shortest notation of the IPv6 address __ is __.
    
- The network layer ensures that two hosts, even on __ networks, can still exchange packets.
    
- In the classful IPv4 addressing, the default subnet mask for the address 45.3.2.1 is /__.
    
- In the classful IPv4 addressing, the default subnet mask for the address 193.3.2.1 is /__.
    

(From your items, concretely:)

- The full length IPv6 address obtained from the shortened notation AABB::A00:B10 is __.
    
- The full length IPv6 address obtained from the shortened notation AABB::A00:B10:E11 is __.
    
- The shortest notation of the IPv6 address AB11:0:0:BB11:0:0:0:EE11 is __.
    
- The shortest notation of the IPv6 address AABB:CCDD:EEFF:0:0:0:AAAA is __.
    
- The shortest notation of the IPv6 address AABB:CCDD:EEFF:0:0:0:AAAA:BBBB is __.
    

### DHCP

- In the first step of the DHCP process, the client sends a DHCP __ message, to which the server replies with a DHCP offer message.
    
- In the DHCP discover message, the source IP address is __ and the destination IP address is __.
    

### NAT / private addressing

- If the address block 10.x.y.z/24 is used by an organization, a __ router must be used before any IP packets originating from within this organization are forwarded into the public internet.
    

### ICMP & troubleshooting tools

- __ is an application that uses ICMP Echo Request and Echo Reply messages to check the NL connectivity between two nodes.
    
- __ is a protocol used for query messaging and error reporting by the network layer.
    
- __ is a protocol used for query messaging and error reporting by the network layer. It runs directly over IP. Your answer must be an acronym.
    
- __ is an application that uses ICMP error-reporting messages to determine the number of routers between a source and a destination.
    

### Service model

- The network layer that follows the __ service model gives a best-effort, connectionless service to the transport layer.
    

### Routing protocols & algorithms (DV/LS/OSPF/RIP/EIGRP) + stability

- In DV routing, if a node X receives an update about a cost from different neighbors, then X takes the __ value of the cost. Choose either "oldest," "latest," "smallest," or "highest."
    
- In DV routing, if a node X receives an update about a cost from the same neighbor, then X takes the __ value of the cost. Choose either "oldest," "latest," "smallest," or "highest."
    
- __ is a technique that could be used to mitigate the CTI instability problem. (Like split horizon)
    
- __ is a technique that could be used to mitigate the Count-To-Infinity (CTI) instability problem. (Like poisoned reverse)
    
- __ is a standard IETF routing protocol that uses the DV algorithm to find the Least Cost Paths (LCPs) in a network.
    
- __ algorithm is used by decentralized routing protocols. The nodes need not be aware of the entire network topology. They simply rely on updates from their immediate neighbors. Your answer must be an acronym.
    
- __ algorithm is used by global routing protocols. It requires that every node be aware of the entire network topology and the cost of its links. Your answer must be an acronym.
    
- __ is a routing protocol that uses a composite metric that is based on delay, bandwidth, reliability, and load. Your answer must be an acronym.
    
- __ is a Cisco proprietary routing protocol that uses DV algorithm to find the LCPs in a network. Your answer must be an acronym.
    
- __ is a two-node instability problem that networks running RIP protocol can suffer from. Your answer must be an acronym.
    
- In a network that runs __ routing protocol, the link cost is inversely proportional to its bit rate.
    
- In a network that runs __ routing protocol, the maximum number of hops is 15.
    

### Subnetting: network & broadcast addresses

- Consider a LAN interface with the IPv4 address 188.165.250.245/20. The network address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 168.255.255.245/23. The network address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 125.125.175.3/29. The broadcast address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 33.60.150.1/28. The broadcast address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 60.33.12.1/15. The network address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 12.6.2.3/17. The network address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 12.6.128.25/19. The broadcast address in this LAN is __.
    
- Consider a LAN interface with the IPv4 address 125.125.175.3/29. The broadcast address in this LAN is __.  
    `125.125.175.3/29 -> 01111101.01111101.1010111.00000011`  
    `11111111.11111111.11111111.11111000`  
    `Network address -> 01111101.01111101.1010111.00000011` (fill result as __ if needed)
    

### IPv4 fragmentation: counts & payload size

- A standard IPv4 datagram with a total length equal to 7800 bytes arrives at a router output port whose MTU is 940 bytes. The number of fragments leaving this router port is equal to __.
    
- A standard IPv4 datagram with a total length equal to 12800 bytes arrives at a router output port whose MTU is 1220 bytes. The payload size of the last fragment leaving this router port is equal to __ bytes.
    
- A standard IPv4 datagram with a total length equal to 4800 bytes arrives to a router output port whose MTU is 820 bytes. The number of fragments leaving this router port is equal to __.
    
- A standard IPv4 datagram with a total length equal to 7800 bytes arrives to a router output port whose MTU is 2940 bytes. The number of fragments leaving this router port is equal to __.
    

### EIGRP metrics

- A network path, composed of many links, has a minimum bit rate of 10 Mbps and a total delay of 10 milliseconds. Compute the EIGRP metrics.  
    • EIGRP bandwidth metric is __.  
    • EIGRP delay metric is __.
    
- A network path, composed of many links, has a minimum bit rate of 10 Mbps and a total delay of 8 milliseconds. Compute the EIGRP metrics.  
    • EIGRP bandwidth metric is __.  
    • EIGRP delay metric is __.
    

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

