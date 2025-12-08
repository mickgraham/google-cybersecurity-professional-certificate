 # Cybersecurity Incident Report

*This cybersecurity incident report is based on a scenario for a fictional incident.*

**References**

* **cybersecurity-incident-report-network-traffic-analysis.docx:**: Incident report template for network traffic analysis
* **cybersecurity-incident-report-example.docx:**: Incident report example for network analysis
* **cybersecurity-incident-report-exemplar.docx:**: Sample solution for the fictional incident
* **cybersecurity-incident-report-exemplar-explained.docx:** Sample solution for the fictional incident with explanation

## Network Traffic Analysis

**Part 1: Provide a summary of the problem found in the DNS and ICMP traffic log.**

* The UDP protocol reveals that:
  * The UDP message requesting an IP address for the domain "www.yummyrecipesforme.com" did not go through to the DNS server because no service was listening on the receiving DNS port.
* This is based on the results of the network analysis, which show that the ICMP echo reply returned the error message:
  * "udp port 53 unreachable".
* The port noted in the error message is used for:
  * Port 53 is a port for DNS service.
* The most likely issue is:
  * A problem with the Domain Name System (DNS) server, which is preventing domain name resolution.

**Part 2: Explain your analysis of the data and provide at least one cause of the incident.**

* Time incident occurred:
  * 1:24 PM to 1:28 PM.
* Explain how the IT team became aware of the incident:
  * Several customers of clients reported that they were not able to access the client company website "www.yummyrecipesforme.com", and saw the error "destination port unreachable" after waiting for the page to load.
* Explain the actions taken by the IT department to investigate the incident:
  * To start, the IT department attempted to visit the website and also receive the error "destination port unreachable". To troubleshoot the issue, the IT department then used a network analyser tool, tcpdump, and attempt to load the webpage again to analyse the packet traffic.
* Note key findings of the IT department's investigation (i.e., details related to the port affected, DNS server, etc.):
  * The UDP message requesting an IP address for the domain "www.yummyrecipesforme.com" did not go through to the DNS server because no service was listening on the receiving DNS port.
* Note a likely cause of the incident:
  * It could be caused by the DNS server being down, a firewall blocking traffic to the server, or a denial-of-service (DoS) attack.

## Incident Report Summary

### Part 1: Provide a summary of the problem found in the DNS and ICMP traffic log**

The network analysis shows that a UDP message requesting the IP address for "www.yummyrecipesforme.com" failed to reach the DNS server because no service was listening on the required DNS port. This is confirmed by the ICMP echo reply, which reported the error "udp port 53 unreachable".

Since port 53 is used for DNS services, the findings indicate a likely issue with the DNS server that is preventing proper domain name resolution.

### Part 2: Explain your analysis of the data and provide at least one cause of the incident

The incident occurred between 1:24 PM and 1:28 PM. The IT team became aware of the issue after several customers reported being unable to access the client website, "www.yummyrecipesforme.com", and receiving the error message "destination port unreachable" after waiting for the page to load.

To investigate, the IT department first attempted to visit the website themselves and confirmed the same error. They then used the network analysis tool tcpdump while attempting to load the webpage again, allowing them to examine the packet traffic and identify the source of the problem.

The investigation revealed that the UDP message requesting the IP address for the domain did not reach the DNS server because no service was listening on the receiving DNS port. Based on these findings, a likely cause of the incident is that the DNS server may have been down, traffic to the server may have been blocked by a firewall, or a denial-of-service (DoS) attack may have disrupted normal DNS operations.
