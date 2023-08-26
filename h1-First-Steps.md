# Table of contents

1. Darknet Diaries Podcast
2. Hutchins et al 2011: Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains
3. Install Debian 12-Bullseye virtual machine in VirtualBox

# Darknet Diaries Podcast 

> https://darknetdiaries.com/episode/124/

## Summary

- In this darknet diaries podcast, episode 124, the host Jack tells the story of how a hacker was able to bypass Facebook's security measures and how he gained access to internal information about the company's operations.

- The hacker was Evaldas Rimasauskas, a guy from Lithuania who wanted to scam Facebook for a lot of money.
- How did he managed to do this ? They have used social engineering tactics. He and his team collected information about Facebook's operations such as names of the contractors and amounts paid to them.  They have created fake invoices and sent them to Facebook from a legitimate-looking email address from on of Facebook's contractors, Quantum Computers.
  - What is social engineering ? it's the use of psychological manipulation to trick people into divulging sensitive information. In this case, it involves impersonating someone.
- The hackers were able to trick Facebook into paying these fake invoices and were able to steal million of dollars. They have also managed to scam Google.
- Facebook and Google eventually discovered the scam and worked with the FBI to have  Evaldas arrested.
- This story shows the importance of taking protective measures against cyber attacks.
  - For example, companies should train their employees to be able to recognize phishing.

> A question I have for this episode is why did it take that much time before Quanta Computers realised that they weren't getting paid ?

# Hutchins et al 2011: Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains

> https://lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Intel-Driven-Defense.pdf

## Summary

### Abstract

- Anti virus and intrusion detection can only focus on on aspect of the risk. 
- Advanced Persistent Threats (APTs) are a new type of threat by very skilled attackers. They usually target highly sensitive information such as economic or national security data.
- APTs use advanced techniques that can easily outsmart the standard defence mechanisms.
- However, defenders can learn and understand how APTs work and can adapt their defense mechanisms.
- Kill Chain Model is a model that describes the different stages of an attack.
- With the evolution of the threats, we now need to use intelligence-based model.

### 3.2 Intrusion Kill Chain

- A Kill Chain is a systematic process to target adversaries
  - The U.S military also uses kill chain with steps such as find, fix, track, engage and assess.
  - A Kill Chain is an end-to-end process. If one step fails, it will interrupt the entire process.
- For intrusions, a Kill Chain model consists of stages:
  1. Reconnaissance: researching and selecting targets by searching the internet for information from mailing list such as email addresses.
  2. Weaponization: combining a remote access trojan with an exploit to create a harmful payload. Usually, PDF files are used to deliver these harmful payloads
  3. Delivery: the weaponized payload is delivered to the target environment. The most common delivery methods are email attachments, websites and USB removable media.
  4. Exploitation: when the weapon has been delivered to victim host, the exploit will then be triggered. This will target vulnerabilities in applications or in the operating system.
  5. Installation: this will be the installation of a backdoor or a trojan in the system of the victim.
  6. Command and Control (C2): the compromised computer will send a signal to an external server for control. When connected, the attackers gain direct control over the target system.
  7. Actions on Objectives: now the attackers can take actions to achieve their goals. Usually their main goal is data exfiltration, which consists of collecting, encrypting and extracting information from the victim's environment. 

### 3.3 Courses of Action

- The intrusion Kill Chain helps the defenders understand how the attackers target a system. 
- Table 1 is a matrix that illustrates actions (detect, deny, disrupt, degrade, deceive & destroy) that the tools are able to do.

<img width="419" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/c305cea6-b8d1-4a5e-9fed-4057faf01fc1">

 - Being complete in security is very important as it lead to resiliency.
- Protecting against "zero-day" exploits is important but it is not the only concern.
- The key to achieve resiliency against persistent adversaries is a defensive strategy. 
- This strategy consists of concentrating on patterns that attackers repeat such as the tools they use.
- Defenders can measure how resilient their defenses are by looking at how their actions work against hackers.
- As illustrated below, defenders initially succeed in protecting their system, but attackers will soon find a way later on. This means that defenders will need to improve their defences to counter the new attacks.

<img width="338" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/940ad858-ab3e-4dba-af55-b1282d3b1b68">

This approach shows continuous improvement, defenders need to keep learning from attacks and adjust their defenses accordingly so that they can remain effective against threats that keep on evolving.

# Install Debian 12-Bullseye virtual machine in VirtualBox

> https://terokarvinen.com/2021/install-debian-on-virtualbox/

## STEPS

1. Install VirtualBox
2. Download Debian ISO image
3. Create a new virtual machine
4. Insert Debian ISO Image as Virtual CDROM
5. Boot to Desktop

## 1. Install VirtualBox

Install VirtualBox if you don't have it yet, [download VirtualBox installer](https://www.virtualbox.org/wiki/Downloads). I'm using the Oracle VM VirtualBox

## 2. Download Debian ISO image

Download the current Debian ISO image: debian-live-12.1.0-amd64-xfce.iso

> This might take some time, don't hesitate to use your phone as a hotspot

## 3. Create a new virtual machine

1. Click on New

2. Be sure to be on expert mode

3. Complete this step by following the images below until you press "Finish"

   You will now see your virtual machine on the left side of the VirtualBox Manager

   <img width="518" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/d7ae964a-89cc-49e1-a630-70a877780ed2">
<img width="401" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/59150df0-52e6-4e0a-a70d-0da9af4e8916">

## 4. Insert Debian ISO Image as Virtual CDROM

<img width="494" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/956c1a30-31a0-4779-8175-9574d05c0796">


## 5. Boot to Desktop

1. Choose the "Live system (amd64)" and press ENTER to boot

<img width="268" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/3c2e75ef-9bd5-4411-9e53-4e49d4714d5f">


2. Click on "Install Debian"

<img width="323" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/998ad899-a1e7-4548-8763-57f125838920">


3. Choose the language for the system

   > Why English ? universal language. If you have any problems, it will be easier for the agent help you debug the problem if he can understand your language.

<img width="341" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/57a7ea96-bf7d-4fe3-b8fe-59b1387831a2">


4. Click Finland on the map

   > The numbers and dates locale will be set to Finnish

<img src="C:\Users\ferna\OneDrive - HESSO\Documents\02_School\00_HAAGA-HELIA\Semester VII\01_Information Security - Tero Karvinen\01_Assignments\h1\h1\image-20230825184356132.png" alt="image-20230825184356132" style="zoom:67%;" />

5. Choose the keyboard you have on your computer.

<img width="335" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/b51012ef-6b1c-4be5-bcc4-91e0c87f302d">


6. Erase disk

   > This will delete everything on your virtual disk.

<img width="332" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/23185826-1bf7-48e2-aebd-b876401c7e99">


7. Users

   > Complete this part with your information

<img width="338" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/f0184bd8-88df-4e40-b85f-8d9dbd11a664">


8. Then click on "Install"

<img width="283" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/ee267179-60ad-431b-ab75-547f1292c4fe">


9. Be patient..! really patient ..

<img width="409" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/62812b0e-b737-45c5-a038-8dc09d415ff9">


10. Restart

<img width="416" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/dafaec12-e104-4437-af96-a51d50287ba4">


11. Log in

<img width="266" alt="image" src="https://github.com/piafernandez/h1-First-Steps/assets/71267247/98d0091a-0410-41ae-a5b6-a6d3abaf94cf">


12. Try browsing the internet to verify that everything is working !



# Sources and links

- Cybercrime 20.09.2022. EP 124: Syntetic remittance. Darknet Diaries. URL:https://darknetdiaries.com/episode/124/ Accessed: 25.08.2023

- Eric M. Hutchins, Michael J. Cloppert , Rohan M. Amin, Ph.D. Lockheed Martin Corporation. Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains. URL:https://lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Intel-Driven-Defense.pdf Accessed: 25.08.2023

- Tero Karvinen 2023. Install Debian on Virtualbox - Updated 2023 URL: https://terokarvinen.com/2021/install-debian-on-virtualbox/ Accessed: 25.08.2023


