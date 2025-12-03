# Incident Report: Apply OS Hardening Techniques

*This cybersecurity incident report is based on a scenario for a fictional incident.*

**References**

* **security-incident-report-template.docx:** Incident report template.
* **tcpdump-traffic-log.docx:** tcpdump traffic log.
* **how-to-read-the-tcpdump-traffic-log.docx:** Instructions for reading the tcpdump.
* **security-incident-report-exemplar.docx:** Sample solution.
* **security-incident-report-exemplar-explained.docx** Sample solution explanation.

## Apply OS Hardening Techniques

**Section 1: Identify the network protocol involved in the incident**

The DNS and HTTP protocols were involved in the incident. The malicious file is observed being transported to the users’ computers using the HTTP protocol at the application layer.

**Section 2: Document the incident**

The tcpdump traffic log shows the source computer sending a DNS resolution request for yummyrecipesforme.com, then the HTTP connection request.

The TCP flags [S][S.][.] show log entries indicating an acknowledged connection request. Communication between the source and the intended destination occurs for about 2 minutes.

The TCP flags [P][.] show log entries requesting data from yummyrecipesforme.com with the HTTP: GET method. This could be the download request for the malicious file.

Then, a sudden change happens in the logs. The traffic is routed from the source computer to the DNS server again using a different port to make another DNS resolution request. This time, the DNS server routes the traffic to a new IP address that is associated with greatrecipesforme.com.http. This is probably done by the malicious file.

**Section 3: Recommend one remediation for brute force attacks**

A recommended remediation is to enforce two-factor authentication(2FA). This will require an additional form of verification that the former employee/hacker is unlikely to have.

Requiring stringer passwords, Monitoring login attempts, or limiting the number of login attempts could also minimise the risk of these incidents occurring in the future.
