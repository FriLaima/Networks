# Configure IPv6 Addresses on Network Devices - Physical Mode
## 📄Description
IPv6 addresses were manually configured on the router, switch, and PCs. IPv6 routing was enabled on router R1, allowing hosts to receive network information through SLAAC. The configuration was then verified using IPv6 `show` commands, `ping`, and `tracert`.

## 📌Objectives
✔ Set Up Topology and Configure Basic Router and Switch Settings <br>
✔ Configure IPv6 Addresses Manually <br> 
✔ Verify End-to-End Connectivity <br>
## 🌐Network Topology
<img src="images/Topology.jpg" width="700">

## 📋Addressing Table
<img src="images/Add table.jpg" width="700">

## 🖥️PC Configuration
<h3><b>PC-A<br></b></h3>
<img src="images/PC-A.png" width="700">
<h3><b>PC-B<br></b></h3>
<img src="images/PC-B.png" width="700">

## ⚙️Router and switch configuration
<h3><b>R1<br></b></h3>
The device’s basic settings have been configured.
<img src="images/Conf R1.png" width="500">
IPv6 global unicast addresses were assigned to both Ethernet interfaces. The same link-local address fe80::1 was manually configured on both interfaces.
<img src="images/IPv6 link-local.png" width="500">
<h3><b>S1<br></b></h3>
The device’s basic settings have been configured.
<img src="images/Conf S1.png" width="500">
The management interface VLAN 1 was configured with an IPv6 address.
<img src="images/Interf vlan1.png" width="500">

## 🔍Verification
<h3><b>R1<br></b></h3>

This command displays the IPv6 addresses and status of the router interfaces `show ipv6 interface g0/0/0`.<br>
<img src="images/verify IPv6 interf g000.png" width="500"><br>
This command verifies the IPv6 configuration of the interface, including its link-local address, global unicast address, and multicast groups.

The IPv6 configuration was verified using `show ipv6 interface brief`.<br>
<img src="images/verify R1 IPv6.png" width="500"><br>
This command displays the IPv6 addresses and status of the router interfaces.

<h3><b>S1<br></b></h3>

This command displays the IPv6 addresses and status of the VLAN 1 management interface `show ipv6 interface vlan1`.<br>
<img src="images/verify S1 vlan1.png" width="500"><br>

## 🧪Testing
Connectivity was tested using `ping` command.
<h3><b>Ping from PC-A to G0/0/1 on R1<br></b></h3>
<img src="images/ping from PC-A to g001 on R1.png" width="500">
<h3><b>Ping from PC-B to G0/0/0 on R1<br></b></h3>
<img src="images/Ping from PC-B to g000 on R1.png" width="500">
<h3><b>Ping from PC-B to PC-A<br></b></h3>
<img src="images/Ping from PC-B to Pc-A.png" width="500">
<h3><b>Tracert<br></b></h3>

From PC-A, I used the `tracert` command to verify that I have end-to-end connectivity to PC-B. <br>
<img src="images/tracert.png" width="500"><br>
All the tests were successful.
## 📚What I Learned
<b>During this lab I practiced:</b><br>
➜ How to configure IPv6 addresses manually <br>
➜ How link-local and global unicast IPv6 addresses work <br>
➜ How to enable IPv6 routing on a Cisco router <br>
➜ How SLAAC provides hosts with IPv6 addressing information <br>
➜ How to verify IPv6 configuration using Cisco IOS commands <br>
➜ How to test IPv6 connectivity using ping and tracert <br>
