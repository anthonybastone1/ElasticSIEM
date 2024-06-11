<h1>Elastic Stack SIEM Home Lab</h1>

<h2>Description</h2>
This lab consists of setting up a home lab for Elastic Stack SIEM using the Elastic Stack web portal and a Kali Linux VM inside of VMWare. I also generated security events on the Kali VM, setup an agent to forward data to the SIEM, and query and analyze the logs in the SIEM.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Linux</b> 
- <b>VMware</b>
- <b>Elastic Agent</b>

<h2>Environments Used </h2>

- <b>Kali Linux VM</b>

<h2>Program walk-through:</h2>

<p align="center">
Setting up the Agent to Collect Logs: <br/>
<img src="https://imgur.com/ASJpQpK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Creating Telemetry:  <br/>
<img src="https://imgur.com/wDxjjpf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create a Dashboard to Visualize the Events:  <br/>
<img src="https://imgur.com/vodDS6D.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create an Alert to Detect Nmap Scans:  <br/>
<img src="https://imgur.com/fnKKgM1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/I81Zqwp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the Action You Want to Take When the Rule is Triggered:  <br/>
<img src="https://imgur.com/TYW1eLu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>


<h2>Conclusion</h2>
In this project, I set up a home lab using Elastic SIEM and a Kali VM. I configured the system to forward data from the Kali VM to the SIEM using the Elastic Beats agent, generated security events on the Kali VM using Nmap, and queried and analyzed the logs in the SIEM using the Elastic web interface. 

I also created a dashboard to visualize security events and then created an alert to detect security events. This home lab provided a valuable environment for learning and practicing the skills necessary for effective security monitoring and incident response using Elastic SIEM.

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
