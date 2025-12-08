# Module 2: Network Operations

## Overview

* **Network protocols:** Set of rules used by two or more devices on a network to describe the order of delivery and the structure of the data.
* **Virtual private networks (VPNs):**
* **Firewalls, security zones, and proxy servers:**

## Network Protocols

A network protocol is a set of rules used by two or more devices on a network to describe the order of delivery and the structure of data. Network protocols can be divided into three main categories: communication protocols, management protocols, and security protocols.

### Communication protocols

Communication protocols govern the exchange of information in network transmission. They dictate how the data is transmitted between devices and the timing of the communication. They also include methods to recover data lost in transit. Here are a few of them:

* **Transmission Control Protocol (TCP):** TCP uses a three-way handshake process. First, the device sends a synchronize (SYN) request to a server. Then the server responds with a SYN/ACK packet to acknowledge receipt of the device's request. Once the server receives the final ACK packet from the device, a TCP connection is established.
* **User Datagram Protocol (UDP):** Connectionless protocol that does not establish a connection between devices before a transmission. This makes it less reliable than TCP. But it also means that it works well for transmissions that need to get to their destination quickly.
* **Hypertext Transfer Protocol (HTTP):** Provides a method of communication between clients and website servers. HTTP is considered insecure, so it is being replaced on most websites by a secure version, called HTTPS that uses encryption from SSL/TLS for communication. However, there are still many websites that use the insecure HTTP protocol.
* **Domain Name System (DNS):** Translates internet domain names into IP addresses.

### Management Protocols

The next category of network protocols is management protocols. Management protocols are used for monitoring and managing activity on a network. They include protocols for error reporting and optimizing performance on the network.

* **Simple Network Management Protocol (SNMP):** Network protocol used for monitoring and managing devices on a network. SNMP can reset a password on a network device or change its baseline configuration.
* **Internet Control Message Protocol (ICMP):** Internet protocol used by devices to tell each other about data transmission errors across the network. ICMP is commonly used as a quick way to troubleshoot network connectivity and latency by issuing the "ping" command.

### Security Protocols

Security protocols are network protocols that ensure that data is sent and received securely across a network. Security protocols use encryption algorithms to protect data in transit. Below are some common security protocols:

* **Hypertext Transfer Protocol Secure (HTTPS):** HTTPS is a secure version of HTTP that uses secure sockets layer/transport layer security (SSL/TLS) encryption on all transmissions so that malicious actors cannot read the information contained.
* **Secure File Transfer Protocol (SFTP):** Secure protocol used to transfer files from one device to another over a network.

| Protocol | Port |
|----------|------|
| TCP | None (transport protocol) |
| UDP | None (transport protocol) |
| HTTP | TCP port 80 |
| DNS | UDP/TCP port 53 |
| SNMP | UDP port 161 |
| ICMP | None (network protocol) |
| HTTPS | TCP port 443 |
| SFTP | TCP port 22 |

### Additional Network Protocols

* **Dynamic Host Configuration Protocol (DHCP):** Used on a network to configure devices. It works with the router to assign a unique IP address to each device and provide the addresses of the appropriate DNS server and default gateway for each device.
* **Address Resolution Protocol (ARP):** Mainly a network access layer protocol in the TCP/IP model used to translate the IP addresses that are found in data packets into the MAC address of the hardware device.
* **Telnet:** Used to connect with a remote system. Telnet sends all information in clear text. It uses command line prompts to control another device similar to secure shell (SSH), but Telnet is not as secure as SSH.
* **Secure shell protocol (SSH):** Provides secure authentication and encrypted communication.
* **Post office protocol (POP):** Used to manage and retrieve email from a mail server. User devices will send requests to the remote mail server and download email messages locally. It does not guarantee that a user can sync the same email across multiple devices.
* **Internet Message Access Protocol (IMAP):** Used for incoming email. It downloads the headers of emails and the message content. The content also remains on the email server, which allows users to access their email from multiple devices.
* **Simple Mail Transfer Protocol (SMTP):** Used to transmit and route email from the sender to the recipients address. SMTP helps to filter out spam by regulating how many emails a source can send at a time.

| Protocol | Port |
|----------|------|
| DHCP | UDP port 67 (servers), UDP port 68 (clients) |
| ARP | none |
| Telnet | TCP port 23 |
| SSH | TCP port 22 |
| POP3 | TCP/UDP port 110 (unencrypted), TCP/UDP port 995 (encrypted, SSL/TLS) |
| IMAP | TCP port 143 (unencrypted), TCP port 993 (encrypted, SSL/TLS) |
| SMTP | TCP/UDP port 25 (unencrypted) |
| SMTPS | TCP/UDP port 587 (encrypted, TLS) |

ARP does not have a specific port number since it is a layer 2 protocol and port numbers are associated with the layer 7 application layer.

### Wireless Protocols

Wi-Fi refers to a set of standards that define communication for wireless LANs. They are based on the 802.11 family of internet communication standards determined by the Institute of Electrical and Electronics Engineers (IEEE).

* **Wired Equivalent Privacy (WEP):** A wireless security protocol developed in 1999. It is the oldest of the wireless security standards, but is largely out of use today.
* **Wi-Fi Protected Access (WPA):** Developed in 2003 to improve upon WEP. WPA was always intended to be a transitional measure so backwards compatibility could be established with older hardware.
* **WPA2:** The second version of WPA was released in 2004. WPA2 uses the Advanced Encryption Standard (AES), improves upon WPAs use of TKIP, and uses the Counter Mode Cipher Block Chain Message Authentication Code Protocol (CCMP). It is considered the security standard for all Wi-Fi transmissions today.
* **WPA3:** The third version of WPA is growing in usage as more WPA3 compatible devices are released. These are the key differences between WPA2 and WPA3:
  * WPA3 addresses the authentication handshake vulnerability to KRACK attacks, which is present in WPA2.
  * WPA3 uses Simultaneous Authentication of Equals (SAE), a password-authenticated, cipher-key-sharing agreement.
  * WPA3 has increased encryption to make passwords more secure by using 128-bit or 192-bit encryption.

## Virtual Private Networks (VPNs)

A virtual private network (VPN) is a network security service that modifies the public IP address and conceals the virtual location of a device to maintain data privacy when operating on public networks such as the internet.

A VPN encrypts data in transit and uses encapsulation to protect information as it travels across the internet. It creates an encrypted tunnel between a device and the VPN server, preventing unauthorized access. This ensures that data, IP addresses, and virtual locations remain hidden from malicious actors.

## Firewalls, Security Zones, and Proxy Servers

**Firewalls** are network security devices that monitor and control traffic based on defined rules, using techniques such as port filtering. They can be hardware, software, or cloud-based, and may operate as stateful (tracking traffic behavior) or stateless (following predefined rules). Next-generation firewalls (NGFWs) provide advanced features like deep packet inspection and intrusion protection, often integrating with cloud threat intelligence. Firewalls are essential for enforcing network security and protecting both internal and cloud-based resources.

**Security zones** segment a network to protect internal resources from external threats. Security zones act as a barrier to internal networks, maintain privacy within corporate groups, and prevent issues from spreading to the whole network. On the outer layer of controlled networks is the demilitarized zone (DMZ). The DMZ acts as a network perimeter to the internal network, which stores private data, and a restricted zone safeguards highly confidential information. Firewalls separate these zones, controlling access and preventing threats from spreading. Security zones are essential for maintaining privacy, isolating issues, and enforcing network security.

**Subnetting** is a common security strategy used by organizations. Subnetting allows organizations to create smaller networks within their private network. This improves the efficiency of the network and can be used to create security zones. CIDR allows a network to be segmented into smaller chunks by assigning subnet masks to IP addresses to create a subnet.

**Proxy servers** act as intermediaries between clients and the internet, forwarding requests while hiding the internal network's IP addresses to enhance security. They can filter traffic, block unsafe websites, and store frequently requested data to reduce exposure to internal servers. Types include forward proxies (control outgoing traffic), reverse proxies (protect internal servers), and email proxies (filter spam and phishing attempts). Proxy servers provide an additional layer of network protection by monitoring and regulating both incoming and outgoing traffic.

## Glossary: Network Operations

**Address Resolution Protocol (ARP):** A network protocol used to determine the MAC address of the next router or device on the path

**Cloud-based firewalls:** Software firewalls that are hosted by the cloud service provider

**Controlled zone:** A subnet that protects the internal network from the uncontrolled zone

**Domain Name System (DNS):** A networking protocol that translates internet domain names into IP addresses

**Encapsulation:** A process performed by a VPN service that protects your data by wrapping sensitive data in other data packets

**Firewall:** A network security device that monitors traffic to or from your network

**Forward proxy server:** A server that regulates and restricts a person's access to the internet

**Hypertext Transfer Protocol (HTTP):** An application layer protocol that provides a method of communication between clients and website servers

**Hypertext Transfer Protocol Secure (HTTPS):** A network protocol that provides a secure method of communication between clients and servers

**IEEE 802.11 (Wi-Fi):** A set of standards that define communication for wireless LANs

**Network protocols:** A set of rules used by two or more devices on a network to describe the order of delivery of data and the structure of data

**Network segmentation:** A security technique that divides the network into segments

**Port filtering:** A firewall function that blocks or allows certain port numbers to limit unwanted communication

**Proxy server:** A server that fulfills the requests of its clients by forwarding them to other servers

**Reverse proxy server:** A server that regulates and restricts the internet's access to an internal server

**Secure File Transfer Protocol (SFTP):** A secure protocol used to transfer files from one device to another over a network

**Secure shell (SSH):** A security protocol used to create a shell with a remote system

**Security zone:** A segment of a company's network that protects the internal network from the internet

**Simple Network Management Protocol (SNMP):** A network protocol used for monitoring and managing devices on a network

**Stateful:** A class of firewall that keeps track of information passing through it and proactively filters out threats

**Stateless:** A class of firewall that operates based on predefined rules and does not keep track of information from data packets

**Subnetting:** The subdivision of a network into logical groups called subnets

**Transmission Control Protocol (TCP):** An internet communication protocol that allows two devices to form a connection and stream data

**Uncontrolled zone:** The portion of the network outside the organization

**Virtual private network (VPN):** A network security service that changes your public IP address and masks your virtual location so that you can keep your data private when you are using a public network like the internet

**Wi-Fi Protected Access (WPA):** A wireless security protocol for devices to connect to the internet
