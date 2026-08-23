# Build a Switch and Router Network – Physical Mode
## 📄Description
A small network was configured, consisting of router R1, switch S1, and two end devices PC-A and PC-B.
## 📌Objectives
✔ Configure IPv4 and IPv6 addressing <br>
✔ Configure basic router and switch settings <br> 
✔ Configure passwords and device access <br>
✔ Verify end-to-end connectivity <br>
## 🌐Network Topology
<img width="644" height="92" alt="image" src="https://github.com/user-attachments/assets/7ece32a0-3244-4902-8e2b-578932a016cb" />

## 📋Addressing Table
<img width="861" height="421" alt="image" src="https://github.com/user-attachments/assets/606502b1-950c-4f5a-a121-ad1f43bb113c" />

## 🖥️PC Configuration
<h3><b>PC-A<br></b></h3>
<img width="785" height="545" alt="image" src="https://github.com/user-attachments/assets/0b84f6d3-7320-44f9-8524-38e3ef05ab9a" />

<h3><b>PC-B<br></b></h3>
<img width="794" height="545" alt="image" src="https://github.com/user-attachments/assets/c3257617-9fab-43cd-9536-29ef394c5b6f" />

## ⚙️Router and switch configuration
<h3><b>Router R1<br></b></h3>
<img width="443" height="532" alt="image" src="https://github.com/user-attachments/assets/47ea2db2-4bae-4988-8d8c-868db92f2608" />

<h3><b>Switch S1<br></b></h3>
<img width="600" height="181" alt="image" src="https://github.com/user-attachments/assets/6a9325ad-9836-4971-b06b-959f101a1038" />

## 🔍Verification
After configuration, connectivity and device settings were verified using `show` commands. <br>
<h3><b>Router R1<br></b></h3>

<img width="641" height="556" alt="image" src="https://github.com/user-attachments/assets/1f88c2f5-f3a4-4534-8682-1000a355ba93" /> <br>

The `show ip route` command displays the IPv4 routing table and the connected networks. <br>
The `show ipv6 route` command displays the IPv6 routing table and the connected networks. <br>

<img width="646" height="136" alt="image" src="https://github.com/user-attachments/assets/f50bedd5-d2d4-4bb6-98ed-48acfda9f48d" /> <br>

The `show ip interface brief` command displays the IPv4 addresses and current status of the router interfaces (both interfaces are operational). <br>

<h3><b>Switch S1<br></b></h3>

<img width="648" height="437" alt="image" src="https://github.com/user-attachments/assets/cb631d15-12d8-4a90-8b7d-fcc859eaab74" /> <br>

The `show ip interface brief` command displays the status of the switch management interface - `Vlan 1` is active.

## 🧪Testing
The tests were performed using the `ping` command from PC-A to PC-B and from switch S1 to PC-B.<br>

<h3><b>PC-A → PC-B<br></b></h3>

<img width="453" height="198" alt="image" src="https://github.com/user-attachments/assets/2ddaf952-88aa-4fb4-8637-4517a39aa731" /><br>

<h3><b>S1 → PC-B<br></b></h3>

<img width="555" height="100" alt="image" src="https://github.com/user-attachments/assets/61e7334f-0e30-4b79-9994-d42b386d2aac" /> <br>

All ping packets were successfully sent.

## 🛠️Testing
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
