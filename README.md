# NetPractice
Introduction This project is a general practical exercise to let you discover networking.

# What is a TCP ?

TCP : Transmission Control Protocol (TCP) is a fundamental communication standard used in networking that ensures reliable data transmission between devices. It is part of the Internet 
protocol suite, commonly referred to as TCP/IP, which facilitates the interconnection of network devices.

# Key Features of TCP

- **Connection-Oriented Protocol**: TCP establishes a connection between two devices before data can be
sent. This connection setup ensures that both parties are ready to
communicate, which is crucial for reliable data exchange
- **Reliable Data Transmission**: One of the primary functions of TCP is to guarantee that data sent from one device reaches its destination accurately and in the correct order. It achieves this through mechanisms such as error checking and
retransmission of lost packets.
- **Flow Control and Congestion Control**: TCP manages the rate of data transmission between devices to prevent
overwhelming the network. It adjusts the flow of data based on the
network's current capacity, ensuring smooth communication    
- **Segmentation of Data**: TCP breaks down larger messages into smaller segments for transmission. Each segment is sent individually and reassembled at the destination,
which helps in managing large data transfers efficiently. <br>
In summary, TCP is essential for applications that require reliable 
communication, such as web browsing, email, and file transfers, making 
it a cornerstone of modern networking.

# What is an IP Address?

An IP address (Internet Protocol address) is a unique identifier assigned to each device connected to a network that uses the Internet Protocol for communication. It serves two main purposes:
Identification: It identifies a device on a network, allowing it to send and receive data.
Location Addressing: It provides information about the device's location within the network.
IP addresses come in two versions: IPv4 and IPv6. IPv4 addresses are written in a format called dotted-decimal notation, consisting of four octets (e.g., 192.168.1.1), while IPv6 addresses are longer and written in hexadecimal.

**Key Components of IP**

- **IP Address**: An IP address is a unique identifier assigned to each device connected
to a network. It allows devices to locate and communicate with one
another. IP addresses can be either IPv4 (32-bit) or IPv6 (128-bit)
formats, with IPv6 designed to accommodate the growing number of devices on the internet
- **Routing**: IP is responsible for routing data packets from the source device to
the destination device. It determines the best path for data to travel
across interconnected networks, ensuring that information reaches its
intended recipient efficiently.
- **Packet Structure**: Data transmitted over IP is broken down into smaller packets. Each
packet contains both the data being sent and the necessary addressing
information, allowing routers to direct the packets through the network. <br>
In summary, IP is essential for enabling communication between devices on 
the internet, providing a structured way to address and route data 
effectively.

# What is a Subnet Mask?

A subnet mask is a 32-bit number that divides an IP address into two parts: the network part and the host part. It helps determine which portion of the IP address refers to the network and which part refers to the specific device (host) within that network.
The subnet mask is also expressed in dotted-decimal format, similar to an IP address (e.g., 255.255.255.0). Each octet in the subnet mask can be either 255 (indicating that the corresponding bits in the IP address are part of the network) or 0 (indicating that the bits are part of the host).

# IP Address Structure
An IP address is a 32-bit number that uniquely identifies a host (such as a computer, printer, or router) on a TCP/IP network
. This address is akin to a postal address, enabling data to be routed to the correct destination
. The 32 bits are typically divided into four octets, each represented by a number between 0 and 255, separated by periods (e.g., 192.168.1.1).
