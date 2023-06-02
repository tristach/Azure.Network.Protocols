# Azure.Network.Protocols
<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/> 
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

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

- Create Resources: Create two VMs.  One with Windows-10, one with Linux.  
- Observe ICMP Traffic:  Install Wireshark on Windows VM.  Filter for ICMP messages only.
- Observe Using Wireshark:  Use the command line to perform various communication tasks between the two PCs.

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/JxPwNaD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Resourse group: Pandora with two VMs (Win-10 and Linux).
</p>
<br />

<p>
<img src="https://i.imgur.com/fSfT6Vi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Win-10 spamming everything.
</p>
<br />

<p>
<img src="https://i.imgur.com/49ZPSqp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Filtering only for icmp traffic using Wireshark.
</p>
<br />

<p>
<img src="https://i.imgur.com/SXFYoHd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Using perpetual ping on CMD line.
</p>
<br />

<p>
<img src="https://i.imgur.com/cWxx0Ay.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Creating new security rule on Azure to stop pings.
</p>
<br />

<p>
<img src="https://i.imgur.com/mpS3k5l.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Pings have now stopped.
</p>
<br />

<p>
<img src="https://i.imgur.com/3g7bmJ1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Logged into Linux VM through CMD.  Using SSH to establish a connection.
</p>
<br />

<p>
<img src="https://i.imgur.com/z10bsDp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now back monitoring dhcp traffic on Wireshark.
</p>
<br />


<p>
<img src="https://i.imgur.com/z10bsDp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Shows dns results for Microsoft website and traffic on Wireshark.
</p>
<br />

<p>
<img src="https://i.imgur.com/oaU9ix0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Final picture shows rdp using tcp port on Wireshark.
</p>
