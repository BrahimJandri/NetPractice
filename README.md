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
