**Structure of the Network:**

![image](https://github.com/Sumukh-Shadakshari/Simulation-of-Voice-Over-IP-VoIP-/assets/131502591/2e110f0e-1c95-4d01-a41a-7e1bdd90740d)

A comprehensive VoIP network has been designed to emulate a genuine business environment. Below are the specifications of the network:
All desktops have an associated telephone set.
There are 4 departments in the company:
1.	Finance: 10 IP phones, 10 PCs, 1 printer.
2.	Sales: 10 IP phones, 10 PCs, 1 printer.
3.	Human Resources: 10 IP phones, 10 PCs, 1 printer.
4.	Information and Communication technology: 10 IP phones, 10 PCs, 1 printer.

The company will be using the following IP addresses: 192.168.100.0/24 for Data, 172.16.100.0/24 for Voice, and 10.10.10.0/24 between the routers.

Routers: Each department is to have VoIP enabled router with server-side LAN attached to the ICT department router. Cisco 2811 router is used.

Switches: Each department has an access layer switch. Cisco 2960 switch is used.

Connections: Serial connections between routers, and a straight through cable between the router to switch, switch to hosts, phones to PCs have been used.

Subnets: Each department will be accessing two subnetworks, i.e, the data and voice subnets. 

DHCP Server: For voice (VoIP), the respective router has been used as the DHCP server while for Data there is a DHCP server device at the server-side site.

VLANs: Each department is a part of two VLANS. One for data and another for voice. All IP phones in the network should are in VLAN 100. For Data exchange: VLAN 10 (FINANCE), VLAN 20 (HR), VLAN 30 (SALES), VLAN 40 (ICT) and VLAN 50 (SERVERS) have been used.

Inter-VLAN Routing: Router-on-a-stick has been used to enable inter-VLAN routing on the network. 

Routing protocol: OSPF has been used as the routing protocol to advertise routes on the routers.

Telephony service: Configured VoIP on the routers and allocated dial numbers in this format for the departments, Finance (1..), HR (2..), Sales (3..), and ICT (4..), (where 1.. can be 101 to 199) and so on.

Routing for VoIP: dial-peering has been configured on the routers to allow IP phones from different routers to communicate with each other.
