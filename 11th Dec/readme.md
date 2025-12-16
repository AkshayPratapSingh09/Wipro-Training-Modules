# 1. Computer Architecture

Computer architecture is the "master blueprint" that defines how hardware and software interact to perform tasks. Most modern computers follow the Von Neumann Architecture, which organizes the system into three main pillars: the Central Processing Unit (CPU), the Memory (RAM/Cache), and Input/Output devices.

**System Design:** The physical structure, including the CPU, memory controllers, and data paths.

**Instruction Set Architecture (ISA):** The set of commands the CPU understands to perform operations like adding numbers or moving data.

---

# 2. The CPU and Cores

The Central Processing Unit (CPU) is the "brain" that executes instructions, performs calculations, and manages data flow.

**The Control Unit (CU):** Acting as the "manager," the CU fetches instructions from memory, decodes them to understand what needs to be done, and directs the flow of data between other components.

**The Arithmetic Logic Unit (ALU):** This is the system's "calculator". It performs all mathematical (addition, subtraction) and logical (AND, OR, NOT) operations.

**Cores:** Modern CPUs are "multi-core," meaning they have multiple independent processing units on a single chip, allowing the computer to handle different tasks simultaneously.

**Registers:** These are the smallest, fastest storage spots located directly inside the CPU. They hold the specific data the CPU is working on right this second.

**What is a Core?** A core is an individual processing unit within the CPU.

**Single-Core:** Imagine a grocery store with one checkout lane. No matter how fast the cashier is, they can only help one person at a time.

**Multi-Core:** This is like opening four, eight, or sixteen checkout lanes. The computer can now handle different tasks—like rendering a video while you browse the web—simultaneously without slowing down.

---

# 3. RAM (Random Access Memory)

If the CPU is the brain, RAM is the short-term memory. It’s the "workspace" where the computer keeps everything it is currently using.

**Volatile Memory:** RAM requires power to hold data. If you turn off the computer without saving your work to the hard drive, the data in the RAM vanishes.

**Why it matters:** When you open an app, the computer pulls it from the slow permanent storage (SSD/Hard Drive) and puts it into the fast RAM so the CPU can access it instantly. The more RAM you have, the larger your "desk" is, allowing you to keep more apps open at once.

---

# 4. Cache

Even though RAM is fast, the CPU is much faster. If the CPU had to go to the RAM for every single piece of data, it would spend most of its time waiting. Cache is a tiny amount of ultra-fast memory located directly on the CPU chip.

## The Hierarchy of Cache:

**L1 Cache:** The smallest and fastest. It sits right inside the core.

**L2 Cache:** Slightly larger and a bit slower than L1.

**L3 Cache:** The largest of the three, usually shared between all cores on the CPU.


# Network Types Classified on Different Bases

## 1. Classification Based on Geographic Area / Coverage

![Network Diagram](https://www.vedantu.com/seo/content-images/4b229310-8572-4ab5-bb75-739644250bec.png)


### PAN (Personal Area Network)
- Covers 1–10 meters.
- Used for connecting personal devices such as smartphones, laptops, and Bluetooth peripherals.

### LAN (Local Area Network)
- Covers a room, building, or campus.
- Common in homes, offices, and schools.

### CAN (Campus Area Network)
- Connects multiple LANs within a campus (universities, enterprise sites).

### MAN (Metropolitan Area Network)
- Spans a city or large campus.
- Used by ISPs and cable networks.

### WAN (Wide Area Network)
- Covers countries or continents.
- The Internet is the largest WAN.

---

## 2. Classification Based on Ownership / Management Model

![Network Diagram](https://media.geeksforgeeks.org/wp-content/uploads/20250728191149568603/3-.webp)
### Private Network
- Owned and managed by a single organization.
- Used for internal corporate communications.

### Public Network
- Available for public use.
- Examples: ISP networks, public Wi-Fi.

### Hybrid Network
- Mix of public and private components.
- Example: VPN over public Internet for corporate access.

---

## 3. Classification Based on Topology (Network Layout)
![Network Diagram](https://media.licdn.com/dms/image/v2/D5612AQFP7npXdC-q6w/article-cover_image-shrink_720_1280/article-cover_image-shrink_720_1280/0/1691158913489?e=2147483647&v=beta&t=yXtYmLR6NG9ZQ9vWXM1lscz5o-EU4Vadrc4zs7fZRX4)

### Bus Topology
- Single shared communication cable.
- Simple but failure-prone.

### Star Topology
- All nodes connect to a central hub/switch.
- Easy to manage, but the central device is a single point of failure.

### Ring Topology
- Nodes connected in a circular manner.
- Predictable performance; break in the ring disrupts communication.

### Mesh Topology
- Each node connects to many others.
- Highly reliable but costly and complex.

### Tree Topology
- Hierarchical combination of star topologies.
- Scalable and structured.

### Hybrid Topology
- Combination of two or more topologies.
- Flexible and customizable.

---

## 4. Classification Based on Transmission Technology
![Network Diagram](https://cdn.shopify.com/s/files/1/0106/6339/5391/files/1024x576-1_512a6eaa-f938-4eab-83ba-bbecb06c3d8f_1024x1024.jpg?v=1734597835)

### Broadcast Networks
- One shared communication channel for all nodes.
- Messages sent by one device are received by all.

### Point-to-Point Networks
- Dedicated communication links between node pairs.
- Provides better privacy and performance.

---

## 5. Classification Based on Networking Roles / Architecture
![Network Diagram](https://www.networkstraining.com/wp-content/uploads/2021/06/Client-Server-p2p.png)

### Client–Server Architecture
- Servers provide centralized services; clients request and use them.
- Common in business networks.

### Peer-to-Peer (P2P)
- All nodes share equal responsibility and act as both clients and servers.
- Used in file-sharing systems.

### Distributed Networks
- Services distributed across multiple interconnected computers.
- Improves reliability and scalability.

### Cloud Networks
- Virtualized infrastructure accessed on demand.
- Managed by cloud providers such as AWS, Azure, and Google Cloud.

---

## 6. Classification Based on Switching Techniques
![Network Diagram](https://imgv2-2-f.scribdassets.com/img/document/100878824/original/f6a49a043e/1?v=1)

### Circuit Switching
- A dedicated communication path established for the entire session.
- Used in traditional telephone networks.

### Packet Switching
- Data divided into packets sent independently through the best path available.
- Basis of the Internet.

### Message Switching
- Entire messages are sent store-and-forward from node to node.
- No need for a dedicated path, but high delay for long messages.



# IPv4 vs IPv6, Subnetting, and Network Address Translation (NAT)

---

# 1. IPv4 vs IPv6

## IPv4 (Internet Protocol Version 4)
- Uses a **32-bit** addressing system.
- Provides about **4.3 billion unique addresses**.
- Address format example: **192.168.1.1**
- Written in **decimal**, separated by dots.
- Supports **manual configuration**, **DHCP**, and **NAT** widely.
- Header is **less complex** with fewer fields.
- Increasing scarcity of addresses led to the creation of IPv6.

## IPv6 (Internet Protocol Version 6)
- Uses a **128-bit** addressing system.
- Provides **3.4 × 10³⁸ addresses**, practically unlimited.
- Address format example: **2001:0db8:85a3:0000:0000:8a2e:0370:7334**
- Written in **hexadecimal**, separated by colons.
- Supports **auto-configuration (SLAAC)**.
- Designed for **security**, **efficiency**, and **scalability**.
- Eliminates the need for NAT due to abundant addresses.

## Key Differences (Summary Table)

| Feature | IPv4 | IPv6 |
|--------|------|------|
| Address Length | 32-bit | 128-bit |
| Number of Addresses | ~4.3 billion | Virtually unlimited |
| Format | Decimal | Hexadecimal |
| Separator | Dots (.) | Colons (:) |
| Security | Optional IPSec | Built-in IPSec |
| Configuration | DHCP/Manual | Auto (SLAAC) |
| NAT Requirement | Yes, due to shortage | No |

---

# 2. Subnetting

Subnetting is the process of **dividing a large network into smaller, manageable subnetworks**.  
It improves performance, security, and efficient IP address usage.

## Why Subnet?
- Reduces network congestion.
- Enhances security by isolating segments.
- Better IP address management.
- Helps create structured network designs.

## How Subnetting Works
A subnet mask determines which part of an IP address is:
- **Network portion**
- **Host portion**

Example:
- IP Address: **192.168.1.50**
- Subnet Mask: **255.255.255.0**
  - First three octets identify the network.
  - Last octet identifies hosts.

## CIDR Notation (Classless Inter-Domain Routing)
Instead of the full mask, we write:
- **192.168.1.0/24**

Here, "/24" means:
- 24 bits are for the network.
- Remaining bits are for host addresses.

---

# 3. Network Address Translation (NAT)

Network Address Translation (NAT) is a method that **maps private IP addresses to a public IP address** so devices inside a local network can access the internet.

## Why NAT is Needed
- IPv4 addresses are limited, and private networks reuse the same internal IP ranges.
- NAT allows multiple devices to share a **single public IP**.
- Provides a layer of security by hiding internal IPs.

## Types of NAT
### 1. Static NAT
- One private IP is mapped to one public IP.
- Used for servers that must be accessible externally.

### 2. Dynamic NAT
- Private IPs map to a pool of public IPs.
- Mapping changes dynamically.

### 3. PAT (Port Address Translation) or NAT Overloading
- Most common form.
- Many devices share one public IP address.
- Differentiates requests using port numbers.

Example:
- Internal: 192.168.1.10:1050  
- External: PublicIP:48562  

## Benefits of NAT
- Conserves public IP addresses.
- Adds a security layer.
- Enables large private networks to operate efficiently.

---
