<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this lab, I observed various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. I also was able to gain knowledge and experince with Virtual Machines, Remote desktops, command lines, Network Protocols, Wireshark, and operating systems.  <br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>Actions and Observations</h2>


- Create Virtual Machines using Microsoft Azure with the Windows 10 and Unbuntu(Linux) server.
 ![image](https://github.com/terranceharris1/azure-network-protocols/assets/142275089/4c4d3679-fd73-4e7e-a662-2ecc1a15dc16)
- Used Remote Desktop to connect the virtual machine.
 ![image](https://github.com/terranceharris1/azure-network-protocols/assets/142275089/d89267b9-5f1b-4c3c-9a25-d2b58f12cdc7)
- Filtered WireShark to only show ICMP so that I could ping the Unbuntu Server using its private IP address. 
 ![image](https://github.com/terranceharris1/azure-network-protocols/assets/142275089/5ad5a414-4b93-4fae-8957-12ca061ba384)
 ![image](https://github.com/terranceharris1/azure-network-protocols/assets/142275089/14c105ca-8b5b-464c-b0fc-f5a0f208cfed)
![image](https://github.com/terranceharris1/azure-network-protocols/assets/142275089/e5151760-0f60-4e28-b63e-b9bb896a634d)
- Disabled Unbuntu's inbound ICMP and watched how there was no response found in WireShark
  ![image](https://github.com/terranceharris1/azure-network-protocols/assets/142275089/f66894da-47de-4d8f-a808-b2715acb799e)
- Used WireShark and PowerShell to SSH into the second virtual machine I created.
 ![image](https://github.com/terranceharris1/azure-network-protocols/assets/142275089/3d51fe1a-d58d-4e03-8f19-b7e4474dadb5)
![image](https://github.com/terranceharris1/azure-network-protocols/assets/142275089/a527170f-fbe1-4648-b8f5-7ea0ae59e746)
- Observed DNS traffic and the addresses of common websites 
![image](https://github.com/terranceharris1/azure-network-protocols/assets/142275089/6c243785-9a6d-4a9d-beac-3f27238ce7c3)
- Observed RDP Traffic using the filter TCP.port==3389 and took note of the different packets.
  ![image](https://github.com/terranceharris1/azure-network-protocols/assets/142275089/2521734b-e4a5-4edf-9dd7-3269bdc0c7f9)
