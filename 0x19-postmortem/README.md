## PARLONS DIGITAL SERVER infrastructure outage incident report


This is the incident report regarding the outage of my digital solution company's infrastructure PARLONS DIGITAL that occurred this November 29, 2022. We understand that this service issue has impacted our valued developers and users, and we apologize to all those affected.

https://www.parlons-digital.com


# Timeline (all times MEA Time)
	
Day 1 : Converse with namesheap team for understandign the problem
Day 2 : Backup the last sauvegarde (12th october) for recover all configuration (Not succes)
Day 3 : Backup the last sauvegarde (13 September) (Not succes)
Day 4 : Our developper enter the server to scan full server

    - 6:19 PM: Scan server 
    - 8:30 PM: Find de malicious file
    - 22:00 PM: deleted all malicious file
    - 23:00 PM: Backup server  
    - 23:30 PM: recover the projects on github to share on the server
    - 00:00 PM: Connect on server with filezila to push the projects 
    - 01:58 PM: Propogation on the DNS
    - 03:10 PM: of trafic back online

# Root Cause

After deploying a website developed in HTML and CSS, we noticed an unexpected redirection of all our projects as well as those of our clients.
After investigations, the developers realized that there were two websites that were not secure with a ssl certifcat;
A hacker exploited these exploits to penetrate the root files of our server.
This malicious file, redirected our domains to another domain, also this file automatically created email accounts based on the existing domains

# Resolution and recovery

At 18:55, we were alerted by an internal system that informs us that there is a problem loading files on the server.
A few minutes later, a client contacts us because he could not consult the training offers page.
At 19:10, we launch a general analysis on the server and a deep scan on the server.
After several investigations and exchanges with the Namesheap team, our developers were able to find the malicious files on our server.
So we deleted all the corrupted files on the server, changed the server password and activated the 2FA server (it was not activated before)
    

# Corrective and Preventative Measures

- Set up a scanning protocol every weekend.
- Change the password every month end
- Avoid hosting a website without SSL certificate
- Provide a 2FA connection for each user connection on the server
- Pay attention to Livewire-laravel when sending a form from a user

PARLONS DIGITAL is committed to continually and quickly improving our technology and operational processes to prevent outages. We appreciate your patience and again apologize for the impact to you, your users, and your organization. We thank you for your business and continued support.

Sincerely,

The Developer Infrastructure Team


Posted by El Hadj Youssouf Ouattara, Editor