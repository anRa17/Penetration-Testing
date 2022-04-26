# Penetration-Testing
<p> Step 1: Google Dorking<br>
Using Google, can you identify who the Chief Executive Officer of Altoro Mutual is:<br>
 Karl Fitzgerald
How can this information be helpful to an attacker:<br>
The information can be used during recon or phishing. </p>
<br>Step 2: DNS and Domain Discovery<br>
Enter the IP address for demo.testfire.net into Domain Dossier and answer the following questions based on the results:
Where is the company located:
Sunnyvale, CA
What is the NetRange IP address:
65.61.137.64-65.137.127
What is the company they use to store their infrastructure:
Rackspace Backbone Engineering
What is the IP address of the DNS server:
65.61.137.117
<brStep 3: Shodan<br>
What open ports and running services did Shodan find:
The ports that appeared open using Shodan were: 80, 443 ,8080
The services running were: Apache Tomcat/Coyote JSP Engine 
<br>Step 4: Recon-ng<br>
Install the Recon module xssed.
Set the source to demo.testfire.net.
Run the module.
Is Altoro Mutual vulnerable to XSS: Vulnerable 
<br>Step 5: Zenmap<br>
Your client has asked that you help identify any vulnerabilities with their file-sharing server. Using the Metasploitable machine to act as your client's server, complete the following:
Command for Zenmap to run a service scan against the Metasploitable machine:
Nmap -T4-A-v192.168.0.10 
Bonus command to output results into a new text file named zenmapscan.txt:


<p> 
 Zenmap vulnerability script command:
Nmap –script samba-vuln-cve-2012-1182 192.168.0.10
Once you have identified this vulnerability, answer the following questions for your client:


What is the vulnerability:<br>
SMB 3
Why is it dangerous:<br>
This vulnerability allows for the attacker to successfully upload a shared library and execute it. <br>
What mitigation strategies can you recommendations for the client to protect their server: Block port:445

</p>
