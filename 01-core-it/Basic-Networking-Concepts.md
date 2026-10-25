# Basic Networking Concepts

## Key Concepts

- A network is a collection of computing devices that can communicate with each other

- Some benefits of Networking are resource sharing, ease of communication, and internet access.

- There are 2 basic types of computer networks: Peer-to-Peer networks and Client-Server network

## Peer-to-Peer Networks

In a P2P network, each computer acts as a server, each equally being able to provide data

Some advantages of establishing a P2P network are:

- They're easy to install and configure
- Don't require a dedicated server or administrator
- Don't require additional equipment or software to operate

These advantages make P2P networks ideal for sharing resources among a small group of users, however, they also come with some disadvantages which are:

- Computers who share resources can possibly face reduced performance
- No centralised organisation to manage access to data
- Security applies to a single resource at a time e.g. one login per resource

## Client-Server Network

In a Client-Server network, one computer is established as the server, responding to requests from other machines i.e. clients, in the network. An example of this, is any website, websites are typically hosted on web servers - A web browser acts as the client that requests data from the server, with the server responding and sending the webpage data back.

A Client-Server Network inverts the disadvantages of P2P Networks, by offering greater control over data and only requiring a single network login to access different resources.

This type of network is not without its own disadvantages however, the centralised aspect of it can also be detrimental. This is because a single server failure, could render a network unstable, which in turn, causes a loss of network resources. Client-Server networks also require dedicated hardware and specialised software, making them a more expensive option relative to P2P Networks.

## Local and Wide Area Networks

- These titles are used to categorise networks according to their scale
- Local Area Networks (LAN), are one of the most common, and are typically within a single building or site
- Wide Area Networks (WAN), are essentially a collection of LANs, and are used to connect computers over a greater distance

## Network Topologies

- A network topology describes how computers and devices in a network are linked together
- There are 4 main network topologies which are: Bus, Star, Ring, Mesh

**Bus Networks** were typically used in early networking, with a single cable connecting each device to the network. A major risk of this topology is that a single computer failure or cable damage can bring down the entire network.
![alt text](<images/Bus Networks.png>)



**Star Networks** are common in modern networking, where each computer is connected to a central device, such as a hub, switch, router. This offers more resilience relative to Bus Networks, as the failure of one device does not disrupt the entire network.
![alt text](<images/Star Networks.png>)



**Ring Networks** consist of each computer being connected to others in a closed loop. This type of network can be resilient if data can travel in both directions as it means that if a single failure occurs, data can still travel in the other direction. 
![alt text](<images/Ring Networks.png>)



**Mesh Networks** are used for critical operations where minimising downtime is a priority. Each computer is connected to every other computer without a central connecting device.
![alt text](images/Mesh.png)

## Network Components

Networks are made up of components that work together to facilitate communication and data exchange between devices. Networks are typically made up of the following components: Devices, Media, Networking Hardware, Protocols and Services.

### Devices

**Devices** are generally split into 2 categories, **Endpoints/end-user** devices and **Intermediate/Intermediary** Devices.

**Endpoints** are devices that connect to a computer network and serve as sources or destinations of data so they are significantly important to the overall functionality of the network. Some common types of **endpoints** are:

- Desktops and laptops
- Servers such as file servers, web servers, and database servers.
- Mobile devices such as smartphones and tablets

**Intermediary** devices facilitate the communication and data exchange. They manage and secure traffic by directing data between different devices. Some common types of these devices are:

- Switches connect devices within the same network, enabling efficient data exchange
- Routers connect different networks together, such as connecting a local network to the internet
- **Wireless Access Points (WAP)** and **controllers (WLC)** allow wireless devices to communicate with each other and facilitate communication with wired networks

### Media

**Media** refers to the method itself of connecting devices together. There are 2 main types of this, which are:

- Cables (Ethernet, Fibre Optic), with the different types of cables being used to transmit data at various speeds and distances
- Wireless (Wi-Fi, Bluetooth), where radio waves or other wireless technologies are used to transmit data

### Networking Hardware

**Networking Hardware** is the equipment that enables networked devices to communicate with each other. This includes:

- **Network Interface Cards (NICs)** enable devices to connect to the network either wired or wirelessly and are typically used by **endpoints**
- **Modems** convert digital data from a computer into analogue signals for transmission over telephone lines
- **Interfaces/Ports** enable **intermediary devices** to connect to other devices on a network. These interfaces can be either wired or wireless and use various protocols for communication.

### Protocols and Services

**Protocols and services** are the rules and conventions that govern the network. Examples of them include:

- Transmission Control Protocol/Internet Protocol (TCP/IP): The core set of rules that allows devices to exchange daya over networks, including the internet.
- Hypertext Transfer Protocol/Hypertext Transfer Protocol Secure (HTTP/HTTPS): The protocol web browsers and servers use to request and deliver web pages. HTTPS is the secure version and adds encryption via **TLS** so that data exchanged like passwords or payment details, can't easily be read or tampered with by anyone.

Easy way to remember: TCP/IP would be responsible for delivering the password itself to a particular website's serber by breaking it down into packets first. HTTP/HTTPS define what the browser and website say to each other i.e. the browser's login prompt and the server's successul or invalid password response - https does this with encryption.

### Hubs, Switches, and Routers

**Hubs** take data in one port and blast it out to every other port, whether or not they need it as it does not know who is connected where. This can cause congestion and weak security.

**Switches** learn which device (by MAC address) is on which port and send data only to the intended recipient. For example, if your laptop sends something to your printer, since the address of the printer is on the home network, the traffic is handled locally

**Routers** connect different networks together and direct traffic between them using **IP addresses**, deciding if the traffoc goes out to the **ISP**. 

Essentially, the **switch** will handle local delivery while the router handles anything headed to another network.

### Network Messages

There are 3 main categories for the types of messages that are communicated over a network, which are Unicast, Multicast, and Broadcast. These types each correspond to the intended recipient/s, in terms of the number of them, of a particular message.

## Network Security

Two key methods of securing data and protecting against attacks are **encryption** and **firewalls**

**Encryption** - A message is encoded in a way in which only someone with a key can decrypt it. This means that even if someone intercepts the data, it's stil unreadable without the key. The purpose of this is confidentiality.

**Firewalls** - Use a set of criteria as filters and decides what type of traffic to let in and out of devices, meaning that they sit between a trusted network (e.g. your home network) and an untrusted one (e.g. the internet). These criteria are usually rules based on things like **IP addresses**, **ports**, or **protocols**. The purpose of this is to provide protection from unauthorised access.


