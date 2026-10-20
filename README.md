VLAN and Inter-VLAN Routing Using Cisco Packet Tracer

📌 Project Overview

This project demonstrates the configuration and implementation of Virtual Local Area Networks (VLANs) and Inter-VLAN Routing using Cisco Packet Tracer.

The network is divided into three departments: HR, IT, and Finance. Each department is assigned a separate VLAN to organize network traffic and improve network management. Two switches are connected using a trunk link, and a router enables communication between different VLANs.

🎯 Objectives

- Create and configure VLANs for different departments.
- Assign switch access ports to the appropriate VLANs.
- Configure trunk links between switches.
- Implement Inter-VLAN Routing using Router-on-a-Stick.
- Configure IP addresses and default gateways.
- Test connectivity using the `ping` command.

🛠️ Technologies Used

- Cisco Packet Tracer
- Cisco IOS CLI
- VLAN Configuration
- IEEE 802.1Q Trunking
- Router-on-a-Stick
- IPv4 Addressing

🏗️ Network Design

The network consists of:
- 1 Router (R1)
- 2 Switches (Switch 1 and Switch 2)
- PCs representing three departments
- Trunk connection between the switches
- Router subinterfaces for Inter-VLAN Routing

🌐 VLAN and IP Addressing Table

| VLAN ID | Department | Network Address | Default Gateway |
|---|---|---|---|
| 10 | HR | 192.168.10.0/24 | 192.168.10.1 |
| 20 | IT | 192.168.20.0/24 | 192.168.20.1 |
| 30 | Finance | 192.168.30.0/24 | 192.168.30.1 |

⚙️ Configuration Summary

1. VLAN Configuration

Three VLANs were created on both switches:
- VLAN 10: HR
- VLAN 20: IT
- VLAN 30: Finance

2. Access Port Configuration

The switch ports connected to end devices were configured as access ports and assigned to their respective VLANs.

3. Trunk Configuration

A trunk link was configured between Switch 1 and Switch 2 using IEEE 802.1Q encapsulation to carry traffic for multiple VLANs.

4. Inter-VLAN Routing

Router subinterfaces were configured on R1:

- GigabitEthernet0/0.10: 192.168.10.1
- GigabitEthernet0/0.20: 192.168.20.1
- GigabitEthernet0/0.30: 192.168.30.1

Each subinterface acts as the default gateway for its respective VLAN.

🧪 Testing and Results

Connectivity was verified using the `ping` command.

The following tests were successful:

- PCs communicating within the same VLAN across both switches.
- PCs reaching their respective default gateways.
- Communication between devices in different VLANs.
- Inter-VLAN routing between HR, IT, and Finance.

The router interfaces and VLAN trunk were also verified using Cisco IOS commands.

📸 Screenshots

Project screenshots can be found in the `screenshots/` folder, including:

- Complete network topology
- VLAN configuration
- Trunk configuration
- Router interface configuration
- Successful ping tests

📚 Key Learning Outcomes

- Understanding VLAN segmentation and its benefits.
- Configuring access and trunk ports.
- Understanding 802.1Q trunking.
- Implementing Router-on-a-Stick.
- Configuring IPv4 addresses and default gateways.
- Troubleshooting network connectivity using CLI commands.

👨‍💻 Author

Vedang Kolte

TYBCA Student | Aspiring AI and Full Stack Developer

📄 License

This project is available for educational and learning purposes.
