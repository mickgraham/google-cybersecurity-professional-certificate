# Activity: Use a playbook to respond to a phishing incident

*This activity is based on a fictional scenario.*

**References**

* **alert-ticket.docx:** Alert ticket
* **phishing-incident-response-playbook.docx:** Phishing playbook (with flowchart)
* **completed-alert-ticket.docx:** Sample solution

## Scenario

You are a level-one security operations center (SOC) analyst at a financial services company. Previously, you received a phishing alert about a suspicious file being downloaded on an employee's computer. After investigating the email attachment file's hash, the attachment has already been verified malicious. Now that you have this information, you must follow your organization's process to complete your investigation and resolve the alert.

Your organization's security policies and procedures describe how to respond to specific alerts, including what to do when you receive a phishing alert.

In the playbook, there is a flowchart and written instructions to help you complete your investigation and resolve the alert. At the end of your investigation, you will update the alert ticket with your findings about the incident.

## Use a playbook to respond to a phishing incident

### Evaluate the alert

**Ticket ID:** A-2703
**Alert Message:** SERVER-MAIL Phishing attempt possible download of malware
**Severity:** Medium
**Details:** The user may have opened a malicious email and opened attachments or clicked links.
**Ticket status:** Escalated

### Determine whether the alert should be escalated

* Does the email contain any links or attachments?
  * Yes (bfsvc.exe)
* Are the links or attachments malicious?
  * Yes (VirusTotal analysis)

**Resolution:** Update the alert ticket and escalate.
