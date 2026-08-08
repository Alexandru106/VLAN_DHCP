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

DHCP pools were also configured on the router for the three networks.
This confirms that the VLANs, trunk connection, router subinterfaces, and inter-VLAN routing are working correctly

This project helped me practice configuring VLANs, assigning switch ports, creating trunk links, configuring router subinterfaces, setting up DHCP, and troubleshooting connectivity problems using Cisco IOS commands.
