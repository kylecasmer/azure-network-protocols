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

<p> 1.Create a resource group in Azure
<p> 2.Create a Windows VM and a Linux VM

<p> <img src="https://i.imgur.com/0lZWDUw.png height="80%" width="80%" alt="[Disk](https://) Sanitization Steps"/>

  
<p> 3.Use Remote Dsktop to connect to Windows VM
<p> 4.Install Wireshark in Windows VM


<img src="https://i.imgur.com/tsLSjR4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<p> 5.Filter by ICMP traffic in windows VM
<p>


<img src="https://i.imgur.com/vxCTb2a.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p> 6.Ping the private IP address of Linux VM from Windows VM using Windows Powershell
</p>


<img src="https://i.imgur.com/ij2FThu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<p> 7.In Windows VM, open Powershell, ping a public address, and observe traffic in Wireshark


<img src="https://i.imgur.com/83D0ezU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<p> 8. Initiate non-stop ping from Windows VM to Linux VM
</p>


<img src="https://i.imgur.com/mtRrYIe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<p> 9. Open the Network Security Group that Linux VM is using and disable ICMP traffic
</p>


<img src="https://i.imgur.com/Ji0DcZv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<p> 10. Observe ICMP traffic in Wireshark



<img src="https://i.imgur.com/lAUHJ4g.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<p> 11. Re-enable ICMP traffic
<p> 12. Ovserve ICMP traffic in Wireshark again
<p> 13. Filter for SSH traffic in Wireshark



<img src="https://i.imgur.com/DpiIY01.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<p> 14. Type commands into Linux VM and observe the SSH traffic in Wireshark
</p>


<img src="https://i.imgur.com/5nZE5sX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<P> 15. Filter DHCP traffic in Wireshark
</P>


<img src="https://i.imgur.com/Vznb62B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<P> 16. Issue a new IP address in Windows VM from the command line
<P> 17. Observe DHCP traffic in Wireshark



<img src="https://i.imgur.com/HdlWkTf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<P> 18. Filter for DNS traffic in Wireshark


<img src="https://i.imgur.com/DToPbag.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<P> 19. Use nslookup in command line to find what the IP addresses are for a few pulic websites
</P>



<img src="https://i.imgur.com/WaYRDDb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<p> 20. Observe DNS traffic in Wireshark
<p> 21. Filter for RDP traffic in Wireshark



<img src="https://i.imgur.com/B5uMhvT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



<p> 22. Observe the non-stop spam of traffic
<p> 23.Close Remote Desktop and delete the resource groups/VMs
