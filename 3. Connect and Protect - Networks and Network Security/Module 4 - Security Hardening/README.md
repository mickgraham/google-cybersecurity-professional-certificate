# Module 4: Security Hardening

* Security hardening
* OS hardening
* Brute force attacks
* Network hardening practices
* Cloud network hardening

## Security Hardening

Security hardening is the process of strengthening a system to reduce its vulnerability and attack surface. All the potential vulnerabilities that a threat actor could exploit are referred to as a system's attack surface.

Using an example that compares a network to a house; The attack surface would be all the doors and windows that a robber could use to gain access to that house. Just like putting locks on all the doors and windows in the house, security hardening involves minimising the attack surface or potential vulnerabilities and keeping a network as secure as possible.

Where security hardening occurs:

* Devices
* Networks
* Applications
* Cloud infrastructure

Security analysts responsibilities include:

* Patch updates
* Backups

Another important strategy for security hardening is to conduct regular penetration testing. A penetration test, also called a pen test, is a simulated attack that helps identify vulnerabilities in a system, network, website, application, and process.

## OS Hardening

Operating system (OS) hardening is crucial for maintaining network security by securing the interface between computer hardware and the user.

### Importance of OS Hardening

* An insecure OS can compromise an entire network, making it essential to secure each system.
* While there are many types of operating systems, they generally share similar security hardening practices.

### Regular OS Hardening Tasks

* **Patch Updates:** A patch update is a software and operating system, or OS, update that addresses security vulnerabilities. Promptly applying patches is critical as malicious actors can exploit known vulnerabilities in outdated systems.
* **Hardware and Software Disposal:** This ensures that all old hardware is properly wiped and disposed of. It's also a good idea to delete any unused software applications to make sure that there aren't any unnecessary vulnerabilities connected with the programs that the software uses.

### One-Time OS Hardening Tasks

* **Baseline Configuration:** A documented set of specifications within a system that is used as a basis for future builds, releases, and updates. This allows for comparison if unusual activity is suspected.
* **Strong Password Policies:** Strong password policies require that passwords follow specific rules. For example, an organization may set a password policy that requires a minimum of eight characters, a capital letter, a number, and a symbol.

Some systems also require **multi-factor authentication (MFA)**. MFA is a security measure which requires a user to verify their identity in two or more ways to access a system or network.

## Brute force attacks

Brute force attacks are a trial-and-error process of guessing passwords. Attacks can be launched manually or through software tools. Methods include simple brute force attacks and dictionary attacks. To protect against brute force attacks, cybersecurity analysts can use sandboxes to test suspicious files, check for vulnerabilities, or to simulate real attacks and virtual machines to conduct vulnerability tests. Some common measures to prevent brute force attacks include: hashing and salting, MFA and/or 2FA, CAPTCHA and reCAPTCHA, and password policies.

* **Simple brute force attacks**: Attackers try to guess a user's login credentials by entering any combination of usernames and passwords that they can think of until they find the one that works.
* **Dictionary attacks**: Attackers use a list of commonly used passwords and stolen credentials from previous breaches to access a system.

Using brute force to access a system can be a tedious and time consuming process, especially when it's done manually. There are a range of tools attackers use to conduct their attacks.

### Assessing vulnerabilities

Before a brute force attack or other cybersecurity incident occurs, companies can run a series of tests on their network or web applications to assess vulnerabilities. Virtual machines and sandboxes can be used to test suspicious files, check for vulnerabilities before an event occurs, or to simulate a cybersecurity incident.

* **Virtual machines (VMs)**: VMs provide an additional layer of security for an organization because they can be used to run code in an isolated environment, preventing malicious code from affecting the rest of the computer or system. However, There is still a small risk that a malicious program can escape virtualization and access the host machine.
* **Sandbox environments**: Commonly used for testing patches, identifying and addressing bugs, or detecting cybersecurity vulnerabilities. Sandboxes can also be used to evaluate suspicious software, evaluate files containing malicious code, and simulate attack scenarios.

Note that some malware authors know how to write code to detect if the malware is executed in a VM or sandbox environment. Attackers can program their malware to behave as harmless software when run inside these types of  testing environments.

### Prevention measures

Some common measures organizations use to prevent brute force attacks and similar attacks from occurring include:

* **Salting and hashing:** Hashing converts information into a unique value that can then be used to determine its integrity. It is a one-way function, meaning it is impossible to decrypt and obtain the original text. Salting adds random characters to hashed passwords. This increases the length and complexity of hash values, making them more secure.
* **Multi-factor authentication (MFA) and two-factor authentication (2FA):** MFA is a security measure which requires a user to verify their identity in two or more ways to access a system or network. 2FA is similar to MFA, except it uses only two forms of verification.
* **CAPTCHA and reCAPTCHA:** CAPTCHA stands for Completely Automated Public Turing test to tell Computers and Humans Apart. It asks users to complete a simple test that proves they are human. This helps prevent software from trying to brute force a password. reCAPTCHA is a free CAPTCHA service from Google that helps protect websites from bots and malicious software.
* **Password policies:** Organizations use password policies to standardise good password practices throughout the business. Policies can include guidelines on how complex a password should be, how often users need to update passwords, whether passwords can be reused or not, and if there are limits to how many times a user can attempt to log in before their account is suspended.

## Network Hardening Practices

Network hardening focuses on network-related security hardening, like port filtering, network access privileges, and encryption over networks. Certain network hardening tasks are performed regularly, while others are performed once and then updated as needed.

### Regular Network Hardening Tasks

* **Firewall Rules and Log Analysis:** Regularly maintain firewall rules and analyze network logs using tools like SIEMs (Security Information and Event Management) to identify and prioritise security events.
* **Patch Updates and Server Backups:** Consistently apply patch updates and perform server backups to ensure system integrity and data recovery.

### One-Time Network Hardening Tasks

* **Port Filtering and Wireless Protocols:** Implement port filtering on firewalls to block unnecessary ports and disable older, less secure wireless protocols.
* **Network Segmentation and Encryption:** Segment networks to isolate departments and sensitive data, and encrypt all network communication using the latest standards, especially for restricted zones.

### Network Security Applications

| Devices / Tools | Advantages | Disadvantages |
|-----------------|------------|---------------|
| Firewall | A firewall allows or blocks traffic based on a set of rules. | A firewall is only able to filter packets based on information provided in the header of the packets. |
| Intrusion Detection System (IDS) | An IDS detects and alerts admins about possible intrusions, attacks, and other malicious traffic. | An IDS can only scan for known attacks or obvious anomalies; new or sophisticated attacks might not be caught. It doesn't stop incoming traffic. |
| Intrusion Prevention System (IPS) | An IPS monitors system activity for intrusions and anomalies and takes action to stop them. | An IPS is an inline appliance - if it fails, the connection between the private network and the internet breaks. It may detect false positives and block legitimate traffic. |
| Security Information and Event Management (SIEM) | A SIEM tool collects and analyses log data from multiple machines and aggregates events in one dashboard. | A SIEM tool only reports on potential security issues and does not take actions to stop or prevent suspicious events. |

## Cloud Network Hardening

A cloud network is a collection of servers or computers that stores resources and data in a remote data center that can be accessed via the internet. They can host company data and applications using cloud computing to provide on-demand storage, processing power, and data analytics. Just like regular web servers, cloud servers also require proper maintenance done through various security hardening procedures. Although cloud servers are hosted by a **cloud service provider (CSP)**, these providers cannot prevent intrusions in the cloud - especially intrusions from malicious actors, both internal and external to an organization.

One distinction between cloud network hardening and traditional network hardening is the use of a server baseline image for all server instances stored in the cloud.
This allows data in the cloud servers to be compared to a baseline image to make sure there haven't been any unverified changes.

There are various techniques and tools that can be used to secure cloud network infrastructure and resources. Some common cloud security hardening techniques include:

* **Identity and Access Management (IAM):** Manages digital identities and authorises user access to various cloud resources.
* **Hypervisors:** Abstract hardware from the operating software environment, with Type One hypervisors commonly used by Cloud Service Providers (CSPs) to manage virtualization components and ensure resource availability.
* **Baselining:** Involves configuring and setting up the cloud environment as a fixed reference point to compare and track changes.
* **Examples of Baselining:** Includes restricting admin portal access, enabling password management, file encryption, and threat detection services for databases.
* **Encryption:** Scrambles information into unreadable ciphertext, relying on secure keys rather than algorithm secrecy for data integrity and confidentiality.
* **Cryptographic Erasure (Crypto-shredding):** A method of data destruction in the cloud where encryption keys are permanently destroyed, rendering the encrypted data undecipherable.

### Shared responsibility model

A commonly accepted cloud security principle is the shared responsibility model. The shared responsibility model states that the CSP must take responsibility for security involving the cloud infrastructure, including physical data centers, hypervisors, and host operating systems. The company using the cloud service is responsible for the assets and processes that they store or operate in the cloud.

The shared responsibility model ensures that both the CSP and the users agree about where their responsibility for security begins and ends. A problem occurs when organizations assume that the CSP is taking care of security that they have not taken responsibility for. One example of this is cloud applications and configurations. The CSP takes responsibility for securing the cloud, but it is the organization's responsibility to ensure that services are configured properly according to the security requirements of their organization.

### Key Management

Modern encryption relies on keeping the encryption keys secure. Below are the measures you can take to further protect your data when using cloud applications:

* **Trusted platform module (TPM):** TPM is a computer chip that can securely store passwords, certificates, and encryption keys.
* **Cloud hardware security module (CloudHSM):** CloudHSM is a computing device that provides secure storage for cryptographic keys and processes cryptographic operations, such as encryption and decryption.

## Glossary: Security Hardening

**Baseline configuration (baseline image):** A documented set of specifications within a system that is used as a basis for future builds, releases, and updates

**Hardware:** The physical components of a computer

**Multi-factor authentication (MFA):** A security measure which requires a user to verify their identity in two or more ways to access a system or network

**Network log analysis:** The process of examining network logs to identify events of interest

**Operating system (OS):** The interface between computer hardware and the user

**Patch update:** A software and operating system update that addresses security vulnerabilities within a program or product

**Penetration testing (pen test):** A simulated attack that helps identify vulnerabilities in systems, networks, websites, applications, and processes

**Security hardening:** The process of strengthening a system to reduce its vulnerabilities and attack surface

**Security information and event management (SIEM):** An application that collects and analyses log data to monitor critical activities for an organization

**World-writable file:** A file that can be altered by anyone in the world
