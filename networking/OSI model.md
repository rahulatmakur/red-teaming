# Open systems interconnection 

> [!abstract] One-line summary
> OSI model is the conneptual structure created by the ISO to describe how the data is transmiited across the network using 7 layers 

## Why does it exist?

it helps to explain how the communication is done between to devices, it has divided the stages in the the communction for the easier understanding  

## How does it work?

![[Pasted image 20260829165703.png]]
## Important components

| Layer                  | Working                                                                                 | Protocol Data Unit (PDU)         | Protocols                     |
| ---------------------- | --------------------------------------------------------------------------------------- | -------------------------------- | ----------------------------- |
| [[Physical Layer]]     | Establishes physical connection between devices and transmits raw bits over the medium. | Bits                             | USB, SONET/SDH                |
| [[Data Link Layer]]    | Provides node-to-node delivery and error detection/correction.                          | Frames                           | Ethernet, PPP, PPTP           |
| [[Network Layer]]      | Handles logical addressing and routing of data between different networks.              | Packets                          | IP, ICMP, IGMP, OSPF          |
| [[Transport Layer]]    | Ensures end-to-end communication, segmentation, flow control, and error handling.       | Segments (TCP) / Datagrams (UDP) | TCP, UDP, SCTP                |
| [[Session Layer]]      | Establishes, manages, and terminates communication sessions between applications.       | Data                             | RPC                           |
| [[Presentation Layer]] | Translates, encrypts, and formats data for the application layer.                       | Data                             | TLS/SSL, MIME                 |
| [[Application layer]]  | Provides network services directly to end-user applications.                            | Data                             | FTP, SMTP, DNS, DHCP, NetBIOS |
