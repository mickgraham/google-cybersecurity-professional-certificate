# Module 1: Security Domains

## Overview

* CISSP's eight security domains
* Threats, risks, and vulnerabilities
* Layers of the web

## CISSP's eight security domains

### Domain one: Security and risk management

All organizations must develop their security posture. Security posture is an organization's ability to manage its defense of critical assets and data and react to change. Elements of the security and risk management domain that impact an organization's security posture include:

* Security goals and objectives
* Risk mitigation processes
* Compliance
* Business continuity plans
* Legal regulations
* Professional and organizational ethics

Information security, or InfoSec, is also related to this domain and refers to a set of processes established to secure information. An organization may use playbooks and implement training as a part of their security and risk management program, based on their needs and perceived risk. There are many InfoSec design processes, such as:

* Incident response
* Vulnerability management
* Application security
* Cloud security
* Infrastructure security

As an example, a security team may need to alter how personally identifiable information (PII) is treated in order to adhere to the European Union's General Data Protection Regulation (GDPR).

### Domain two: Asset security

Asset security involves managing the cybersecurity processes of organizational assets, including the storage, maintenance, retention, and destruction of physical and virtual data. Because the loss or theft of assets can expose an organization and increase the level of risk, keeping track of assets and the data they hold is essential. Conducting a security impact analysis, establishing a recovery plan, and managing data exposure will depend on the level of risk associated with each asset. Security analysts may need to store, maintain, and retain data by creating backups to ensure they are able to restore the environment if a security incident places the organization's data at risk.

### Domain three: Security architecture and engineering

This domain focuses on managing data security. Ensuring effective tools, systems, and processes are in place helps protect an organization's assets and data. Security architects and engineers create these processes.

One important aspect of this domain is the concept of shared responsibility. Shared responsibility means all individuals involved take an active role in lowering risk during the design of a security system. Additional design principles related to this domain, which are discussed later in the program, include:

* Threat modeling
* Least privilege
* Defense in depth
* Fail securely
* Separation of duties
* Keep it simple
* Zero trust
* Trust but verify

An example of managing data is the use of a security information and event management (SIEM) tool to monitor for flags related to unusual login or user activity that could indicate a threat actor is attempting to access private data.

### Domain four: Communication and network security

This domain focuses on managing and securing physical networks and wireless communications. This includes on-site, remote, and cloud communications.

Organizations with remote, hybrid, and on-site work environments must ensure data remains secure, but managing external connections to make certain that remote workers are securely accessing an organization's networks is a challenge. Designing network security controls—such as restricted network access—can help protect users and ensure an organization's network remains secure when employees travel or work outside of the main office.

### Domain five: Identity and access management

The identity and access management (IAM) domain focuses on keeping data secure. It does this by ensuring user identities are trusted and authenticated and that access to physical and logical assets is authorized. This helps prevent unauthorized users, while allowing authorized users to perform their tasks.

Essentially, IAM uses what is referred to as the principle of least privilege, which is the concept of granting only the minimal access and authorization required to complete a task. As an example, a cybersecurity analyst might be asked to ensure that customer service representatives can only view the private data of a customer, such as their phone number, while working to resolve the customer's issue; then remove access when the customer's issue is resolved.

### Domain six: Security assessment and testing

The security assessment and testing domain focuses on identifying and mitigating risks, threats, and vulnerabilities. Security assessments help organizations determine whether their internal systems are secure or at risk. Organizations might employ penetration testers, often referred to as “pen testers,” to find vulnerabilities that could be exploited by a threat actor.

This domain suggests that organizations conduct security control testing, as well as collect and analyze data. Additionally, it emphasizes the importance of conducting security audits to monitor for and reduce the probability of a data breach. To contribute to these types of tasks, cybersecurity professionals may be tasked with auditing user permissions to validate that users have the correct levels of access to internal systems.

### Domain seven: Security operations

The security operations domain focuses on the investigation of a potential data breach and the implementation of preventative measures after a security incident has occurred. This includes using strategies, processes, and tools such as:

* Training and awareness
* Reporting and documentation
* Intrusion detection and prevention
* SIEM tools
* Log management
* Incident management
* Playbooks
* Post-breach forensics
* Reflecting on lessons learned

The cybersecurity professionals involved in this domain work as a team to manage, prevent, and investigate threats, risks, and vulnerabilities. These individuals are trained to handle active attacks, such as large amounts of data being accessed from an organization's internal network, outside of normal working hours. Once a threat is identified, the team works diligently to keep private data and information safe from threat actors.

### Domain eight: Software development security

The software development security domain is focused on using secure programming practices and guidelines to create secure applications. Having secure applications helps deliver secure and reliable services, which helps protect organizations and their users.

Security must be incorporated into each element of the software development life cycle, from design and development to testing and release. To achieve security, the software development process must have security in mind at each step. Security cannot be an afterthought.

Performing application security tests can help ensure vulnerabilities are identified and mitigated accordingly. Having a system in place to test the programming conventions, software executables, and security measures embedded in the software is necessary. Having quality assurance and pen tester professionals ensure the software has met security and performance standards is also an essential part of the software development process.

##  Threats, risks, and vulnerabilities

A **threat** is any circumstance or event that can negatively impact assets. One example of a threat is a social engineering attack.

**Risks** are different from threats. A risk is anything that can impact the confidentiality, integrity, or availability of an asset. A risk can be thought of as the likelihood of a threat occurring. An example of a risk to an organization might be the lack of backup protocols for making sure its stored information can be recovered in the event of an accident or security incident.

Organizations tend to rate risks at different levels: low, medium, and high, depending on possible threats and the value of an asset.

* A low-risk asset is information that would not harm the organization's reputation or ongoing operations, and would not cause financial damage if compromised. This includes public information such as website content, or published research data.
* A medium-risk asset might include information that's not available to the public and may cause some damage to the organization's finances, reputation, or ongoing operations. For example, the early release of a company's quarterly earnings could impact the value of their stock.
* A high-risk asset is any information protected by regulations or laws, which if compromised, would have a severe negative impact on an organization's finances, ongoing operations, or reputation. This could include leaked assets with SPII, PII, or intellectual property.

A **vulnerability** is a weakness that can be exploited by a threat. Both a vulnerability and threat must be present for there to be a risk. Examples of vulnerabilities include:

* An outdated firewall, software, or application
* Weak passwords
* Unprotected confidential data

People can also be considered a vulnerability. People's actions can significantly affect an organization's internal network. Whether it's a client, external vendor, or employee, maintaining security must be a united effort.

##  Layers of the web

The web is an interlinked network of online content that's made up of three layers: the **surface web**, the **deep web**, and the **dark web**.

* The **surface web** is the layer that most people use. It contains content that can be accessed using a web browser.
* The **deep web** generally requires authorization to access it. An organization's intranet is an example of the deep web, since it can only be accessed by employees or others who have been granted access.
* Lastly, the **dark web** can only be accessed by using special software. The dark web generally carries a negative connotation since it is the preferred web layer for criminals because of the secrecy that it provides.

## Glossary: Security Domains

**Assess:** The fifth step of the NIST RMF that means to determine if established controls are implemented correctly

**Authorize:** The sixth step of the NIST RMF that refers to being accountable for the security and privacy risks that may exist in an organization

**Business continuity:** An organization's ability to maintain their everyday productivity by establishing risk disaster recovery plans

**Categorize:** The second step of the NIST RMF that is used to develop risk management processes and tasks

**External threat:** Anything outside the organization that has the potential to harm organizational assets

**Implement:** The fourth step of the NIST RMF that means to implement security and privacy plans for an organization

**Internal threat:** A current or former employee, external vendor, or trusted partner who poses a security risk

**Monitor:** The seventh step of the NIST RMF that means be aware of how systems are operating

**Prepare:** The first step of the NIST RMF related to activities that are necessary to manage security and privacy risks before a breach occurs

**Ransomware:** A malicious attack where threat actors encrypt an organization's data and demand payment to restore access

**Risk:** Anything that can impact the confidentiality, integrity, or availability of an asset

**Risk mitigation:** The process of having the right procedures and rules in place to quickly reduce the impact of a risk like a breach

**Security posture:** An organization's ability to manage its defense of critical assets and data and react to change

**Select:** The third step of the NIST RMF that means to choose, customize, and capture documentation of the controls that protect an organization

**Shared responsibility:** The idea that all individuals within an organization take an active role in lowering risk and maintaining both physical and virtual security

**Social engineering: * A manipulation technique that exploits human error to gain private information, access, or valuables

**Vulnerability:** A weakness that can be exploited by a threat
