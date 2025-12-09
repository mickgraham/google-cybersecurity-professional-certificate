# Activity: Apply the PASTA threat model framework

*This activity is based on a fictional scenario.*

**References**

* **pasta-worksheet.docx:** PASTA worksheet template
* **pasta-data-flow-diagram.pptx:** Sample data flow diagram
* **pasta-attack-tree.pptx:** Sample attack tree
* **pasta-worksheet-exemplar.docx:** Sample solution

## Scenario

You're part of the growing security team at a company for sneaker enthusiasts and collectors. The business is preparing to launch a mobile app that makes it easy for their customers to buy and sell shoes.

You are performing a threat model of the application using the PASTA framework. You will go through each of the seven stages of the framework to identify security requirements for the new sneaker company app.

## Apply the PASTA threat model framework

### I. Define business and security objectives

* User registration and account management features.
  * Data privacy regulations need to be considered
* Direct messaging between buyers and sellers.
  * Requires real-time back-end processing
* A payment gateway with several payment options.
  * Requires the app to process transactions
  * Legal regulations need to be considered

### II. Define the technical scope

List of technologies used by the application: Application programming interface (**API**), Public key infrastructure (**PKI**), **SHA-256**, **SQL**.

* Using a third-party API reduces development time and complexity by not having to develop one from scratch.
* Using a combination of Public key infrastructure (PKI) and SHA-256 hashing improves security and ensures sensitive personal and payment information is encrypted (e.g. passwords and credit card details).
* SQL allows for sneaker data to be securely stored and accessed. SQL injection prevention measures such as prepared statements and input validation should be used.

### III. Decompose application

Review Sample data flow diagram.

### IV. Threat analysis

List 2 types of threats in the PASTA worksheet that are risks to the information being handled by the application.

* What are the internal threats?
  * Disgruntled, usually former, employees.
* What are the external threats?
  * Malicious hackers.
  * Unexpected power outages or natural disasters.

### V. Vulnerability analysis

List 2 vulnerabilities in the PASTA worksheet that could be exploited.

* **Broken access control:** Issues in the codebase could allow access control checks to be bypassed by modifying the URL, or access controls could be missing for the API.
* **Injection:** SQL injection could occur if the database is not protected against it.
* **Cryptographic failures:** Public Key Infrastructure (PKI) can be compromised when TLS certificates are expired, self-signed, or not properly validated. API failures could occur if communication is not secured using HTTPS or the TLS version used becomes outdated.

### VI. Attack modelling

Review Sample attack tree diagram.

### VII. Risk analysis and impact

List 4 security controls that you've learned about that can reduce risk.

* **Access cards or badges (Physical):** Used to restrict entry into sensitive areas such as server rooms.
* **Firewalls (Technical):** Monitor and filter incoming network traffic to the application.
* **MFA (Technical):** Strong authentication and access controls reduce the risk of unauthorised account access.
* **Separation of duties (Administrative):** Divide access to critical tasks such as; user authentication, payment gateway, direct messaging API.
