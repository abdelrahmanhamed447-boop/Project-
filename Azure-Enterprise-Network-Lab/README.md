# Azure Enterprise Network Lab

## 📌 Overview

Hands-on Azure enterprise networking lab covering Virtual Network and subnet design, Network Security Groups, Windows Server Virtual Machines, IIS Web Servers, Azure Load Balancer, health probes, load balancing rules, Public IP, and Azure VPN Gateway configuration and connectivity.

---

## 📑 Table of Contents

- [Lab Objectives](#-lab-objectives)
- [Lab Environment](#-lab-environment)
- [Technologies & Services](#-technologies--services)
- [Lab Workflow](#-lab-workflow)
  - [1. Virtual Network & Subnets](#1-virtual-network--subnets)
  - [2. Network Security Group](#2-network-security-group)
  - [3. Public IP Configuration](#3-public-ip-configuration)
  - [4. Windows Server Virtual Machines](#4-windows-server-virtual-machines)
  - [5. IIS Web Servers](#5-iis-web-servers)
  - [6. Azure Load Balancer](#6-azure-load-balancer)
  - [7. Load Balancer Health Probe](#7-load-balancer-health-probe)
  - [8. Load Balancing Rule](#8-load-balancing-rule)
  - [9. Azure VPN Gateway](#9-azure-vpn-gateway)
  - [10. VPN Connectivity Validation](#10-vpn-connectivity-validation)
- [Validation & Testing](#-validation--testing)
- [Skills Demonstrated](#-skills-demonstrated)
- [Evidence & Documentation](#-evidence--documentation)
- [Project Structure](#-project-structure)
- [Project Summary](#-project-summary)

---

## 🎯 Lab Objectives

- Design and deploy an Azure Virtual Network.
- Configure multiple subnets.
- Configure Network Security Groups.
- Deploy Windows Server Virtual Machines.
- Configure IIS Web Servers.
- Configure Public IP addressing.
- Deploy and configure Azure Load Balancer.
- Configure backend pools and health probes.
- Configure load-balancing rules.
- Deploy Azure VPN Gateway.
- Establish and validate Point-to-Site VPN connectivity.

---

## 🖥️ Lab Environment

The lab environment included:

- Microsoft Azure
- Azure Resource Group
- Azure Virtual Network
- Multiple Subnets
- Network Security Groups
- Public IP
- Windows Server Virtual Machines
- IIS Web Server
- Azure Load Balancer
- Azure VPN Gateway
- Point-to-Site VPN

---

## 🛠️ Technologies & Services

- Microsoft Azure
- Azure Virtual Network (VNet)
- Subnets
- Network Security Groups (NSG)
- Azure Virtual Machines
- Windows Server
- IIS
- Azure Load Balancer
- Backend Pools
- Health Probes
- Load Balancing Rules
- Public IP
- Azure VPN Gateway
- Point-to-Site (P2S) VPN

---

# 🔄 Lab Workflow

## 1. Virtual Network & Subnets

Designed and deployed the Azure Virtual Network and configured the required subnets for the lab environment.

Activities included:

- Resource Group configuration
- Virtual Network deployment
- Subnet creation
- Network addressing configuration

---

## 2. Network Security Group

Configured Network Security Groups to control network traffic to and from Azure resources.

Activities included:

- NSG creation
- Security rule configuration
- Network traffic control
- NSG association with network resources

---

## 3. Public IP Configuration

Configured Public IP addressing for Azure resources requiring external connectivity.

Activities included:

- Public IP deployment
- IP configuration
- Public connectivity validation

---

## 4. Windows Server Virtual Machines

Deployed and configured Windows Server Virtual Machines within the Azure network environment.

Activities included:

- Virtual Machine deployment
- Network interface configuration
- Private IP addressing
- Public IP association where required
- Windows Server configuration

---

## 5. IIS Web Servers

Configured IIS Web Server on the Windows Server Virtual Machines.

The environment included web servers used to demonstrate load balancing and web traffic distribution.

Activities included:

- IIS installation
- Web Server configuration
- Web service validation
- Connectivity testing

---

## 6. Azure Load Balancer

Configured Azure Load Balancer to distribute incoming web traffic across backend virtual machines.

Activities included:

- Frontend IP configuration
- Backend pool configuration
- Virtual Machine association
- Load Balancer configuration

---

## 7. Load Balancer Health Probe

Configured an HTTP health probe to monitor the availability of backend IIS web servers.

Activities included:

- HTTP health probe configuration
- Backend health monitoring
- Service availability validation

---

## 8. Load Balancing Rule

Configured a load-balancing rule to distribute incoming traffic across the backend web servers.

Activities included:

- Frontend IP configuration
- Backend pool association
- Health probe association
- Load-balancing rule configuration
- Web traffic distribution testing

---

## 9. Azure VPN Gateway

Deployed and configured Azure VPN Gateway to provide secure remote connectivity to the Azure virtual network.

Activities included:

- VPN Gateway deployment
- Gateway configuration
- Virtual Network Gateway configuration
- VPN connectivity configuration

---

## 10. VPN Connectivity Validation

Established and validated Point-to-Site VPN connectivity to the Azure environment.

Activities included:

- Point-to-Site VPN configuration
- VPN client configuration
- VPN connection establishment
- Connectivity validation

---

# 🧪 Validation & Testing

The lab configuration was validated through practical testing of:

- Virtual Network connectivity
- Subnet communication
- NSG behavior
- Windows Server accessibility
- IIS web server availability
- Azure Load Balancer functionality
- Backend health probes
- Load-balancing rules
- VPN Gateway connectivity
- Point-to-Site VPN connection

---

# 🧠 Skills Demonstrated

### Azure Networking

- Virtual Network Design
- Subnetting
- Network Security Groups
- Public IP Configuration
- Azure Load Balancer
- Azure VPN Gateway
- Point-to-Site VPN

### Server & Web Services

- Windows Server
- IIS Web Server
- Virtual Machine Deployment
- Network Interface Configuration

### Load Balancing

- Backend Pools
- Health Probes
- Load Balancing Rules
- Traffic Distribution
- Backend Availability Monitoring

### Network Administration

- Network Design
- Network Connectivity
- Troubleshooting
- Infrastructure Validation

---

# 📸 Evidence & Documentation

The project documentation contains implementation evidence covering:

- Azure Virtual Network
- Subnets
- Network Security Groups
- Public IP
- Windows Server Virtual Machines
- IIS Web Servers
- Azure Load Balancer
- Backend Pools
- Health Probes
- Load Balancing Rules
- Azure VPN Gateway
- Point-to-Site VPN Connectivity

---

# 📁 Project Structure

```text
Azure-Enterprise-Network-Lab/
│
├── README.md
│
└── Azure_Enterprise_Lab_GitHub_Ordered.pdf
