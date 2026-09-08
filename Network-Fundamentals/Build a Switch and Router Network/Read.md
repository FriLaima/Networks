# Build a Switch and Router Network – Physical Mode
## 📄Description
A small network was configured, consisting of router R1, switch S1, and two end devices PC-A and PC-B.
## 📌Objectives
✔ Configure IPv4 and IPv6 addressing <br>
✔ Configure basic router and switch settings <br> 
✔ Configure passwords and device access <br>
✔ Verify end-to-end connectivity <br>
## 🌐Network Topology
<img src="images/Topology.png" width="700">

## 📋Addressing Table
<img src="images/Add table.png" width="700">

## 🖥️PC Configuration
<h3><b>PC-A<br></b></h3>
<img src="images/PC-A.png" width="700">

<h3><b>PC-B<br></b></h3>
<img src="images/PC-B.png" width="700">

## ⚙️Router and switch configuration
<h3><b>Router R1<br></b></h3>
<img src="images/Conf R1.png" width="370">

<h3><b>Switch S1<br></b></h3>
<img src="images/Conf S1.png" width="500">

## 🔍Verification
After configuration, connectivity and device settings were verified using `show` commands. <br>
<h3><b>Router R1<br></b></h3>

<img src="images/Sh IP Route R1.png" width="500">

The `show ip route` command displays the IPv4 routing table and the connected networks. <br>
The `show ipv6 route` command displays the IPv6 routing table and the connected networks. <br>

<img src="images/Sh IP Interf R1.png" width="500"> <br>

The `show ip interface brief` command displays the IPv4 addresses and current status of the router interfaces (both interfaces are operational). <br>

<h3><b>Switch S1<br></b></h3>

<img src="images/Sh IP Interf S1.png" width="500"> <br>

The `show ip interface brief` command displays the status of the switch management interface - `Vlan 1` is active.

## 🧪Testing
The tests were performed using the `ping` command from PC-A to PC-B and from switch S1 to PC-B.<br>

<h3><b>PC-A → PC-B<br></b></h3>

<img src="images/Ping to PC-B.png" width="500"> <br>

<h3><b>S1 → PC-B<br></b></h3>

<img src="images/Ping From S1 To PC-B.png" width="500"> <br>

All ping packets were successfully sent.

## 🛠️Troubleshooting 
The initial ping from PC-A to PC-B was unsuccessful because the router interfaces had not yet been configured, so Layer 3 traffic could not be routed between the subnets.

## 📚What I Learned
<b>During this lab I practiced:</b><br>
➜ Configuring router interfaces and a switch management interface<br>
➜ Configuring IPv4 and IPv6 addresses<br>
➜ Enabling IPv6 routing<br>
➜ Checking routing tables<br>
➜ Checking interface status<br>
➜ Testing end-to-end connectivity with ping<br>
➜ Troubleshooting basic network connectivity problems<br>
