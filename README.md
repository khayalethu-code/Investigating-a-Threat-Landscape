# Investigating-a-Threat-Landscape
Packet Tracer project lab investigating  three vulnerabilities that can be exploited by threat actors.

Project Name

Investigating a Threat Landscape

 Objectives

Part A: Investigate a Network Configuration Vulnerability
Part B: Investigate a Phishing Malware Vulnerability
Part C: Investigate a Wireless Network and DNS Vulnerability

The threat landscape consists of all the vulnerabilities that can be exploited by threat actors. Every cybersecurity incident involves the exploitation of vulnerabilities by different types of threat actors. Some threat actors want money, others want to be famous, and yet others want to destroy information and infrastructure.

In this Packet Tracer project lab, I will investigate three vulnerabilities that can be exploited by threat actors.

 Cybersecurity Skills Learned
•	Network Security Assessment
•	Threat Analysis & Mitigation
•	Attack Simulation & Defense
•	Security Investigation & Forensics
•	Risk Awareness & Strategy
•	Tool Proficiency & Security Mindset

Tools Used
•	CISCO Packet Tracer

 Steps

Part 1: Investigating a Network Configuration Vulnerability

Sometimes network security vulnerabilities can happen by accident. For example, forgetting to update server or host software may expose known vulnerabilities that could easily be mitigated with a simple update. Similarly, vulnerabilities may be introduced when a network device is not configured properly, or a device is defective. In this part, I will explore a vulnerability that results from a device that is not properly configured with security best practices.

Step 1: Used a guest network to gain access to other devices on the network on  Greenville and  clicked  Smartphone 3 just outside Home.

<img width="962" height="585" alt="image" src="https://github.com/user-attachments/assets/3e7504f6-31ad-4e6e-836a-637d7d69ba16" />

•	Clicked Smartphone 3, and then clicked Command Prompt then enter the command ping 192.168.100.101.
•	 The ping was successful , which proves the network is very vulnerable to attack, because  someone could take control of the webcam, for example, and watch video from inside the house. 

<img width="1018" height="541" alt="image" src="https://github.com/user-attachments/assets/22df1e19-d05f-466e-9542-fc4e8114da5b" />

Step 2: Explore the Home network to identify the vulnerability.
•	Clicked Home, because home routers typically control home wireless networks. So I  used the Home Office PC to connect to the router after  the IP address has been determined.

•	Clicked Home Office PC > Desktop tab > Command Prompt, and then entered  the command ipconfig.
In other words , the default gateway is the IP address for the Home Wireless Router which is 192.168.100.1 

<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/56d54c27-ed4b-4b18-9697-06856b6d97e2" />

•	I used the Web Browser on Packet tracer to connect to the Home Wireless Router. Entered  the default gateway IP address 192.168.100.1

<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/864ba9d5-e22b-47d8-be35-3374fd2bc463" />

•	Clicked Wireless and reviewed the basic wireless settings for each of the three radios that are part of the wireless router.
•	All the radios were active with their  SSIDs that are assigned to them

<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/1aab4942-4427-4d0d-b378-c5abc82ffaf1" />

•	 Clicked  the Wireless Security submenu to check if the security is activated for each of the radio and  passphrases set. Yes they were
<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/42c64466-acda-4b4f-add0-f2b97c8a5308" />

•	 I was able to access the network from outside without logging in; therefore, I investigated  further by  clicking the Guest Network submenu and investigate the settings and the Guest network was  active on 5 GHz-1 radio and the security mode was disabled which makes it vulnerable 

<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/6640f88c-dbe7-448e-841d-3960342096bb" />


•	The  wireless Guest network should only provide access to the internet for guests. It should not permit guests to access the devices on local network inside the house. In this case, guests can access the local network. This indicates that the home router is misconfigured.

Part 2: Investigating a Phishing Malware Vulnerability

Phishing is a type of social engineering attack where a threat actor disguises themself as being a legitimate, trusted source in order to trick the end user into installing malware on their device, or share personal or financial information.

 Phishing attacks typically come through emails or phone calls. Unlike other network vulnerabilities, the primary vulnerability in phishing attacks is the users of the network. For this reason, an important defense against phishing is training users on how to prevent phishing exploits.
In this part, I will simulate and investigate a phishing attack

Step 1: Pose as a threat actor and create a phishing email.
•	Navigated to the Cafe network to click the Cafe Hacker Laptop > Desktop tab > Email then  Clicked Compose. 

<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/856567d6-ceee-486e-9c0a-1eaa8ee4aee8" />

•	The objective is to persuade the user to copy and paste a URL from your email message into their browser. I sent the phishing emails to the following users:
user1@mail.isp.net
user2@mail.isp.net
user3@mail.isp.net
Step 2: Open the emails received from the threat actor
•	Navigated to the Branch Office and clicked one of the devices, either PC-BR1
•	Clicked  Desktop tab > Email, and then click Receive. And the email was received

<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/c0877891-d7ce-4cd4-9d55-51b0987f8494" />

Step 3: Pose as a victim and follow the phishing instructions.

•	 On PC-BR1 read the email and copy the website address on the Mail Browser window, and then click Web Browser to paste the URL into the URL field, and then Go as shown below 

<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/fb24f479-e932-47bf-843d-5c5056bb4428" />

•	Unfortunately, I used an invalid Domain name so that why the output is Domain Name Unresolved

•	If the email virus spreads this message to everyone in the network, those users also follow the instructions, then numerous hard drives could be encrypted and a lot of data potentially lost. In some cases, companies and other organizations have paid thousands of dollars in hopes of recovering the encrypted data.

Risk Mitigation

Employees should be trained how to identify phishing emails and the actions that should be taken to prevent damage from them. In addition, organizations can configure firewalls, intrusion prevention systems, and other security devices and software, to block phishing emails before entering the network. 
Some businesses subscribe to services that compile and maintain lists of malicious websites. The security devices in the organization can then uses these lists to automatically update filters for blocking malicious traffic.

Part 3: Investigate a Wireless Network and DNS Vulnerability

The  average network user tends to trust open Wi-Fi networks out in public places. Using Wi-Fi instead cellular data services can provide faster data rates and be more cost effective.

However, threat actors can configure a laptop with a Wi-Fi interface that can act as both a Wi-Fi access point and a Wi-Fi client. This means that threat actors can create their own wireless networks and broadcast a convincing SSID to potential victims in public places. 

Threat actors use these rogue access points to create main-in-the-middle attacks. In this attack, threat actors can capture and read all the wireless traffic from devices that associate with the rogue access point, potentially learning usernames, passwords, and other confidential information.
In this part, I will investigate how a rogue access point can be used to entice users to connect to a fake wireless network. When combined with network services such as DHCP and DNS, users can become victims of malicious website attacks through DNS hijacking

Step 1: Connect to the threat actor’s wireless network.

Navigated to the Cafe and clicked the Hacker Backpack to investigate the contents. In his backpack, he has a wireless router and a network sniffer. The goal is to intercept user traffic and direct it to a malicious server. 

<img width="962" height="504" alt="image" src="https://github.com/user-attachments/assets/6cb348ac-c523-4988-8758-3122686f6a82" />

•	Returned to the Cafe and clicked the Cafe Customer laptop > Desktop tab > PC Wireless application. 

<img width="962" height="1302" alt="image" src="https://github.com/user-attachments/assets/fea5cf1f-fda4-4aa2-8778-4a4f67168021" />

•	If I was in the Cafe with my laptop, I was going to connect to the Cafe_WI-FI_FAST network because it is very tempting.

 It is named to look legitimate, but better than the real network. Also, it has a slightly stronger signal than the legitimate network. The Cafe_WiFi network is the only one with security enabled.
 
Step 3: Investigate the source of the attack.

•	Clicked IP Configuration and in the Cafe, I clicked VPN Laptop > Desktop tab > IP Configuration to compare the values between the two devices. 

<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/d706b659-1886-4df4-a042-e338b6cc264b" />

•	The host IP addresses are different, but this is normal. Each host on a LAN needs a unique IP address. The subnet masks are the same. The DNS server addresses are different.

•	Moved into Cafe to investigate the , I found that it’s IP address is  192.168.10.199 and it the same as the DNS server address that is configured on the Cafe Customer laptop 

<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/162c9012-1ffd-4aa5-9c37-fba93b4e052b" />

•	On the Café Hacker Laptop, I clicked the Services tab > DNS to locate the Name for the friends.example.com website. Note that the IP address is the same IP address as is associated with pix.example.com from the phishing attack earlier. 

<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/f9bb3b1e-2455-49c•	Under Services, clicked DHCP and noticed that the DNS server address distributed to the hosts over DHCP is the same one assigned to Café Customer. 5-b90a-10b2f85981dd" />

<img width="962" height="541" alt="image" src="https://github.com/user-attachments/assets/b8ac5221-4d3e-47c2-8d25-daee2a94422a" />

Steps In The Attack

When Cafe Customer connected to the rogue access point's wireless network, it received an IP address configuration from DHCP. 
The DHCP server is configured to distribute the hacker laptop address as the DNS server address. 

The DNS server on the Cafe Hacker Laptop associates the IP address of a malicious server, 10.6.0.250, with the name of a popular website, friends.example.com.

 When the user of the Cafe Customer laptop tries to visit the website, traffic is redirected to the malicious server instead.
 Ransomware is then installed on Cafe Customer laptop the user's files are encrypted.
















