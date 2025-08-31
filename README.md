# Welcome to My project page

<a href="https://github.com/AbhiRaj-on-Git/phases_of_mythic_c2/tree/main"> Phases of Mythic C2 </>

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


