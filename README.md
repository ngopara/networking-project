# TechNova LTD Networking Project

This project demonstrates the design and configuration of a **multi-department network** for TechNova LTD using Cisco Packet Tracer. The network connects the **IT, Sales, and HR departments**, implements IP addressing and access control, and verifies connectivity and controlled access to a server.

## Table of Contents

* Project Overview
* Network Topology
* Tools and Technologies
* Configuration Steps
* Results and Findings
* Author

## Project Overview

The goal of this project was to create and configure a functional network environment for **TechNova LTD** using Cisco Packet Tracer.

The project focused on:

* Connecting the **IT, Sales, and HR departments** through a central router.
* Configuring IP addresses for devices within each department.
* Connecting an IT server to provide network services.
* Testing connectivity between departments.
* Implementing an **Access Control List (ACL)** to control traffic between departments.
* Verifying that Sales users could access the server's **HTTP service** while selected interdepartmental traffic was restricted.

The completed topology and configuration evidence are documented in the uploaded project report. 

## Network Topology

The network was designed using a **central Cisco 2911 router** connected to three departmental networks.

* **IT Department**

  * Network: `192.168.10.0/24`
  * Router gateway: `192.168.10.1`
  * Server: `192.168.10.2`
  * Two IT PCs connected through a switch

* **Sales Department**

  * Network: `192.168.20.0/24`
  * Router gateway: `192.168.20.1`
  * Two Sales PCs connected through a switch

* **HR Department**

  * Network: `192.168.30.0/24`
  * Router gateway: `192.168.30.1`
  * Two HR PCs connected through a switch

* **Router**

  * Cisco 2911 router
  * Connects the IT, Sales, and HR networks through separate interfaces
  * Provides routing between the departmental subnets
  * Uses an **ACL** to control network traffic

The topology screenshot shows the three departmental switches connected to the router, with the IT server connected to the IT departmental switch. 

## Tools and Technologies

* **Cisco Packet Tracer**
* **Cisco 2911 Router**
* **Cisco switches**
* **PC-PT workstations**
* **Server-PT**
* **IPv4 addressing**
* **Subnetting**
* **Router interfaces**
* **ICMP/Ping testing**
* **HTTP service**
* **Access Control Lists (ACLs)**
* **Router CLI**

## Configuration Steps

1. Created the network topology in **Cisco Packet Tracer**.
2. Added a **Cisco 2911 router** to serve as the central routing device.
3. Created separate departmental networks for **IT, Sales, and HR**.
4. Connected each department's PCs to its corresponding network switch.
5. Connected the IT server to the IT departmental switch.
6. Configured the router interfaces with the appropriate departmental gateway addresses:

   * `192.168.10.1` for IT
   * `192.168.20.1` for Sales
   * `192.168.30.1` for HR
7. Configured IP addressing on PCs in each department.
8. Configured the IT server with the `192.168.10.2` address shown in the topology.
9. Tested connectivity between departmental devices using **ping**.
10. Verified successful communication from an **HR PC to an IT PC**.
11. Configured an **ACL** on the router to restrict specified traffic between the Sales and IT networks.
12. Tested connectivity from a **Sales PC to an IT PC** and confirmed that the restricted connection failed.
13. Verified that Sales users could still access the server's **HTTP service**.
14. Reviewed the resulting network behavior using Cisco Packet Tracer's simulation and testing features.

The report documents the IP configuration for PCs in the IT, Sales, and HR departments, followed by connectivity and ACL testing. 

## Results and Findings

The completed network successfully demonstrated **departmental connectivity and controlled network access**.

* The **IT, Sales, and HR networks** were successfully connected through the router.
* IP addressing was configured for devices across the departmental networks.
* A ping from an **HR PC to an IT PC was successful**, demonstrating permitted interdepartmental connectivity. 
* A ping from a **Sales PC to an IT PC failed** after the ACL was implemented, demonstrating that the ACL successfully restricted the specified traffic. 
* The **Sales department retained access to the server's HTTP service**, demonstrating that the ACL could restrict specific traffic without preventing all access to the server. 
* Overall, the project demonstrated practical application of **IP addressing, routing, connectivity testing, ACL configuration, and network access control** in Cisco Packet Tracer.

## Author

**Ngozi Opara**

* **Student ID:** `GRC-C26-08-EU-004`
* **Date:** 11 September 2026
* **GitHub:** `linkedin.com/in/rosemaryopara`
* ![Network Topology](Steep 4)
