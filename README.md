# Welcome to My project page

<h3>Cloud-Based SOC Project</h3>

Built a SOC lab on Vultr cloud including Windows and Ubuntu machines integrated with Elastic SIEM. Configured dashboards and alerts for login activity (Windows RDP & SSH). Simulated attacks using Kali Linux (brute force and Mythic C2 Apollo via PowerShell IEX) and monitored logs in ELK. Integrated alerts with osTicket for automated incident ticketing.

<h4>SOC Lab Architecture<h4/>
  
The diagram illustrates a cloud-based SOC setup on Vultr. Windows (RDP) and Ubuntu (SSH) servers forward logs via a Fleet server to Elastic/Kibana for centralized monitoring and alerting. A separate osTicket server generates tickets from alerts. An attacker’s Kali Linux machine and a Mythic C2 server simulate threats, while the SOC analyst accesses Elastic/Kibana via the web for detection and response.

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/0%20diagram%20for%20soc.jpg" alt="SOC Diagram" width="600" />

<h4>This SOC is built on VULTR Cloud</h4> 

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/vultr%20cloud.png" alt="Vultr Cloud" width="600" />

Working of Elastic Stack

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/working%20of%20elastic.png" alt="Elastic" width="600" />

Installed Elastic Search on ELK server

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/Intalled%20and%20configured%20elastic.png" alt="Elastic Configuration" width="600" />

Kibana service

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/2%20Kibana%20service%20installed.png" alt="Kibana Service Installed" width="600" />

Windows Server is created (vulnerable to RDP attacks)

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/3%20windows%20server%20(attack%20target).png" alt="Windows Server (Attack Target)" width="600" />

Installing Sysmon and ingesting logs into Elastic 

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/4%20intalled%20sysmon%20and%20ingesting%20logs%20into%20elastic.png" alt="Installed Sysmon and Ingesting Logs into Elastic" width="600" />

Sysmon logs in Elastic

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/5%20viewing%20sysmon%20logs%20in%20elasatic.png" alt="Viewing Sysmon Logs in Elastic" width="600" />

Elastic agent

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/5.png" alt="Project Image 5" width="600" />

Creating a SSH Server 

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/6%20Creating%20an%20SSH%20server.png" alt="Creating an SSH Server" width="600" />

Installing Elastic Agent on SSH server

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/7%20Installing%20Elastic%20agent%20on%20SSH%20server.png" alt="Installing Elastic Agent on SSH Server" width="600" />

Ingested SSH logs into Elastic

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/8%20Ingested%20SSH%20logs%20into%20elastic.png" alt="Ingested SSH Logs into Elastic" width="600" />

Created a Dashboard in Elastic to Monitor Successful(Accepted) and Unsuccesful(Failed) login Authentication to the SSH server

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/9%20Dashboard%20to%20monitor%20SSH%20Authentication%20on%20SSH%20server.png" alt="Dashboard to Monitor SSH Authentication on SSH Server" width="600" />

Created a Dashboard and a Table for Successful and Unsuccessful RDP Connection 

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/10%20Dashboard%20and%20table%20for%20RDP%20Failed%20and%20Successful%20Authentication%20in%20Elastic.png" alt="RDP Dashboard for Failed and Successful Authentication in Elastic" width="600" />

## Mythic C2 

<h3>A C2 (Command and Control) server is used by attackers to remotely control compromised systems, send commands, and exfiltrate data.</h3>

<h3>Mythic C2 is an open-source, customizable command-and-control framework that allows red teamers and penetration testers to simulate real-world adversary operations.</h3>

<a href="https://github.com/AbhiRaj-on-Git/phases_of_mythic_c2/tree/main" > Phases of a C2 server ? </a>

Creating a server for Mythic C2

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/13%20server%20for%20Mythic%20C2.png" alt="Server for Mythic C2" width="600" />

Mythic C2 installed

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/14%20installed%20Mythic%20C2%201.png" alt="Installed Mythic C2" width="600" />

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/14%20installed%20Mythic%20C2%202.png" alt="Installed Mythic C2 (Part 2)" width="600" />

Installed Kali Linux on Attacker machine 

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/15%20%20Kali%20linux%20for%20RDP%20brute%20force.png" alt="Kali Linux for RDP Brute Force" width="600" />

Using Hydra (Tool for brute forcing), brute-forcing into the Windows vulnerable machine

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/16%20hydra%20for%20brute%20force%20RDP%20(windows%20attack%20machine).png" alt="Hydra RDP Brute Force" width="600" />

Successful brute-force attempt

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/17%20hydra%20brute%20force%20successful%20RDP%20(windows%20attack%20machine).png" alt="Hydra Brute-Force Successful RDP" width="600" />

Logged into the Windows machine after successful brute force attempt

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/18%20logged%20into%20windows%20machine%20through%20RDP.png" alt="Logged into Windows Machine via RDP" width="600" />

(All these C2 Activity can be seen in the Elastic Dashboard along with other details)

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/19%20Elastic%20Instance%20dashboard%20displays%20logged%20session.png" alt="Elastic Dashboard - Logged Session Display" width="600" />

After logging into vulnerable windows machine through brute-forcing RDP connection
Installing Mythic C2 Apollo using Powershell IEX

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/20%20installing%20appolo%20agent%20from%20Mythic%20C2%20on%20target%20machine.png" alt="Installing Apollo Agent from Mythic C2 on Target Machine" width="600" />

Mythic C2 gets a call back from apollo installed device

we can now execute the commands from here

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/21%20Mythic%20C2.png" alt="Mythic C2" width="600" />

(Mythic C2 activities can be seen in the Elastic Dashboard)

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/23%20created%20alerts%20to%20track%20mythic%20c2%20activity.png" alt="Created Alerts to Track Mythic C2 Activity" width="600" />

osTicket

<h3>Ticketing software in a Security Operations Center (SOC) helps track, assign, and resolve security incidents by managing them as structured tickets</h3>

<h3>osTicket is an open-source ticketing tool that SOC teams can use to log, prioritize, and monitor cybersecurity alerts and incident response workflows</h3>

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/24%20Installing%20os%20ticket%20for%20ticketing.png" alt="Installing osTicket for Ticketing" width="600" />

Integrating Elastic Search Alerts with osTicket for handling Alerts using Webhook

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/25%20osTicket%20Elastic%20search%20integration%201.png" alt="osTicket Elastic Search Integration 1" width="600" />

(using api key)

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/25%20osTicket%20Elastic%20search%20integration.png" alt="osTicket Elastic search integration" width="600" />

Ticket is generated when an alert is generated

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/26%20Ticket%20is%20generated%20on%20elastic%20search%20alerts.png" alt="Ticket is generated on Elastic Search Alerts" width="600" />

## Investigating Mythic C2 telemetries

Mythic C2 telemetries can be viewed in the elastic 

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/27%20Investigating%20mythic%20c2.png" alt="Investigating Mythic C2" width="600" />

Artifacts collected 

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/28%20recorded%20artifacts.png" alt="Recorded Artifacts" width="600" />

## Elastic EDR 
<h3>Elastic EDR (Endpoint Detection and Response) is a security solution from Elastic that monitors, detects, and responds to malicious activity on endpoints in real time.</h3>

(Elastic EDR blocks the c2 when tried to execute on the Host)

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/27%20Using%20Elastic%20EDR.png" alt="Using Elastic EDR" width="600" />

Also isolates the Host when affected 

<img src="https://raw.githubusercontent.com/AbhiRaj-on-Git/project-images/main/29%20Elastic%20EDR%20completely%20isolates%20the%20host%20from%20connecting%20to%20network.png" alt="Elastic EDR Completely Isolates the Host from Connecting to Network" width="600" />

<h2>Thank you</h2>

Thank you for going through my project, this site consists some major parts of my project which demonstrates the servers and tools used and not the full project itself. 












