 # Incident Report: Network Attack

*This cybersecurity incident report is based on a scenario for a fictional incident.*

**References**

* **incident-report-network-attack.docx:** Incident report template for network attack
* **http-log.xlsx:** Wireshark TCP/HTTP log
* **how-to-read-a-Wireshark-log.docx:** Instructions for reading a Wireshark TCP/HTTP log
* **incident-report-network-attack-exemplar.docx:** Sample solution for the fictional incident

## Network Attack

**Section 1: Identify the type of attack that may have caused this network interruption**

* One potential explanation for the website's connection timeout error message is:
  * The web server takes too long to respond to the message from the requesting browser.
* The logs show that:
  * The web server is receiving an abnormal number of SYN requests coming in at a rapid pace.
* This event could be:
  * A network level denial of service (DoS) attack, called a SYN flood attack, that targets network bandwidth to slow traffic. A SYN flood attack simulates a TCP connection and floods the server with SYN packets. As there is only one IP address attacking the web server, it appears to be a DoS SYN flood attack.

**Section 2: Explain how the attack is causing the website to malfunction**

* When website visitors try to establish a connection with the web server, a three-way handshake occurs using the TCP protocol. Explain the three steps of the handshake:
  1. The [SYN] (synchronize) packet is the initial request from an employee visitor trying to connect to a web page hosted on the web server.
  2. The [SYN, ACK] (synchronize acknowledge) packet is the web server's response to the visitor's request agreeing to the connection. The server will reserve system resources for the final step of the handshake.
  3. The [ACK] (acknowledge) packet is the visitor's machine acknowledging the permission to connect. This is the final step required to make a successful TCP connection.
* Explain what happens when a malicious actor sends a large number of SYN packets all at once:
  * If the number of SYN requests is greater than the server resources available to handle the requests, then the server will become overwhelmed and unable to respond to the requests.
* Explain what the logs indicate and how that affects the server:
  * Initially, the attacker's SYN request is answered normally by the web server. However, the attacker keeps sending more SYN requests, communications to the web server begin to fail, then the web server stops responding.

**Identify the type of attack causing the network interruption**

Reflect on the types of network intrusion attacks that you have learned about in this course so far. As a security analyst, identifying the type of network attack based on the incident is the first step to managing the attack and preventing similar attacks in the future.

* What do you currently understand about network attacks?
  * A network attack is any attempt to disrupt, damage, or gain unauthorised access to a computer network, its devices, or the data flowing through it. These attacks are carried out by malicious actors with the goal of stealing information, interrupting services, or compromising systems.
* Which type of attack would likely result in the symptoms described in the scenario?
  * A DoS SYN flood attack.
* What is the difference between a denial of service (DoS) and distributed denial of service (DDoS)?
  * A DoS attack originates from a single source, a DDoS attack uses multiple devices or servers in different locations.
* Why is the website taking a long time to load and reporting a connection timeout error?
  * The number of SYN requests is greater than the server resources available to handle the requests, so the server becomes overwhelmed and unable to respond to the requests.

### Step 4: Explain how the attack is causing the website to malfunction

Review the Wireshark reading from step 2 and try to identify patterns in the logged network traffic. Analyze the patterns to determine which type of network attack occurred. Write your analysis in section one of the Cybersecurity incident report template provided.

* Describe the attack. What are the main symptoms or characteristics of this specific type of attack?
  * This is a network level denial of service (DoS) attack, called a SYN flood attack, that targets network bandwidth to slow traffic. A SYN flood attack simulates a TCP connection and floods the server with SYN packets.
* Explain how it affected the organization's network. How does this specific network attack affect the website and how it functions?
  * Initially, the attacker's SYN request is answered normally by the web server. However, the attacker keeps sending more SYN requests, communications to the web server begin to fail, then the web server stops responding.
* Describe the potential consequences of this attack and how it negatively affects the organization.
  * The attack will definitely cause service disruption as legitimate users are unable to access the web server resources. It also may cause loss of revenue and damage to reputation.
* _Optional:_ Suggest potential ways to secure the network so this attack can be prevented in the future.
  1. Firewall rules could be updated to detect abnormal spikes in SYN traffic.
  2. Network traffic rate limiting per IP address could be implemented.