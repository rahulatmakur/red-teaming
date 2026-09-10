
> [!abstract] One-line summary
> layer 4 providing the reliable , ordered ,effiecient communication from end to end 
>  

- Operates at Layer 4 (Transport Layer) of the OSI model
- Enables process-to-process communication using port numbers
- Ensures reliability through error control, sequencing, and retransmission
- Supports flow control to prevent receiver overload
- Uses protocols like TCP, UDP, and SCTP for different application needs

## 3-Way Handshake

The 3-Way Handshake ensures both client and server are ready before data transmission begins:

****Step 1: SYN (Client -> Server)****

- Client sends a TCP segment with SYN=1, including its ISN (Initial Sequence Number).
- Marks the request to initiate a connection

****Step 2****: SYN‑ACK (Server -> Client)

- Server replies with SYN=1 & ACK=1, containing its own ISN and ACK = client_ISN + 1.
- Confirms receipt of client’s SYN and initiates its own sync

****Step 3: ACK (Client -> Server)****

- Client sends an ACK=1 segment with ACK = server_ISN + 1.
- Completes synchronization; connection enters ESTABLISHED state

## Transport Layer Protocols

Transport Layer Protocol uses different protocol for the better communication between two ends uses of protocol may differ from specifications. Below mention are some protocols used in Transport Layer

### 1. Transmission Control Protocol(TCP)

- ****TCP**** is connection-oriented Protocol.
- TCP is reliable protocol.
- As [TCP](https://www.geeksforgeeks.org/computer-networks/what-is-transmission-control-protocol-tcp/) is connection-oriented protocol, so first the connection is established between two ends and then data is transferred and then the connection is terminated after all data being sent.

### 2. User Datagram Protocol (UDP)

- UDP is not reliable protocol
- The protocol [UDP](https://www.geeksforgeeks.org/computer-networks/user-datagram-protocol-udp/) is connectionless.
- When speed and size are more important than security and dependability, this kind of protocol is employed.
- The data from the higher layer is supplemented with transport-level addresses, checksum error control, and length information by UDP, an end-to-end transport level protocol.
- A user datagram is the packet that the UDP protocol generates.

### 3. Stream Control Transmission Protocol (SCTP)

- Many Internet applications use SCTP to perform transport layer duties, similar to User Datagram Protocol (UDP) and Transmission Control Protocol (TCP).
- On top of a connectionless packet network like IP, SCTP is a dependable transport protocol that facilitates data transfer over the network in scenarios involving one or more IP addresses.