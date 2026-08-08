# Cisco VLAN & Inter-VLAN Routing

A network configuration project built in **Cisco Packet Tracer** demonstrating VLAN segmentation, trunking, DHCP, and inter-VLAN routing using the Router-on-a-Stick method.

## Project Overview

The network is divided into three VLANs:

* **VLAN 10 – IT**
* **VLAN 20 – HR**
* **VLAN 30 – Management**

A Cisco switch is connected to a Cisco router through a trunk link. The router uses subinterfaces to provide gateway addresses and enable communication between the different VLANs.

## Technologies Used

* Cisco Packet Tracer
* VLANs
* 802.1Q Trunking
* Router-on-a-Stick
* DHCP
* Inter-VLAN Routing
* IPv4
* Cisco IOS CLI

## Network Configuration

| VLAN | Department | Network         | Gateway      |
| ---- | ---------- | --------------- | ------------ |
| 10   | IT         | 192.168.10.0/24 | 192.168.10.1 |
| 20   | HR         | 192.168.20.0/24 | 192.168.20.1 |
| 30   | Management | 192.168.30.0/24 | 192.168.30.1 |

## Main Configuration

The switch uses access ports for the end devices and a trunk connection toward the router.

The router uses the following subinterfaces:

* `G0/0.10` → `192.168.10.1`
* `G0/0.20` → `192.168.20.1`
* `G0/0.30` → `192.168.30.1`

DHCP pools were also configured on the router for the three networks.

## Testing

Connectivity was tested using ICMP ping.

The client successfully reached:

* `192.168.10.1`
* `192.168.20.1`
* `192.168.30.1`

This confirms that the VLANs, trunk connection, router subinterfaces, and inter-VLAN routing are working correctly.

## Files

* `cisco-vlan-router-on-a-stick.pkt` – Cisco Packet Tracer project file
* Screenshots – Configuration and connectivity tests

## What I Learned

This project helped me practice configuring VLANs, assigning switch ports, creating trunk links, configuring router subinterfaces, setting up DHCP, and troubleshooting connectivity problems using Cisco IOS commands.
