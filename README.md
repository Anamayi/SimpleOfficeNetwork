<h1>Building a simple Office Network, using Cisco Packet Tracer</h1>

<h2>OBJECTIVES OF PROJECT</h2>

- <b>Design a network structure with multiple switches and endpoints,</b> 
- <b>create subnets, subnet masks, assign IP addresses and gateway to devices on network,</b>
- <b>configure router, switch and endpoint devices,</b> 
- <b>test connectivity between subnets using a ping.</b>


<h2>OVERVIEW</h2>

In this project, I designed a simple virtual office network using the CISCO PACKET TRACER. It provided a means of understanding, network structure, movement of data in a network, usage of Cisco Packet Tracer and built practical experience of the networking process, subnetting, assigning IP addresses and calculation of subnet masks in a network. For this project a fictional Office was used.

<h2>SCENARIO</h2>

XYZ company is a small procurement and courier business operating out of Lagos. They handle deliveries for various individuals and companies. Seeing as the company has recently expanded into 2 separate departments, the Finance/HR department and the Delivery/Customer Service department, in their office, the have requested my services to create a simple LAN network incorporating both departments.

<h3>Starting configurations</h3>

The network address will be 192.168.40.0 and we will be configuring 2 subnets, one for each department.


<h2>STEP-BY-STEP PROCESS:</h2>

<h3>Step 1 – Network Structure</h3>

The physical network topology;

- <b>End Devices: PC (4), Printer (2)</b> 
- <b>Network: Router, Switch (2)</b>

Firstly, all devices to be used by each department were added and all end point devices were linked to the appropriate switches, which were then linked to the router using suitable cabling (Gigabit Ethernet and Fast Ethernet cables).
  
<p align="center">
Network Structure: <br/>
<img src="https://i.imgur.com/BBnIn1r.png" height="80%" width="80%" alt="Office Network Structure"/>

<h3>Step 2 – Subnetting</h3>

<p align="center">
Subnet Mask Calculation: <br/>
<img src="https://i.imgur.com/LWlwk8g.png" height="80%" width="80%" alt="Subnet and IP"/>

<h3>Step 2 – Device setup and configuration</h3>

Router setup and configuration;
<p align="center">
To turn on router interfaces: <br/>
<img src="https://i.imgur.com/dqAOFJG.png" height="80%" width="80%" alt="Subnet and IP"/>
<br />
<br />
Assigning IP addresses to the interfaces: <br/>
<img src="https://i.imgur.com/kxECL6I.png" height="80%" width="80%" alt="IP adresses"/>

<h4>PC configuration</h4>

For the devices in subnet 1, I assigned the following IPs

- <b>PC0 – 192.168.40.2</b> 
- <b>PC1 – 192.168.40.3</b>
- <b>Printer0 – 192.168.40.4</b>

The default gateway was 192.168.40.1 i.e. the router interface IP, and the subnet mask was 255.255.255.128.

For the devices in subnet 2, I assigned the following IPs

- <b>PC2 – 192.168.40.130</b> 
- <b>PC3 – 192.168.40.131</b>
- <b>Printer1 – 192.168.40.132</b>

The default gateway was 192.168.40.129 i.e. the router interface IP, and the subnet mask was 255.255.255.128.

<h3>Step 4 – Testing configuration using a ping</h3>

In the end, we needed to see if both subnets could communicate with each other for a working LAN. So we used the ping command to send a ping from PC0 to PC3 on command prompt;
<p align="center">
Pinging PC3 from PC0: <br/>
<img src="https://i.imgur.com/rexIYJf.png" height="80%" width="80%" alt="Subnet and IP"/>

PC0 sent a packet to PC3 and PC3 replied to PC0 which implies that the Network connection is working.



<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
