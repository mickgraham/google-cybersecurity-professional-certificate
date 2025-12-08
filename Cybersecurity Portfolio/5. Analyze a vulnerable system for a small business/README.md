# Portfolio Activity: Analyze a vulnerable system for a small business

*This activity is based on a fictional scenario.*

**References**

* **vulnerability-assessment-report-template.docx:** Vulnerability Assessment Report
* **NIST-SP-800-30-Rev-1.docx**: NIST SP 800-30 Rev. 1
* **vulnerability-assessment-report-exemplar.docx:** Sample solution

## Scenario

You are a newly hired cybersecurity analyst for an e-commerce company. The company stores information on a remote database server, since many of the employees work remotely from locations all around the world. Employees of the company regularly query, or request, data from the server to find potential customers. The database has been open to the public since the company's launch three years ago. As a cybersecurity professional, you recognize that keeping the database server open to the public is a serious vulnerability.

You are tasked with completing a vulnerability assessment of the situation to communicate the potential risks to decision makers at the company. You must create a written report that explains how the vulnerable server is a risk to business operations and how it can be secured.

## Vulnerability Assessment Report

### System Description

The server hardware consists of a powerful CPU processor and 128GB of memory. It runs on the latest version of Linux operating system and hosts a MySQL database management system. It is configured with a stable network connection using IPv4 addresses and interacts with other servers on the network. Security measures include SSL/TLS encrypted connections.

### Scope

The scope of this vulnerability assessment relates to the current access controls of the system. The assessment will cover a period of three months, from June 2025 to August 2025. NIST SP 800-30 Rev. 1 is used to guide the risk analysis of the information system.

### Purpose

* How is the database server valuable to the business?
  * There is only a single database server that stores all of the data for the company. It is used by employees and public users.
* Why is it important for the business to secure the data on the server?
  * The company relies on the server and does not have any backup services in place.
* How might the server impact the business if it were disabled?
  * The impact could be severe. Employees would not be able to use the server to find customers. The public users would not be able to use the system. Loss of revenue and reputation would occur.

### Risk Assessment

| Threat source      | Threat event                                  | Likelihood | Severity | Risk |
|--------------------|-----------------------------------------------|------------|----------|------|
| E.g. Competitor    | Obtain sensitive information via exfiltration | 1          | 3        | 3    |
| Malicious software | Conduct "man-in-the-middle" attacks           | 2          | 3        | 3    |
| Power outages      | Disrupt mission-critical operations           | 2          | 2        | 4    |

### Approach

The likelihood of a threat occurrence and the impact of these potential events were weighed against the risks to day-to-day operational needs. Risks to day-to-day operational needs lists power outages as the highest risk score of 4.

### Remediation Strategy

* Implementation of authentication, authorization, and auditing mechanisms to ensure that only authorized users access the database server. This includes using strong passwords, role-based access controls, and multi-factor authentication to limit user privileges.
* Encryption of data in motion using TLS instead of SSL.
* IP allow-listing to corporate offices to prevent random users from the internet from connecting to the database.
* Enforce certificate validation using server certificates signed by a Certificate Authority (CA) trust chain.
* Use Uninterruptible Power Supplies (UPS) to provide a temporary battery backup during power loss.
* Use offsite or could-based redundancy to eliminate single point of failure from local power sources.
