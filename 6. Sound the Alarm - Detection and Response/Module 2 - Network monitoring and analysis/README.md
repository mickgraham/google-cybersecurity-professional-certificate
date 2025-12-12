# Module 2: Network Monitoring and Analysis

## Overview

* Network traffic flows
* Packet sniffers
* Packet analysis

## Network Traffic Flows

Network traffic refers to the amount of data moving across a network, while network data is the data transmitted between devices. In large organizations, there can be a massive volume of network traffic, making it crucial to distinguish between normal and abnormal activity. By understanding expected network traffic patterns, security professionals can easily spot unusual behaviour.

* **Indicators of Compromise (IoC)** Provide analysts with specific evidence associated with an attack, such as a known malicious IP address, which can help quickly identify and respond to a potential security incident.
* **Data exfiltration** is the unauthorised transmission of data from a system, often involving sensitive information like usernames or intellectual property.

### Attacker's Perspective on Data Exfiltration

* Attackers first gain initial access, often through social engineering like phishing, to compromise a system.
* After gaining access, they perform lateral movement to explore the network, expand access, and identify valuable assets such as sensitive data.
* Attackers collect, package, and prepare the identified data for exfiltration, often reducing its size to evade security controls.
* Data is then exfiltrated to the attacker's chosen destination, which can involve methods like emailing stolen data from a compromised account.

### Defending Against Data Exfiltration Attacks

* Implement measures like multi-factor authentication to protect against phishing.
* Develop a baseline of normal or expected behaviour.
* Continuously monitor network activity for suspicious behaviour and maintain an asset inventory with appropriate security controls.

Organizations may deploy a **network operations center (NOC)**, which is an organizational unit that monitors the performance of a network and responds to any network disruption, such as a network outage. While a **security operations centers (SOC)** is focused on maintaining the security of an organization through detection and response, a NOC is responsible for maintaining network performance, availability, and uptime.

## Packet sniffers

**Network protocol analysers (packet sniffers)** are tools designed to capture and analyse data traffic within a network. Examples of network protocol analysers include tcpdump, Wireshark, and TShark.  They inspect packets for indicators of compromise, creating a **packet capture (P-cap)** file that contains intercepted data packets.

Contents of a packet:

* **Header:** Contains information such as the network protocol, port, and source/destination IP addresses. Protocols are rules for data transmission, and ports organise data transmission.
* **Payload:** This is the actual data being delivered, comparable to the content of a letter inside an envelope.
* **Footer:** Signifies the end of the packet.

Beyond their use in security as an investigative tool used to monitor networks and identify suspicious activity, network protocol analysers can be used to collect network statistics, such as bandwidth or speed, and troubleshoot network performance issues, like slowdowns.

Network protocol analysers can also be used for malicious purposes. For example, malicious actors can use network protocol analysers to capture packets containing sensitive data, such as account login information.

## Packet analysis

**Tcpdump** is a command-line network protocol analyser used to capture network traffic.

Here is a breakdown of the tcpdump syntax for capturing packets:

`sudo tcpdump [-i interface] [option(s)] [expression(s)]`

* The **sudo tcpdump** command begins running tcpdump using elevated permissions as sudo.
* The **-i** parameter specifies the network interface to capture network traffic. You must specify a network interface to capture from to begin capturing packets. For example, if you specify -i any you'll sniff traffic from all network interfaces on the system.
* The **option(s)** are optional and provide you with the ability to alter the execution of the command.
* The **expression(s)** are a way to further filter network traffic packets so that you can isolate network traffic.

Example command output (`sudo tcpdump -i any -v -c 1`):

![tcpdump](./tcpdump.png)

* **Timestamp:** The output begins with the timestamp, which starts with hours, minutes, seconds, and fractions of a second.
* **Source IP:** The packet's origin is provided by its source IP address.
* **Source port:** This port number is where the packet originated.
* **Destination IP:** The destination IP address is where the packet is being transmitted to.
* **Destination port:** This port number is where the packet is being transmitted to.

## Glossary: Network Monitoring and Analysis

**Command and control (C2):** The techniques used by malicious actors to maintain communications with compromised systems

**Command-line interface (CLI):** A text-based user interface that uses commands to interact with the computer

**Data exfiltration:** Unauthorised transmission of data from a system

**Data packet:** A basic unit of information that travels from one device to another within a network

**Indicators of compromise (IoC):** Observable evidence that suggests signs of a potential security incident

**Internet Protocol (IP):** A set of standards used for routing and addressing data packets as they travel between devices on a network

**Intrusion detection systems (IDS):** An application that monitors system activity and alerts on possible intrusions

**Media Access Control (MAC) Address:** A unique alphanumeric identifier that is assigned to each physical device on a network

**National Institute of Standards and Technology (NIST) Incident Response Lifecycle:** A framework for incident response consisting of four phases: Preparation; Detection and Analysis; Containment, Eradication and Recovery; and Post-incident activity

**Network data:** The data that's transmitted between devices on a network

**Network protocol analyser (packet sniffer):** A tool designed to capture and analyse data traffic within a network

**Network traffic:** The amount of data that moves across a network

**Network Interface Card (NIC):** Hardware that connects computers to a network

**Packet capture (p-cap):** A file containing data packets intercepted from an interface or network

**Packet sniffing:** The practice of capturing and inspecting data packets across a network

**Playbook:** A manual that provides details about any operational action

**Root user (or superuser):** A user with elevated privileges to modify the system

**Sudo:** A command that temporarily grants elevated permissions to specific users

**tcpdump:** A command-line network protocol analyser

**Wireshark:** An open-source network protocol analyser
