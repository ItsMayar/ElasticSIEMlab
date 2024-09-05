<h1>Elastic Stack SIEM Implementation and Security Event Management</h1>

<h2>Description</h2>
In this project, I successfully implemented and configured Elastic Stack SIEM in a home lab environment. The setup included deploying a Kali Linux VM and configuring Elastic Agents for efficient log collection and forwarding data to the SIEM, enabling robust security event monitoring.I gained practical experience by generating and analyzing security events using Nmap on the Kali Linux platform, which enhanced my ability to query Elastic SIEM for identifying and investigating security incidents. This project allowed me to develop a custom dashboard within Elastic SIEM, enabling effective visualization of security events and showcasing my skills in data interpretation and pattern recognition. Additionally, I created and tested alert rules for detecting specific security events, demonstrating my proficiency in proactive incident response and alert management.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Kali Linux</b> 
- <b>Elastic</b>
- <b>VirtualBox or VMware</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
1) Log into your Elastic SIEM instance and navigate to the Integrations page.
<br/>
2) Add Elastic Defend: <br/>
<img src="https://i.imgur.com/CH12MSf.png" height="70%" width="70%" alt="Elastic"/>
<br />
<br />
3) Install Elastic Agent on your Kali VM: <br/>
<img src="https://i.imgur.com/HqTLFpL.png" height="70%" width="70%" alt="Elastic"/>
<br />
<br />
4) Paste the selected command for Linux into the Kali terminal: <br/>
<img src="https://i.imgur.com/bI7R8ry.png" height="70%" width="70%" alt="Elastic"/>
<br />
<br />
<img src="https://i.imgur.com/ltgtMhk.png" height="70%" width="70%" alt="Elastic"/>
<br />
<br />
5) Verify the agent is working, by generating security-related events on your Kali VM using Nmap. 
<br /> 
<img src="https://i.imgur.com/icz0dOn.png" height="70%" width="70%" alt="Elastic"/>
<br />
Nmap is a free and open-source utility used for network exploration, management, and security auditing. It is designed to discover hosts and services on a computer network, thus creating a “map” of the network. Nmap can be used to scan hosts for open ports, determine the operating system and software running on the target system, and gather other information about the network.
<br />
<br />
6) With the data from the Kali VM now forwarded to the SIEM, we can begin querying and analyzing the logs: <br/>
<img src="https://i.imgur.com/TnC15lI.png" height="70%" width="70%" alt="Elastic"/>
<br />
<br />
7) Create an alert in the Elastic SIEM instance that will monitor the logs for Nmap scan events and then notify user when detected:
<br/>
<img src="https://i.imgur.com/3h4tzXc.png" height="70%" width="70%" alt="Elastic"/>
<br />
<br />
In a SIEM, alerts are a crucial feature for detecting security incidents and responding to them in a timely manner. Alerts are created based on predefined rules or custom queries, and can be configured to trigger specific actions when certain conditions are met. <br/>
<img src="https://i.imgur.com/VCbdaaI.png" height="70%" width="70%" alt="Elastic"/>
<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
