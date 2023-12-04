
# Campus-LAN-Network


Description:
University Campus Network Topology have been designed and implemented in Packet Tracer. All network devices used in this project are Cisco Devices. University has two campuses with many buildings located in Houston and Austin areas. I have created both logical and physical network layouts for this university.	In Houston Campus there are several buildings such as:
-Administration Building: Administrative staff in the departments of management, HR and finance. The admin staff PCs are distributed in the building offices and it is expected that they will share some networking equipment.The Faculty of Business is also situated in this building. Total of 4 Access Switches, 1 Multilayer Switch and 1 Router are located in this building.
- Academic Building: College of Engineering and College of Art. Total of 2 Access Switches are located in this building.
- Library & IT Room: Students’ labs and IT department. Total of 2 Access Switches, Web Server, DNS Server, and FTP Servers are located in the IT room.
In Austin Campus there is only 1 building with 2 floors. 2 Access Switches, 1 Multilayer 3 and 1 Router have been deployed.
Email server of the University hosted Externally on the Cloud 


Technical Report of the Network Design:

Access Switches:
Switch ports have been configured in proper VLANs meeting network requirements. Port Security have been enabled on all the switch interfaces to add extra layer of security to the network. In addition, all unused ports have been shut down to prevent unauthorized access and cyber attacks. Portfast feauture is on access ports to eliminate the delay in the STP (Spanning Tree Protocol) blocking state. It helps in reducing the time it takes for devices to become operational after being connected to the network. BPDU Guard Security feature have been enabled to protect the network against misconfigurations or potential loops caused by unauthorized switches being connected to ports configured with PortFast. The 'enable secret' password is set to ensure that only authorized personnel can access the device's privileged mode. This prevents unauthorized configuration changes or access to critical settings that can impact the network. The uplink interfaces of the Access Switches have been configured as trunk ports and connected to the Multilayer Switch via high speed fiber optic cable. Total of 10 Vlans have been created for the University for better security and easy manageability.

Multilayer Switch:

The network is 2-tier network consisting of Access and Core Switches. There are total of 2 Multilayer Switches have been deployed, 1 for each site and connected to the Access Switches and Routers. Inter-Vlan Routing have been enabled on the switch SVIs to route traffic between different VLANs on the network. Also, Layer 3 switches serve as DHCP Servers for end devices such as PCs & Printers to obtain IPv4 address dynamically. DHCP pools for all VLANs have been created starting from
  Vlan 10 - 192.168.1.0/24
  Vlan 20 - 192.168.2.0/24
  Vlan 30 - 192.168.3.0/24
  ,etc..


Routers:

Houston and Austin Campuses are connected via Wide Area Network (WAN) using Serial Cables and have been configured with Open Shortest Path First Routing Protocol. Each Router interface have been assigned with proper IPv4 address using /30 prefix. Total of 3 routers have been configured including Cloud Router as there's no actual Internet connection feauture in Packet Tracer.

Conclusion:

This Hiararchiel Network is fully operational, network communication between devices have been tested and verified. Feel free to download Packet Tracer File and explore the Logical and Physical Topologies of the Network. You may customize and make any relevant changes to the network as you wish. 


**Logical Topology:**

Whole Network:

<img width="1319" alt="Logical View" src="https://github.com/aakbarjon/Campus-LAN-Network/assets/99519116/793259da-9138-49f2-885f-2208704d2d6a">

Houston Campus:

<img width="1289" alt="Houston Logical" src="https://github.com/aakbarjon/Campus-LAN-Network/assets/99519116/92ffaef1-aeb3-44fa-8e72-5997e5f54f69">

Austin Campus:

<img width="490" alt="Austin Logical" src="https://github.com/aakbarjon/Campus-LAN-Network/assets/99519116/67970683-3603-4c77-b993-976b527d1c47">


**Physical Topology:**

Whole Network:

<img width="1175" alt="Physical View" src="https://github.com/aakbarjon/Campus-LAN-Network/assets/99519116/46936657-e6f7-4531-8d30-311cef175f00">


Houston Campus:

<img width="1319" alt="Houston Campus" src="https://github.com/aakbarjon/Campus-LAN-Network/assets/99519116/6abf197b-bd83-467b-8ca1-cc38fe47d710">


Austin Campus:

<img width="867" alt="Austin Campus" src="https://github.com/aakbarjon/Campus-LAN-Network/assets/99519116/20396aa6-c58a-4a8d-8d3e-64dbccd95d1d">




**Devices used in the network design.**

Cisco ISR Routers 2911:


<img width="245" alt="image" src="https://github.com/aakbarjon/Campus-LAN-Network/assets/99519116/4d607f0f-bfea-45ba-bdb9-65cf7114526e">


    
Cisco Switch 2960:

<img width="215" alt="image" src="https://github.com/aakbarjon/Campus-LAN-Network/assets/99519116/b9773b44-d610-4ea3-b487-dc7c5908fb81">


 			 
Cisco Layer 3 Switch 3550:


<img width="241" alt="image" src="https://github.com/aakbarjon/Campus-LAN-Network/assets/99519116/ee54af0b-991d-4c71-9237-a5dadd0d3aa4">


 					 
Servers:

<img width="245" alt="image" src="https://github.com/aakbarjon/Campus-LAN-Network/assets/99519116/ebbb52cd-0488-41e1-823d-105ea605d9d2">

 			 


Printers:

<img width="153" alt="image" src="https://github.com/aakbarjon/Campus-LAN-Network/assets/99519116/7312e4f8-2c53-4b0f-9a66-b82b5756d8ef">


 				 
Personal Computers:

<img width="148" alt="image" src="https://github.com/aakbarjon/Campus-LAN-Network/assets/99519116/470f3cc3-7a15-4059-9597-a6f1c70dce52">


 				 
