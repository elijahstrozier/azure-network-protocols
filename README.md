<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />






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

- Create A Resource Group Using Microsoft Azure
- Create A Virtual Machine Running Windows 10
- Create Another Virtual Machine Running Linux (ubuntu 20.04)
- Install Wireshark

<h2>Actions and Observations</h2>

<p>

  >
</p>
<p>
Observe ping requests and replies within WireShark
From The Windows 10 VM, open command line or PowerShell and attempt to ping a public website (such as www.google.com) and observe the traffic in WireShark.

<![image](https://github.com/elijahstrozier/azure-network-protocols/assets/161254320/2ebe07f1-26d2-4f0a-b68b-e1f577dded41)

![image](https://github.com/elijahstrozier/azure-network-protocols/assets/161254320/c3ae036f-70ca-444f-8e38-b849614dade0)




  
Initiate a perpetual/non-stop ping from your Windows 10 VM to your Ubuntu VM.

Open the Network Security Group your Ubuntu VM is using and disable incoming (inbound) ICMP traffic
  
  
  
  -Back in the Windows 10 VM, observe the ICMP traffic in WireShark and the command line Ping activity
  -Re-enable ICMP traffic for the Network Security Group your Ubuntu VM is using
  -Back in the Windows 10 VM, observe the ICMP traffic in WireShark and the command line Ping activity (should start working)
  -Stop the ping activity

  <![image](https://github.com/elijahstrozier/azure-network-protocols/assets/161254320/45c30c11-fe82-461e-8f2e-67132367c42e)

.
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
