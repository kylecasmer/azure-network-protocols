<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In the tutorial below, I will observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create a resource group within Azure
- Create a Windows VM and a Linux VM
- Use Remote Desktop to connect to Windows VM
- Install Wireshark in Windows VM
- Filter by ICMP traffic in Windows VM
- Ping the private IP address of Linux VM from Windows VM
- In Windows VM, open Powershell, ping a public address, and observe traffic in Wireshark
- Initiate non--stop ping from Windows VM to Linux VM
- Open the Network Security Group that Linux VM is using and disable ICMP traffic
- Observe ICMP traffic in Wireshark
- Re-enable ICMP traffic
- Observe ICMP traffic in Wireshark again
- Filter for SSH traffic in Wireshark
- Type commands into Linux VM and observe the SSH traffic in Wireshark
- Filter for DHCP traffic in Wireshark
- Issue a new IP address in Windows VM from the command line
- Observe DHCP traffic in Wireshark
- Filter for DNS traffic in Wireshark
- Use nslookup in command line to find what the IP addresses are for a few public websites
- Observe DNS traffic in Wireshark
- Filter for RDP traffic in Wireshark
- Observe the non-stop spam of traffic
- Close Remote Desktop and delete the resource groups/VMs

<h2>Actions and Observations</h2>

<p> <img src="https://i.imgur.com/0lZWDUw.png height="80%" width="80%" alt="[Disk](https://) Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
