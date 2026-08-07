# Amazon VPC (Virtual Private Cloud)

## What is Amazon VPC?

Amazon VPC (Virtual Private Cloud) is a logically isolated virtual network in AWS where we can launch and manage AWS resources securely.

It allows us to control:

- IP Address Range
- Subnets
- Routing
- Internet Access
- Security

---

# Why do we need VPC?

Without VPC:

- All resources would be on the same network.
- No network isolation.
- Less security.
- Difficult to control traffic.

With VPC:

- Isolated Network
- Secure Communication
- Controlled Internet Access
- Better Architecture

---

# CIDR Block

CIDR (Classless Inter-Domain Routing) defines the IP address range of a VPC.

Example:

10.0.0.0/16

Meaning:

- Network Address: 10.0.0.0
- Prefix: /16
- Remaining bits are used for host IP addresses.

---

# Public Subnet

A Public Subnet is a subnet that has a route to the Internet Gateway.

Resources inside a Public Subnet can access the Internet (if they have a Public IP).

Example:

- Web Server
- Bastion Host

---

# Private Subnet

A Private Subnet does not have a direct route to the Internet Gateway.

Resources inside a Private Subnet are not directly accessible from the Internet.

Example:

- Amazon RDS
- Internal Application Servers

---

# Route Table

A Route Table contains routing rules that decide where network traffic should go.

Example:

Destination: 10.0.0.0/16

Target: Local

Meaning:
Traffic inside the VPC stays inside the VPC.

Example:

Destination: 0.0.0.0/0

Target: Internet Gateway

Meaning:
Traffic for the Internet goes to the Internet Gateway.

---

# Local Route

Every VPC automatically contains a Local Route.

Example:

Destination:

10.0.0.0/16

Target:

Local

Purpose:

Allows communication between resources inside the same VPC.

---

# Internet Gateway (IGW)

An Internet Gateway connects a VPC to the Internet.

Functions:

- Allows inbound Internet traffic.
- Allows outbound Internet traffic.
- Required for Public Subnets.

Without an Internet Gateway, Internet communication is not possible.

---

# NAT Gateway

A NAT Gateway allows resources inside a Private Subnet to access the Internet without exposing them to inbound Internet traffic.

Example:

- Software Updates
- Package Installation

Private resources remain inaccessible directly from the Internet.

---

# Security Group

Security Group is a virtual firewall attached to an AWS resource.

Features:

- Instance Level Security
- Stateful Firewall
- Supports Allow Rules Only

Example:

SSH (22)

HTTP (80)

HTTPS (443)

---

# Network ACL (NACL)

Network ACL is a subnet-level firewall.

Features:

- Works at Subnet Level
- Stateless Firewall
- Supports Allow and Deny Rules

---

# Security Group vs NACL

| Security Group | NACL |
|----------------|------|
| Instance Level | Subnet Level |
| Stateful | Stateless |
| Allow Rules Only | Allow & Deny Rules |
| Applied to EC2 | Applied to Subnet |

---

# VPC Peering

VPC Peering allows two VPCs to communicate privately using their private IP addresses.

Use Cases:

- Communication between two VPCs
- Internal AWS networking

---

# VPC Endpoint

A VPC Endpoint allows private access from a VPC to supported AWS services without using the Internet.

Example:

EC2 → S3

without Internet Gateway.

---

# Transit Gateway

Transit Gateway is a central hub used to connect multiple VPCs and On-Premises Networks.

Instead of creating many VPC Peering connections, all VPCs connect to one Transit Gateway.

---

# Packet Flow

User

↓

Internet

↓

Internet Gateway

↓

Public Route Table

↓

Public Subnet

↓

EC2

↓

Private IP

↓

Private Subnet

↓

Amazon RDS

---

# Practical Performed

✅ Created Custom VPC

✅ Configured IPv4 CIDR

✅ Created Public Subnet

✅ Created Private Subnet

✅ Created Internet Gateway

✅ Attached Internet Gateway to VPC

✅ Configured Public Route Table

✅ Associated Public Subnet with Route Table

✅ Launched EC2 in Public Subnet

✅ Connected EC2 using SSH

---

# Real World Use Cases

- Three-Tier Architecture
- Web Applications
- Private Databases
- Secure Internal Communication
- Enterprise Cloud Networks

---

# Interview Questions

1. What is Amazon VPC?

2. What is CIDR?

3. Difference between Public and Private Subnet?

4. What is an Internet Gateway?

5. What is a Route Table?

6. Difference between Security Group and NACL?

7. What is NAT Gateway?

8. What is VPC Peering?

9. What is a VPC Endpoint?

10. What is Transit Gateway?

---

# Notes

Amazon VPC provides an isolated virtual network in AWS.

Public resources communicate through an Internet Gateway.

Private resources remain isolated and communicate internally using private IP addresses.

Security Groups secure instances, while Network ACLs secure subnets.

A secure production architecture typically places web servers in a Public Subnet and databases in a Private Subnet.
