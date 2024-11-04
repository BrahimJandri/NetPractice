# NetPractice
Introduction This project is a general practical exercise to let you discover networking.

# TCP — Transmission Control Protocol
Is a protocol that ensures a reliable data transfer, it ensures that the data being transferred arrives and in the correct order.

# IP — Internet Protocol
Is a unique address that define the identity of the devices when is connected to the internet. It is responsible for addressing and routing data packets across the network.

There are two types of IP (Ipv4 & Ipv6), Ipv4 is a 32-bit number divided into 4 block (4 octet) each 8-bits.

The IP address has two main parts: the Host ID, and the Network ID.

![image](https://github.com/user-attachments/assets/1134d570-f2d9-46d7-8555-a09150ecd16e)

Classful Addressing is a way of organizing and managing IP Addresses.

Class A (first bit is 0), range: 0000 0000 to 0111 1111
Class B (first two bits is 10), range: 1000 0000 to 1011 1111
Class C (first three bits is 110), range: 1100 0000 to 1101 1111
Class D (first four bits is 1110), range: 1110 0000 to 1110 1111
Class E (first three bits is 1111), range: 1111 0000 to 1111 1111

# Private Networks
They are Networks reserved for internal use with organization or home or small office network.
- 10.0.0.0 - 10.255.255.255
- 172.16.0.0 - 172.31.255.255
- 192.168.0.0 - 192.168.255.255

# Loop-back Addresses
They are addresses that are reserved for internal testing and communication within a device, like when using 127.0.0.1 ‘localhost’ for accessing the device itself.
- 127.0.0.0 — 127.255.255.255

# What is a Switch?
A switch is a device that connects multiple devices in a single network. Unlike router, the switch it only purpose is to distribute packets in its local network.

# What is a Router?
A router is a device that connects two or more IP Networks. Each network that a router connects to is linked through an interface, which can be a physical port or a wireless connection.

# What is TCP/IP Model?
This is the Model that all the devices uses today, it is a model that defines how data will be transferred from the sender to the receiver.

This Model is similar to the OSI Model which uses all the 7 layers that we talk about, but this Model only uses 4 layers.

![image](https://github.com/user-attachments/assets/fb76698e-5fa3-4ba5-a8d0-ec048e055392)


