# Networking basics #0

**Level:** Novice  
**Author:** Sylvain Kalache  
**Weight:** 1  

---

## 📖 Description
This project introduces the fundamental concepts of networking.  
It covers the **OSI model**, different types of networks (LAN, WAN, Internet), MAC and IP addresses, TCP/UDP protocols, ports, and the use of basic networking tools like `ping` and `netstat`.

At the end of this project, you should be able to explain these concepts clearly without external references.

---

## 📚 Resources
Read or watch:
- OSI model
- Different types of network
- LAN, WAN, Internet
- MAC address
- What is an IP address
- Private and public address
- IPv4 and IPv6
- Localhost
- TCP and UDP
- TCP/UDP ports list
- What is ping / ICMP
- Positional parameters

Man pages or help:
- `netstat`
- `ping`

---

## 🎯 Learning Objectives
You should be able to explain:

### OSI Model
- What it is
- Number of layers
- How it is organized

### Networks
- **LAN:** usage and typical geographical size  
- **WAN:** usage and typical geographical size  
- **Internet**

### IP Addressing
- What is an IP address
- Types (private/public)
- Localhost
- Subnet
- Why IPv6 was created

### Protocols
- TCP vs UDP  
- Main differences
- Ports (SSH: 22, HTTP: 80, HTTPS: 443)  
- Tool/protocol to check connectivity (ping/ICMP)

---

## 📝 Requirements
- All Bash script files must:
  - Be interpreted on **Ubuntu 22.04**
  - End with a newline
  - Be executable
  - Pass `shellcheck` without errors
  - Start with `#!/usr/bin/env bash`
  - Have a second line comment describing the script

- A `README.md` file is mandatory at the root of the project.

- For multiple choice questions, answer files should contain only the correct option number.

---

## 🧩 Tasks

### 0. OSI model
- Understand the 7 layers of the OSI model.
- Focus on Transport (TCP/UDP) and Network (IP/ICMP) layers.

File: `0-OSI_model`

---

### 1. Types of network
- Differentiate between LAN, WAN, and Internet.

File: `1-types_of_network`

---

### 2. MAC and IP address
- MAC = unique identifier of a network interface.
- IP = address used for communication (like a postal address).

File: `2-MAC_and_IP_address`

---

### 3. UDP and TCP
- TCP: reliable, slower, ensures delivery.  
- UDP: faster, may lose data, no guarantee.  

File: `3-UDP_and_TCP`

---

### 4. TCP and UDP ports
- 65,535 ports available.
- Common ones:
  - 22 → SSH
  - 80 → HTTP
  - 443 → HTTPS
- Write a Bash script to display **listening ports** with PID and program.

File: `4-TCP_and_UDP_ports`

---

### 5. Is the host on the network
- Write a Bash script to ping an IP address (argument).
- If no argument → show usage message.
- Send 5 ping requests.

File: `5-is_the_host_on_the_network`

---

## 📂 Repository Structure
holbertonschool-network/
└── basics_0/
├── 0-OSI_model
├── 1-types_of_network
├── 2-MAC_and_IP_address
├── 3-UDP_and_TCP
├── 4-TCP_and_UDP_ports
├── 5-is_the_host_on_the_network
└── README.md

---

## ✅ Usage
Examples:

```
./4-TCP_and_UDP_ports
./5-is_the_host_on_the_network 8.8.8.8
```

---

📌 Notes

Use ping to test connectivity.

Remember the analogy:

IP address = postal address

TCP/UDP ports = doors/windows

Socket = IP + port

