Ethernet is a primary wired networking standard , it provides framing ,media access control and scale able physical layer 

## Ethernet (IEEE 802.3) Frame Format
![[Pasted image 20260910151238.png]]
- preamble : 0 and 1 indicating the receiver that a frame is incoming and the locking it also allow for the synchronization of both parties

- start of frame (SFD) : 1-byte field containing 10101011.indicating the upcoming bits are the start of the frame and it is last chance to synchronize

- destination Add : 6 bytes that contain the mac address 
- source Add : 6 byte that contains the source address , it is individual add in uni-cast and always starts with 0
- length : Length is a 2-byte field indicating the length of the frame, can hold value up-to 65535 but length cant be grater than 1500 bytes 
- data: AKA payload both IP and data is here if IP is used , max length 1500 and min length 46 bytes and 0's padding is added 
- Cyclic redundancy check (CRC or FCS ):4 byte field - 32 bit hash code generated over the destination,source,length,data field ,if the checksum generated destination is not same data is corrupted 
- vlan tag : 4 - byte which is inserted after source add 
- jumbo frames : frames with payload larger than 1500 bytes, supported by only some devices and will increase networks throughput because of less over head 
- multicast frames : multicast group of devices and broadcast is all devices on network

### CAM table 
content addressable memory a high speed memory in side switch that maps mac address to physical port or VLAN

### MAC table 
a database where in switches where is stores the physical address  to specific port 

### MTU 
Maximum transmission unit largest size of packet you can send over the network 

# security 
- MAC spoofing : 
	 changing the device physical address to imitate other device 
- ARP attack :
	 sending fake ARP messages to link the IP of the legitimate device like router 
- VLAN hopping:
	 attack which allows attacker to listen to unauthorised vlan wit =hout going through router