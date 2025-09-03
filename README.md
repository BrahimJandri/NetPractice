# NetPractice

**NetPractice** is an interactive educational tool designed to help students understand and practice networking concepts. This project is part of the École 42 curriculum and provides hands-on experience with TCP/IP networking, subnetting, routing, and network configuration through visual simulations.

![NetPractice](netpractice.png)

## 📋 Table of Contents

- [About](#about)
- [Features](#features)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Levels Overview](#levels-overview)
- [How to Use](#how-to-use)
- [Networking Concepts](#networking-concepts)
- [License](#license)

## 🎯 About

NetPractice is a practical exercise designed to help you discover and understand networking fundamentals. Through 10 progressive levels, you'll learn to configure network topologies, assign IP addresses, set up routing tables, and understand how data flows through networks.

### Key Learning Objectives:
- Understanding TCP/IP protocol suite
- IP addressing and subnetting
- Network routing and switching
- Network topology design
- Troubleshooting network connectivity

## ✨ Features

- **10 Progressive Levels**: From basic IP configuration to complex routing scenarios
- **Interactive Web Interface**: Visual network diagrams with editable configuration fields
- **Real-time Validation**: Immediate feedback on your network configurations
- **Educational Content**: Comprehensive networking theory and examples
- **42 School Integration**: Supports intranet login for personalized configurations

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Basic understanding of computer networks (helpful but not required)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/BrahimJandri/NetPractice.git
cd NetPractice
```

2. Open the main interface:
```bash
# Option 1: Open directly in browser
open net_practice/index.html

# Option 2: Serve with a local web server (recommended)
python3 -m http.server 8000
# Then visit http://localhost:8000/net_practice/
```

## 📁 Project Structure

```
NetPractice/
├── README.md                 # This file
├── netpractice.png          # Project screenshot
├── level1.json              # Level 1 configuration
├── level2.json              # Level 2 configuration
├── ...                      # Levels 3-10
├── level10.json             # Level 10 configuration
└── net_practice/            # Web application
    ├── index.html           # Main entry point
    ├── level1.html          # Level 1 interface
    ├── level2.html          # Level 2 interface
    ├── ...                  # Levels 3-10 interfaces
    ├── level10.html         # Level 10 interface
    ├── end.html             # Completion page
    ├── css/                 # Stylesheets
    ├── js/                  # JavaScript logic
    ├── img/                 # Images and diagrams
    └── License              # License information
```

## 📚 Levels Overview

The NetPractice exercises are organized into 10 levels of increasing difficulty:

- **Levels 1-3**: Basic IP addressing and simple networks
- **Levels 4-6**: Subnetting and network segmentation
- **Levels 7-8**: Routing between multiple networks
- **Levels 9-10**: Complex routing scenarios and advanced configurations

Each level presents a network topology where you must configure:
- IP addresses for network interfaces
- Subnet masks (CIDR notation)
- Routing tables
- Network connections

## 🖥️ How to Use

1. **Start the Application**: Open `net_practice/index.html` in your browser
2. **Enter Your Login** (optional): For 42 students, enter your intranet login
3. **Select a Level**: Choose from levels 1-10 or start with level 1
4. **Configure the Network**: 
   - Click on editable fields (highlighted in the interface)
   - Enter appropriate IP addresses, subnet masks, or routes
   - Follow CIDR notation for subnets (e.g., /24, /28)
5. **Validate**: Click "Check again" to verify your configuration
6. **Proceed**: Move to the next level once the current one is correctly configured

### Defense Mode
Leave the login field empty to access defense mode: 3 random levels (6-10) to solve in 15 minutes.

## 🌐 Networking Concepts

This section provides essential networking theory covered in NetPractice:

### TCP — Transmission Control Protocol
TCP is a protocol that ensures reliable data transfer, guaranteeing that data arrives at its destination in the correct order.

### IP — Internet Protocol
IP provides unique addresses that identify devices when connected to the internet. It's responsible for addressing and routing data packets across networks.

**IPv4 Structure**: A 32-bit number divided into 4 octets (8 bits each), with two main parts:
- **Network ID**: Identifies the network
- **Host ID**: Identifies the specific device on the network

![Network Structure](https://github.com/user-attachments/assets/1134d570-f2d9-46d7-8555-a09150ecd16e)

### Classful Addressing

IP addresses are organized into classes:

- **Class A** (first bit is 0): Range 0.0.0.0 to 127.255.255.255
- **Class B** (first two bits are 10): Range 128.0.0.0 to 191.255.255.255  
- **Class C** (first three bits are 110): Range 192.0.0.0 to 223.255.255.255
- **Class D** (first four bits are 1110): Range 224.0.0.0 to 239.255.255.255 (Multicast)
- **Class E** (first four bits are 1111): Range 240.0.0.0 to 255.255.255.255 (Reserved)

### Private Networks
Networks reserved for internal use within organizations or homes:
- **10.0.0.0/8**: 10.0.0.0 - 10.255.255.255
- **172.16.0.0/12**: 172.16.0.0 - 172.31.255.255
- **192.168.0.0/16**: 192.168.0.0 - 192.168.255.255

### Loopback Addresses
Reserved for internal testing and communication within a device:
- **127.0.0.0/8**: 127.0.0.0 - 127.255.255.255 (localhost)

### Network Devices

#### Switch
A device that connects multiple devices within a single network. Unlike routers, switches only distribute packets within their local network segment.

#### Router  
A device that connects two or more IP networks. Each network connection uses an interface (physical port or wireless connection).

### TCP/IP Model
The modern networking model used by all devices today, defining how data transfers from sender to receiver.

![TCP/IP Model](https://github.com/user-attachments/assets/fb76698e-5fa3-4ba5-a8d0-ec048e055392)

This model uses 4 layers (compared to OSI's 7 layers):
1. **Network Access Layer**
2. **Internet Layer**  
3. **Transport Layer**
4. **Application Layer**

### Subnetting
The process of dividing a network into smaller sub-networks.

#### Subnet Attributes:
- **Network ID**: First IP address in the subnet
- **Broadcast IP**: Last IP address in the subnet
- **First Host IP**: First usable IP (Network ID + 1)
- **Last Host IP**: Last usable IP (Broadcast IP - 1)
- **Next Network**: Network ID of the next subnet
- **IP Address Count**: Number of IPs in subnet
- **CIDR/Subnet Mask**: Network size notation

**Formula**: Number of IP addresses = 2^(32-CIDR)

#### Subnetting Cheat Sheet

1. **Start with powers of 2**: 1, 2, 4, 8, 16, 32, 64, 128
![Subnetting Step 1](https://github.com/user-attachments/assets/b5b341f1-16ce-4a43-9706-f846ac357104)

2. **Subtract from 256**: 256-1=255, 256-2=254, etc.
![Subnetting Step 2](https://github.com/user-attachments/assets/8fc45bef-8640-4454-8c41-95589aa96675)

3. **CIDR notation**: /32, /31, /30, etc.
![CIDR Notation](https://github.com/user-attachments/assets/4d7cab72-6999-4fc1-86c5-61874795684d)

4. **Complete reference table**:
![Subnetting Table](https://github.com/user-attachments/assets/14924fde-d78d-4828-a113-133303543fe3)

#### Example: 10.1.1.37/29
![Subnetting Example](https://github.com/user-attachments/assets/b1c5631c-a631-426d-b0f7-cdf69b4088af)

**Tips for calculating subnet information**:

1. **Find the group size and increment**:
![Calculation Tip 1](https://github.com/user-attachments/assets/c6c3be68-d523-4e18-b8ca-53325ab842c3)

2. **Use subnet values from the table**:
![Calculation Tip 2](https://github.com/user-attachments/assets/c8ac8d52-940f-4c41-a968-8312c395b072)

3. **Calculate by subtraction**:
![Calculation Results](https://github.com/user-attachments/assets/dc5ba25d-9fa1-436e-8184-0318d98d9786)
![Final Results](https://github.com/user-attachments/assets/ffe30dc5-231f-4590-a31e-13a0050d934b)

### TCP Connection Process

#### 1. Connection Establishment (3-Way Handshake)
1. **SYN**: Client sends SYN with sequence number
2. **SYN-ACK**: Server responds with SYN-ACK and acknowledgment number  
3. **ACK**: Client sends final ACK to establish connection

#### 2. Data Transmission
- **Segmentation**: Data broken into smaller segments
- **Sequence Numbers**: Each segment gets a sequence number for proper ordering
- **Acknowledgments**: Receiver sends ACK for each segment
- **Flow Control**: "Sliding window" prevents overwhelming the receiver
- **Error Checking**: Checksums verify data integrity

**Example**:
- Connection established with ISN 1000
- Segment 1: "Hello" (5 bytes) - Sequence: 1000-1004
- Segment 2: "World" (5 bytes) - Sequence: 1005-1009

#### 3. Connection Termination (4-Way Handshake)
1. **FIN**: One side sends FIN (finish) signal
2. **ACK**: Other side acknowledges the FIN
3. **FIN**: Second side sends its own FIN
4. **ACK**: Original sender acknowledges, connection closed

### Communication Types

#### Data Distribution:
- **Unicast**: One-to-one communication (email)
- **Multicast**: One-to-many specific destinations (video streaming)
- **Broadcast**: One-to-all devices in network segment

#### Communication Modes:
- **Simplex**: One-way communication (radio broadcast)
- **Half-Duplex**: Two-way, but not simultaneous (walkie-talkie)
- **Full-Duplex**: Simultaneous two-way communication (phone call)

## 📄 License

This content is provided for educational purposes as part of the École 42 curriculum. It is not authorized for duplication, modification, or use in any other context (personal, commercial, public, open source, etc.).

---

**Note**: The network architectures and addresses used in these exercises are fictitious and not connected to real configurations.