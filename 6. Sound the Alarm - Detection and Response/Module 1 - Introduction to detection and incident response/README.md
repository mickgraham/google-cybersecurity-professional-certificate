# Module 1: Introduction to Detection and Incident Response

## Overview

* Incident response lifecycle
* Incident handler's journal
* Incident response
* Documentation, detection, and management tools

## Incident Response Lifecycle

Incident lifecycle frameworks provide a structure to support incident response operations. Frameworks help organizations develop a standardised approach to their incident response process, so that incidents are managed in an effective and consistent way.

### National Institute of Standards and Technology's (NIST) Incident Response (IR) Framework

The NIST IR framework for incident response consisting of four phases:

* **Preparation**
* **Detection and Analysis**
* **Containment, Eradication, and Recovery**
* **Post-incident activity**

### The 5 W's of an incident:

* **Who** triggered the incident?
  * Was it an unauthorised user, a malicious actor, or even an accidental action by an employee?
* **What** happened?
  * What kind of attack was it? What systems were affected? What data was compromised?
* **When** did the incident take place?
  * Knowing the timeline helps in understanding the sequence of events.
* **Where** did the incident take place?
  *  Which specific systems, networks, or locations were involved?
* **Why** did the incident occur?
  * What was the motive? What vulnerabilities were exploited?

## Incident Handler's Journal

An **Incident handler's journal** is a structured record used by cybersecurity professionals to document security incidents from detection through resolution. It helps ensure accurate tracking, analysis, and reporting of incidents using the incident response lifecycle.

## Incident Response

A **computer security incident response team (CSIRT)** is a specialised group of security professionals that are trained in incident management and response. Their goals include efficiently managing incidents, providing recovery resources, and preventing future occurrences. For incident response to be effective and efficient, there must be clear command, control, and communication of the situation to achieve the desired goal:

* **Command** refers to having the appropriate leadership and direction to oversee the response.
* **Control** refers to the ability to manage technical aspects during incident response, like coordinating resources and assigning tasks.
* **Communication** refers to the ability to keep stakeholders informed.

**Roles** within CSIRTs:

* **Security Analyst:** Monitors for threats, analyses alerts, performs root-cause investigations, and escalates critical threats.
* **Technical Lead:** Manages technical aspects of incident response, determines root causes, and implements containment, eradication, and recovery strategies.
* **Incident Coordinator:** Coordinates with various departments to ensure open communication and awareness of incident status.

**Incident response plans** are crucial for organizations to respond to security incidents quickly and consistently, especially given potential regulatory reporting requirements.
These plans are customised to an organization's unique needs, considering factors like mission, size, culture, industry, and structure. Key Elements of an incident response plan are:

* **Incident response procedures:** These provide step-by-step instructions for handling various incidents.
* **System information:** This includes vital data such as network diagrams, data flow diagrams, logging details, and asset inventory.
* **Supporting documents:** Contact lists, forms, and templates are also integral parts of the plan.

## Documentation, Detection, and Management Tools

Documentation encompasses any recorded content—audio, digital, handwritten, or video—serving a specific purpose, with organizations often setting their own standards due to the lack of a universal industry standard. Common types include **playbooks**, **incident handler's journals**, **policies**, **plans**, and **final reports**, all designed to provide instruction and guidance.

Intrusion Detection Systems (IDS), Intrusion Prevention Systems (IPS), and Endpoint Detection and Response (EDR) are all detection tools used in cybersecurity.

* **Intrusion Detection Systems (IDS):** An IDS monitors system activity and alerts on potential intrusions without actively stopping them.
* **Intrusion Prevention Systems (IPS):** An IPS monitors for intrusive activity and takes action to stop it, similar to an IDS but with the added capability of prevention.
* **Endpoint Detection and Response (EDR):** Unlike IDS or IPS, EDR uses behavioural analysis, often powered by machine learning and AI, to identify threat patterns and can automatically stop attacks.

| Capability                    | IDS | IPS | EDR |
|-------------------------------|-----|-----|-----|
| Detects malicious activity    | ✓   | ✓   | ✓  |
| Prevents intrusions           | N/A | ✓   | ✓   |
| Logs activity                 | ✓   | ✓   | ✓  |
| Generates alerts              | ✓   | ✓   | ✓  |
| Performs behavioural analysis | N/A | N/A | ✓   |

**Security Information and Event Management (SIEM)** tools collect and analyze log data from various sources like IDS, IPS, databases, and firewalls to provide a high-level overview of network activity. They aggregate this data into a centralised platform, making it easier for security professionals to monitor and identify potential threats.

* **Collection and Aggregation:** SIEM tools gather massive amounts of log data from different sources and centralise it in one place.
* **Normalisation:** Raw data is cleaned by removing non-essential attributes and creating consistency in log records, which is crucial for incident investigation.
* **Analysis:** Normalised data is analysed against a predefined rule set to detect security incidents, which are then categorised and reported as alerts.

While SIEM tools focus on collecting, analysing, and reporting security events for human review, **Security Orchestration, Automation, and Response (SOAR)** tools automate the analysis and response to security incidents. SOAR can also track and manage multiple incidents as a single case, offering a centralised view of all related events.

## Glossary: Introduction to Detection and Incident Response

**Computer security incident response teams (CSIRT):** A specialised group of security professionals that are trained in incident management and response

**Documentation:** Any form of recorded content that is used for a specific purpose

**Endpoint detection and response (EDR):** An application that monitors an endpoint for malicious activity

**Event:** An observable occurrence on a network, system, or device

**False negative:** A state where the presence of a threat is not detected

**False positive:** An alert that incorrectly detects the presence of a threat

**Incident:** An occurrence that actually or imminently jeopardises, without lawful authority, the confidentiality, integrity, or availability of information or an information system; or constitutes a violation or imminent threat of violation of law, security policies, security procedures, or acceptable use policies

**Incident handler's journal:** A form of documentation used in incident response

**Incident response plan:** A document that outlines the procedures to take in each step of incident response

**Intrusion detection system (IDS):** An application that monitors system activity and alerts on possible intrusions

**Intrusion prevention system (IPS):** An application that monitors system activity for intrusive activity and takes action to stop the activity

**National Institute of Standards and Technology (NIST) Incident Response Lifecycle:** A framework for incident response consisting of four phases: Preparation; Detection and Analysis; Containment, Eradication, and Recovery; and Post-incident activity

**Playbook:** A manual that provides details about any operational action

**Security information and event management (SIEM):** An application that collects and analyses log data to monitor critical activities in an organization

**Security operations center (SOC):** An organizational unit dedicated to monitoring networks, systems, and devices for security threats or attacks

**Security orchestration, automation, and response (SOAR):** A collection of applications, tools, and workflows that uses automation to respond to security events

**True negative:** A state where there is no detection of malicious activity

**True positive:** An alert that correctly detects the presence of an attack