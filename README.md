<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
Observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />

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

1. Create and Deploy Resources and Define Security Rules: Create NSGs with specific inbound and outbound security rules to allow or deny traffic. These rules can be based on source IP addresses, destination IP addresses, ports, and protocols.
2. Grouping Resources: Consider grouping resources based on their functions or roles. Create NSGs that can be associated with multiple VMs or subnets, making management more efficient.
3. Create Network Security Groups: Create NSGs with the predefined security rules. Associate the NSGs with the respective Azure Virtual Machines or subnets. This association enforces the defined rules for inbound and outbound traffic.
4. Verify the rules: Test the NSGs by sending traffic between the VMs. Verify that the intended traffic is allowed and unauthorized traffic is denied as per the defined rules.

<h2>Actions and Observations</h2>

<p>  
<img src="https://i.imgur.com/lxsKnw8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create and Deploy Resources - Two Virtual Machines - VM1 and VM2 created.
</p>
<br />

<p>
<img src="https://i.imgur.com/f9o4Dh1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Capturing and observing the internet traffic.
</p>
<br />

<p>
<img src="https://i.imgur.com/1EeCbi1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Edit the inbound rules to deny traffic below ports number 300.
</p>

<p>
<img src="https://i.imgur.com/KtPZjc2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Observing the new inbound rules being inforce.
</p>
<br />
