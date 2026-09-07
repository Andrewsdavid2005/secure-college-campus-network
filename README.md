# 🎓 Secure College Campus Network

A medium-level enterprise campus network designed and simulated using **Cisco Packet Tracer**.

The project demonstrates how VLAN segmentation, inter-VLAN routing, DHCP, OSPF and network security mechanisms can be combined to build a secure and scalable college network.

---

## 📌 Project Overview

A college has multiple departments sharing the same network.

The existing flat network creates problems such as:

- Excessive broadcast traffic
- Poor network segmentation
- Unauthorized access
- Difficult network management
- Limited scalability

To solve these problems, a segmented and secure campus network was designed using Cisco networking technologies.

---

## 🎯 Objectives

- Separate departments using VLANs
- Provide communication between VLANs
- Automatically assign IP addresses using DHCP
- Establish WAN connectivity
- Configure dynamic routing using OSPF
- Restrict unauthorized traffic using ACLs
- Secure device management using SSH
- Protect switch ports using Port Security
- Provide an internal web server
- Test and verify network connectivity and security

---

## 🏢 Network Departments

| VLAN | Department | Network | Gateway |
|------|------------|---------|---------|
| 10 | Administration | 192.168.10.0/24 | 192.168.10.1 |
| 20 | Computer Science | 192.168.20.0/24 | 192.168.20.1 |
| 30 | Electronics | 192.168.30.0/24 | 192.168.30.1 |
| 40 | Guest | 192.168.40.0/24 | 192.168.40.1 |

---

## 🖥️ Network Devices

### Routers
- Cisco 2911 × 2

### Switches
- Cisco 3560 Layer-3 Switch × 1
- Cisco 2960 Access Switches × 3

### End Devices
- Administration PCs × 2
- Computer Science PCs × 2
- Electronics PCs × 2
- Guest PCs × 2
- Internal Server × 1

---

## 🛠️ Technologies Used

- Cisco Packet Tracer
- VLAN
- VLAN Trunking
- IPv4 Subnetting
- Inter-VLAN Routing
- Layer-3 Switching
- DHCP
- OSPF
- Extended ACL
- SSH
- Port Security
- HTTP Server
- WAN Connectivity

---

## 🌐 Network Architecture

```text
                         CAMPUS-R1
                         /       \
                        /         \
                  CAMPUS-L3      CAMPUS-R2
                 /    |    \
                /     |     \
         ADMIN-SW   CS-SW   ECE-SW
          / | \      / \      / \
         PC PC G    PC PC    PC PC
