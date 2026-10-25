# The Principles of Network Addressing

## Key Concepts

- Network addressing ensures data travelling from one device gets to the correct destination
- There are 2 main types of network addresses which are physical addresses and logical addresses, with each serving a unique function in the delivery of data
- a physical address is a hardware identifier that is burned into a device's **network card (NIC)**, while a logical address is assigned to a device by the network, which can change depending on where it connects 

### Physical Network Address

- This is referred to as Media Access Control or **MAC Address**
- Every device that can connect to a network has a unique MAC which does not change even if a user connects to a different WI-FI network.
- A MAC Address is a 48-bit pattern with the first 24 identifying the NIC's manufacturer and the last 24 indicating the individual board number. The figure below shows the MAC Address in hexadecimal and binary.
![alt text](<images/MAC Address bit pattern.png>)



### Logical Network Address

- This is otherwise known as an Internet Protocol (IP) Address and is useful for helping direct data to the correct place
- The 2 main versions used today are version 4 and version 6 (IPv4 and IPv6 respectively)
- An IP Address is not fixed to a device like a MAC Address e.g. A phone wiil have a different IP Address when it connects to one WI-FI then to another.

**IPv4** Addresses are written as 4 numbers, each ranging from 0 to 255, and the size of them is 32 bits. As seen in the image below, one part represents the network, and the other represents the host. 
![alt text](<images/IPv4 Address.png>)

**IPv6** Addresses were created due to the significant increase in internet-connected devices and use a 128 bit pattern, which therefore gives it a greater range of addresses.

## Numbering Systems