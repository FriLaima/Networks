# Design and Implement a VLSM Addressing Scheme – Physical Mode
## 📄Description
A VLSM addressing scheme was designed for a network using the 192.168.33.128/25 address space. The network was divided into subnets of different sizes according to the number of hosts required.
The calculated IPv4 addresses and subnet masks were assigned to the router interfaces, and connectivity between the routers was tested using the ping command.
## 📌Objectives
✔ Design a VLSM addressing scheme for an IPv4 network <br>
✔ Calculate subnet addresses and subnet masks based on host requirements <br> 
✔ Configure the router interfaces according to the addressing plan <br>
✔ Test connectivity between routers using `ping` <br>
## 🌐Network Topology
<img width="598" height="128" alt="image" src="https://github.com/user-attachments/assets/baa0e34f-9d54-499b-b9a2-3ef67f00ec72" />

## 📋Addressing Tables
<h3><b>VLSM Addressing Scheme<br></b></h3>
The 192.168.33.128/25 network provides 126 usable host addresses. A total of 6 subnets were required for the topology. <br>
<br><img width="907" height="324" alt="image" src="https://github.com/user-attachments/assets/6363827c-3ed5-40d9-8db5-1c54504d5688" />

The subnets were allocated from the largest host requirement to the smallest, which allows the available address space to be used efficiently.
<h3><b>Device Addressing Table<br></b></h3>
<img width="817" height="225" alt="image" src="https://github.com/user-attachments/assets/54d6911d-43cd-4d3e-9da3-f593e5755dbd" />

## ⚙️Router BR-2 configuration
<img width="723" height="318" alt="image" src="https://github.com/user-attachments/assets/924d70d0-1d3e-4897-a77a-fb8809b4c6af" />

## 🧪Testing
Connectivity between the routers was tested using the `ping` command.
<h3><b>From BR1, ping G0/0/0 interface on BR2<br></b></h3>
<img width="583" height="98" alt="image" src="https://github.com/user-attachments/assets/fa9ce76a-71a2-46f4-891f-df7a6743dc18" />

<h3><b>From BR2, ping G0/0/0 interface on BR1<br></b></h3>
<img width="579" height="97" alt="image" src="https://github.com/user-attachments/assets/d2b3ab02-a4b6-4530-9f50-e8010f3282f1" />

<br>Successful pings confirmed connectivity between the two routers.

## 📚What I Learned
<b>During this lab I practiced:</b><br>
➜ How to design a VLSM addressing scheme <br>
➜ How to calculate subnet sizes based on host requirements <br>
➜ How to divide an IPv4 network into subnets of different sizes 
