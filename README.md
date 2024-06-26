<h1>Elastic Stack SIEM Home Lab</h1>

<h2>Description</h2>
This lab consists of setting up a home lab for Elastic Stack SIEM using the Elastic Stack web portal and a Kali Linux VM inside of VMware. I also generated security events on the Kali VM, set up an agent to forward data to the SIEM, and query and analyze the logs in the SIEM.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Linux</b> 
- <b>Elastic Agent</b>

<h2>Environments Used </h2>

- <b>VMware</b>
- <b>Kali Linux VM</b>

<h2>Program Walk-Through:</h2>

<p align="center">
<br />
After Successfully Installing Elastic Agent, I Began Generating Security Events on the Kali VM:  <br/>
<img src="https://imgur.com/Y3OUufU.png" height="80%" width="80%"/>
<br />
<img src="https://imgur.com/mDaRUyj.png"height="80%" width="80%"/>
<br />
<br />
<br /> 
<br />
<br />
Then I Began Querying for Security Events in the Elastic SIEM:  <br/>
<img src="https://imgur.com/azhNKzd.png" height="80%" width="80%"/>
<br />
<img src="https://imgur.com/WOHvQMm.png"height="80%" width="80%"/> 
<br />
<br />
<br /> 
<br />
<br /> 
Here I Created a Dashboard to Visualize the Events:  <br/>
<img src="https://imgur.com/ZWkndDB.png" height="80%" width="80%"/>
<br />
<br />
<br /> 
<br />
<br />  
The Process for How I Created an Alert to Detect Nmap Scans:  <br/>
<img src="https://imgur.com/0JkrWYR.png" height="80%" width="80%"/>
<br />
<img src="https://imgur.com/6Lw0LL6.png" height="80%" width="80%"/>
<br />
<img src="https://imgur.com/bwdk2eL.png" height="80%" width="80%"/>
<br />
<img src="https://imgur.com/wddPVex.png" height="80%" width="80%"/>
<br />
<img src="https://imgur.com/8AiWgmj.png" height="80%" width="80%"/>
<br />
<img src="https://imgur.com/cJp97kz.png" height="80%" width="80%"/> 
<br />
<br />
<br /> 
<br />
<br />  
After implementing the new alert, I attempted to put the Elastic SIEM to the test and trigger an alert. However, an alert was not triggered when I performed an nmap scan. I soon realized that the custom query I created was the issue. So I changed the query from event.action: "nmap_scan" to process.name: "nmap"  <br/>
<img src="https://imgur.com/YrBIyJt.png" height="80%" width="80%"/>
<br />
<img src="https://imgur.com/bKpy8OM.png" height="80%" width="80%"/>
<br />
<br />
<br /> 
<br />
<br />
Once I Made the Change to the Custom Query, I attemped Another Nmap Scan
<img src="https://imgur.com/j1mXTBd.png" height="80%" width="80%"/>
<br />
<br />
<br /> 
<br />
<br />
Once the Next Scan Occurred, an Alert was Successfully Triggered and an Email was Sent so I Could Be Notified
<img src="https://imgur.com/b9Doryh.png" height="80%" width="80%"/>
<br />
<img src="https://imgur.com/klwMUfu.png" height="80%" width="80%"/>
</p>
<br />
<br />
<h2>Conclusion</h2>
In this project, I set up a home lab using Elastic SIEM and a Kali VM. I configured the system to forward data from the Kali VM to the SIEM using the Elastic Beats agent, generated security events on the Kali VM using Nmap, and queried and analyzed the logs in the SIEM using the Elastic web interface. 
<br />
<br />
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
