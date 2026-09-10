second layer in the OSI model 
> [!abstract] One-line summary
> second layer in OSI
> responsible for node to node transmission  
> major role error free transmission
> resposnible for encoding and decoding


DLL is divided further into two more layers :
1. logical link layer :- deals with multiplexing ,flow of the data and also responsible for error and acknowledgment
2. media access control : this layer is respnosible for the device interactions and the ==**Frame addressing**== and physical media access 
   this layer recieves the packets from the network layer and coverts them in the frames and ttransfers them to the physical layer bit by bit 

## Protocols in Data link layer

There are various [protocols in the data link layer](https://www.geeksforgeeks.org/computer-networks/examples-of-data-link-layer-protocols/), which are as follows:

- [Synchronous Data Link Protocol (SDLC)](https://www.geeksforgeeks.org/computer-networks/basic-frame-structure-of-sdlc/)
- [High-Level Data Link Protocol (HDLC)](https://www.geeksforgeeks.org/computer-networks/basic-frame-structure-of-hdlc/)
- [Serial Line Interface Protocol (SLIP)](https://www.geeksforgeeks.org/computer-networks/slip-full-form/)
- [Point to Point Protocol (PPP)](https://www.geeksforgeeks.org/computer-networks/point-to-point-protocol-ppp-encapsulation/)
- [Link Access Procedure (LAP)](https://www.geeksforgeeks.org/computer-networks/link-access-procedure-lap-protocols/)
- Link Control Protocol (LCP)
- [Network Control Protocol (NCP)](https://www.geeksforgeeks.org/computer-networks/network-control-protocol-ncp/)
  
  ## Devices Operating at the Data Link Layer
- switch
- bridge
- NIC
- WAP
- layer 2 switch 
  
>   Note: The Data Link Layer can be targeted by attacks like MAC spoofing or ARP poisoning. Understanding how devices and frames operate at this layer helps detect and mitigate such threats.  

## Limitations of Data Link Layer

- ****Limited Scope****: It operates only within a local network and cannot handle end-to-end communication across different networks.
- ****Increased Overhead****: Adding headers, trailers, and redundant data (for error correction) increases the size of transmitted data.
- ****Error Handling Dependency****: While it can detect and correct some errors, it relies on upper layers for handling more complex issues.
- ****No Routing Capability****: The Data Link Layer cannot make routing decisions. It only ensures delivery within the same network segment.
- ****Resource Usage****: Flow control and error correction mechanisms may consume extra processing power and memory

## Applications of Data Link Layer

- ****Local Area Networks (LANs)****: Enables reliable communication between devices within a local network using protocols like Ethernet (IEEE 802.3).
- ****Wireless Networks (Wi-Fi)****: Manages communication between devices in wireless networks via protocols like IEEE 802.11 hence, handling media access and error control.
- ****Switches and MAC Addressing****: Facilitates the operation of switches by using MAC addresses to forward data frames to the correct device within the network.
-  **Point-to-Point Connections*: Used in protocols like PPP (Point-to-Point Protocol) to establish and manage direct communication between two nodes.