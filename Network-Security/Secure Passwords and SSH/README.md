# Configure Secure Passwords and SSH
## 📄Description
In this lab, basic security settings were configured on router RTA and switch SW1. Password encryption, local user authentication, and SSH were used to protect network devices from unauthorized access. Unused switch ports were disabled, and login protection was configured to prevent repeated failed login attempts. SSH connections were tested to verify secure remote management.
## 📌Objectives
✔ Configure basic security settings on a router and a switch <br>
✔ Encrypt passwords and set password requirements <br> 
✔ Configure SSH for secure remote access <br>
✔ Disable unused switch ports <br>
✔ Configure login protection and session timeout <br>
✔ Verify SSH connectivity to network devices <br>
## 🌐Network Topology
<img src="images/Topology.png" width="250">

## 📋Addressing Table
<img src="images/ADD Table.png" width="800">

## 🖥️PC Configuration
<img src="images/IP Conf PCA.png" width="800">

## ⚙️Router and switch configuration
<h3><b>Router RTA<br></b></h3>

The router was configured with basic security settings. Password encryption was enabled, and a minimum password length was set to 10 characters. A strong enable secret was configured, and DNS lookup was disabled. A domain name and local user account were created for authentication. RSA keys were generated to enable SSH access. Login protection was configured to block login attempts after repeated failures, and the session timeout was set to 6 minutes. <br>

<img src="images/RTA Conf.png" width="700">

<h3><b>Switch SW1<br></b></h3>

The switch was configured with a management IP address, default gateway, and basic security settings. Password encryption and local user authentication were enabled. RSA keys were generated, and SSH was configured for secure remote access. Unused switch ports were disabled, and the session timeout was set to 6 minutes. <br>

<img src="images/SW1 Conf.png" width="700">
<img src="images/SW1 Conf 2.png" width="700">

## 🧪Testing
SSH connections were tested from PC-A to RTA and SW1 using the configured local username and password. <br>

<img src="images/Check SSH.png" width="700">

Successful SSH connections confirmed that secure remote access was configured correctly.

## 🛠️Troubleshooting 
During configuration, the following settings were checked: <br>
🔴 Correct IP addresses and default gateway <br>
🔴 Router and switch interfaces were enabled <br>
🔴 RSA keys were generated <br>
🔴 SSH was allowed on VTY lines <br>
🔴 Local user authentication was configured <br>
🔴 Unused switch ports were disabled <br>

## 📚What I Learned
<b>During this lab I practiced:</b><br>
➜ How to secure Cisco network devices <br>
➜ How password encryption works in Cisco IOS <br>
➜ How to configure local user authentication <br>
➜ How to generate RSA keys for SSH <br>
➜ How SSH provides secure remote access <br>
➜ How to disable unused switch ports <br>
➜ How to configure login protection and session timeouts <br>
