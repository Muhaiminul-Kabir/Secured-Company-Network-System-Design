# Secured-Company-Network-System-Design
## Case Study and Requirements:

The main task is to design and implement a network for a trading floor support centre that employs 600 staff. The company has recently expanded and needs to move to a new building with no network infrastructure. The new building consists of three floors, each accommodating two departments.

## Building Layout:

**First Floor:**
- Sales and Marketing Department - 120 users
- Human Resource and Logistics Department - 120 users

**Second Floor:**
- Finance and Accounts Department - 120 users
- Administrator and Public Relations Department - 120 users

**Third Floor:**
- ICT Department - 120 users
- Server Room - 12 devices

## Objectives

The objective is to design and implement a network for the building, ensuring it meets business needs and is future-proof. Cisco Packet Tracer was used to create the design and follow a hierarchical model providing redundancy at every layer.

## Network Design Requirements

### Hierarchical Model:
- Implemented two routers and two multilayer switches for redundancy.
- Connected to at least two ISPs for redundancy, with each router connected to both ISPs.

### Wireless Network:
- Ensured each department has a wireless network.

### VLAN and Subnetting:
- Assigned each department to a different VLAN and subnet.
- Used subnetting of the base network of 172.16.1.0 to allocate the correct number of IP addresses to each department.

### IP Addressing:
- Used static public IP addresses: 195.136.17.0/30, 195.136.17.4/30, 195.136.17.8/30, and 195.136.17.12/30 for ISP connections.
- Assigned static IPs to devices in the server room.
- Configured DHCP servers in the server room to provide dynamic IPs to all other devices.

### Device Configuration:
- Set hostnames, console passwords, enable passwords, and banner messages.
- Disabled IP domain lookup.
- Configured inter-VLAN routing on multilayer switches.
- Assigned IP addresses to multilayer switches.
- Set up SSH for remote login on routers and layer three switches.
- Configured port security for the Finance and Accounts department using the sticky method and shutdown violation mode.
- Set up PAT using the outbound router interface IPv4 address and necessary ACL rules.

### Routing and Security:
- Used OSPF as the routing protocol.
- Configured standard and extended ACLs.

### Testing:
- Tested all configurations to ensure everything is working as expected and ensure smooth communication.

## Technologies Implemented
- Created a network topology using Cisco Packet Tracer.
- Implemented a hierarchical network design.
- Connected networking devices with the correct cabling.
- Configured basic device settings.
- Created VLANs and assigned port VLAN numbers.
- Performed subnetting and IP addressing.
- Configured inter-VLAN routing on multilayer switches (Switch Virtual Interface).
- Set up a dedicated DHCP server device for dynamic IP allocation.
- Configured SSH for secure remote access.
- Set up OSPF as the routing protocol.
- Implemented NAT Overload (PAT).
