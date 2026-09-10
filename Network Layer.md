

> [!abstract] One-line summary
> responsible for logical addressing, routing, and end-to-end packet delivery across interconnected networks.
> - handles IP
> - decicdes optimal route 
> - hosts to hosts communication 

# key resposnsiblity
- logicall address : - assigning the ip addr 
- packetizattion : converts segments into packets 
- host to host delivery 
- forwarding :- forwards the packet from the recived interface to the correct interface 
- routing :- decides the optimal path for the packet to travel 
- fragmantation and defragmentation : divides the large packet into the MTU and re assembles them at the destination 
- subnetting : dividesthe large networks into the smaller networks 
-  NAT : maps private ip to public ip to conserve the ip addrs 

## Protocols Operating at the Network Layer

- ****IP (Internet Protocol - IPv4/IPv6):**** Provides logical addressing and delivers packets across networks; IPv6 offers a larger address space and better efficiency.
- ****ICMP (Internet Control Message Protocol):**** Sends error reports and diagnostic messages (e.g., destination unreachable, ping).
- ****ARP (Address Resolution Protocol):**** Maps IP addresses to MAC addresses within a local network.
- ****RARP (Reverse Address Resolution Protocol):**** Retrieves a device’s IP address using its MAC address (largely obsolete).
- ****NAT (Network Address Translation):**** Converts private IP addresses to public IPs, conserving addresses and improving security.
- ****IPSec (Internet Protocol Security):**** Secures IP communication through encryption and authentication.
- ****MPLS (Multiprotocol Label Switching):**** Uses labels to forward packets efficiently and manage traffic.
# routing protocols 
- RIP (routing information protocol) : - uses hop cont , distance vector 
- OSPF (open shortest path first ) : -link state protocol uses the shortest path using netwrok topology 
- BGP(border gateway protocol ): routes data between autonoums systems on the inernet 

## Limitations of the Network Layer

- No flow control mechanism; congestion may occur if too many datagrams are in transit.
- Limited error control; mainly relies on upper layers for reliability.
- Routers may drop packets under heavy load, leading to possible data loss.
- Fragmentation increases processing overhead and may affect performance.

## Difference Between Routing and Flooding

|Routing|Flooding|
|---|---|
|A routing table is required.|No Routing table is required|
|May give the shortest path.|Always gives the shortest path.|
|Routing is less reliable|Flooding is more reliable|
|Traffic is less in Routing|Traffic is more in Flooding|
|Duplicate packets are not present|Duplicate packet are present|
