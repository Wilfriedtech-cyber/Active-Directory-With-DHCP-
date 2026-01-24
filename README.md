Introduction 
Welcome to my first lab detection and monitoring homelab 
Goals 
The purpose of this lab is to develop detection skills with splunk by simulating attacks on vulnerable machines and send those logs to my splunk siem. 
Why did i choose thius lab?
As i was building my skills after i passed my btl1 i Wanted to build something from scrath and see how everything workls in the background of getting logs uploaded to splunk and working on detection rules. So i looked up online on any type of soc lab udeas and i found two interesting one shout out to Nakkouch Tarek (link) and Day johnson(link). 
Essentially I didn't want to create something identical and be a little bit creative.However for now I will start with a small network topology and build upon this foundation 
sKILLS GAINED?
SPLUNK SEARCHES
LOGS CORRELATION
DOCKER
SYSMON LOGS INVESTIGATION
ETC...

lAB EXPLAINED
1-) The employee/analyst will be connected to the internal network to only access the splunk server through openvpn

2-) a public IP will be assigned to the fortigate NGFW with open port 22 and 80 to perform port forwarding to the actual ip of the vulnerable server hosting the dvwa and the ssh cowrie honeypot

3-) PFSENSE WILL BE USED AS A ROUTER,FIREWAll,IDS/IPS WITH SURICATA AND ALL THE LOGS WILL BE FORWARDED TO THE SPLUNK SERVER 

4-) Sysmon will be installed on the domain controller and the client just to monitor the logs on it in case the client or dc gets compromised 
Stay tuned as I will explain how i built this lab :)
