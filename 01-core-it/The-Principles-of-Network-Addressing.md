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

Different numbering systems are used to represent network addresses. IPv4 addresses are written using decimal and MAC Addresses use **hexadecimal**.

**Hexadecimal** is often used in computing to represent large binary numbers in a more compact and human-readable format, such as in MAC addresses. It is a number system that uses 16 digits: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F. The value of the letters continues the sequence, with A = 10, B = 11, and so on.

**Binary** is a numbering system that only uses 2 digits, 1 and 0. To a network device, both IPv4 and Mac Addresses are read and stored as binary. The other numbering systems are used to make it easier for people to represent and communicate network addresses.

**Binary Explained**
In a decimal number, such as 3452, the value of each digit is calculated by its place in the sequence of numbers, which gets multiplied by 10 each time you go to the left and starting with 1 on the furthest right. So 3 x 1000, 4 x 100, 5 x 10, 2 x 1, adding them up, giving you 3452. **Binary** works just like decimal, but because it’s only got two digits (0 and 1), it’s based on the value 2 rather than 10. For example, the binary number 11011, has five digits, and it’s the equivalent of the decimal number 27.

**Converting binary to decimal**

Just like decimal, each place in that sequence has a place value. It starts on the right, with the place value of 1. Each subsequent place value going left in the sequence is the previous place value multiplied by 2. So in a 5 digit binary number like 11011, to convert it into decimal, you can start from the left with **1** x 16, **1** x 8, **0** x 4, **1** x 2, and **1** x 1 - adding them up would then give the decimal number 27.

**Converting hexadecimal to decimal**

In hexadecimal, each digit’s position represents a different power of 16. The rightmost digit is multiplied by 16⁰ (which is 1), the next digit to the left is multiplied by 16¹ (which is 16), then 16² (which is 256), and so on.

For example, in the hexadecimal number A3F:

F is in the rightmost place, so it’s 15 × 1.
3 is next, so it’s 3 × 16.
A is next, so it’s 10 × 256.
Add them up: 2560 (A) + 48 (3) + 15 (F) = 2623 in decimal

**Converting decimal to binary**

To convert from decimal into binary, you can use the method of successive division by 2. This involves dividing the decimal number by 2, recording the remainder, and then continuing the process with the quotient until you reach a quotient of 0. The binary number is then formed by reading the remainders in reverse order.

Here's a step-by-step example of converting the decimal number 45 into binary:

Divide the number by 2 and write down the remainder:

45 ÷ 2 = 22 remainder 1

Divide the quotient from the previous step by 2 and record the remainder:

22 ÷ 2 = 11 remainder 0

Repeat the process with the new quotient:

11 ÷ 2 = 5 remainder 1

Continue dividing and recording the remainders:

5 ÷ 2 = 2 remainder 1

2 ÷ 2 = 1 remainder 0

1 ÷ 2 = 0 remainder 1

Now, write the remainders in reverse order to get the binary equivalent:

45 in decimal is 101101 in binary.

**Converting decimal to hexadecimal**

To convert decimal to hexadecimal, you would follow the same steps as before but, dividing by 16 as opposed to 2, and since in hexadecimal, numbers from 10 to 15 are represented by the letters A to F - This also applies to remainders here.

To convert the decimal number 4924 to hexadecimal, follow these steps:

Divide the decimal number by 16 and keep track of the quotient and the remainder:

4924 ÷ 16 = 307 remainder 12

Note that in hexadecimal, remainders from 10 to 15 are represented by the letters A to F. So, a remainder of 12 is written as C.

Repeat the process with the new quotient:

307 ÷ 16 = 19 remainder 3

Continue dividing and recording the remainders:

19 ÷ 16 = 1 remainder 3

1 ÷ 16 = 0 remainder 1

Now, write the remainders in reverse order to get the hexadecimal equivalent:

The remainders are 1, 3, 3, C. In reverse order, they form the hexadecimal number 133C.

Therefore, the decimal number 4924 is equivalent to 133C in hexadecimal.