# Argus
Welcome to Argus


Hello Everyone, I am the founder of Argus, which will hopefully be a full stack SOC application : ) 

Welcome to the journey 


Testing#3


[MacBook (Victim)] ←→ [Home Network] ←→ [SOC Server]
     ↑                        ↑                        ↓
[MacBook (Attacker)]     [Router/Firewall]       [Dockerized Tools]
     ↓                        ↓                        ↓
[Phishing, Malware] → [Traffic Captured] → [Logs → Wazuh → Elastic SIEM]
                                                  ↓
                                        [TheHive + Cortex + Shuffle]

TODO List
---------------------------------------------
- Create a full stack SOC system to monitor network
     - Tools Needed (These are all open source):
	[] EDR/AV - Either OpenEDR or OSSEC
	[] Phishing - GoPhish
	[] Vulnerability Management - OpenVAS and Nikto for web servers
	[] Insider Risk/ DLP - myDLP (preferred) or openDLP if anything
	[] Cloud Security - CloudSploit
	[] Logging/SIEM - Elastic SIEM with Kibana and Beats or Wazuh
		- First, instak ELK stack (Elastic + logstash + kibana). Ensure it is up and running
       		- Second, attempt to integrate wuzuh into the ELK stack
           	- Create some garbage JSON to have it flow though the pipeline
	[] Logging - Shuffle + Wazuh + TheHive + Cortex = Automation Bliss
