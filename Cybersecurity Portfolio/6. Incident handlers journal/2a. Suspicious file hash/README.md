# Activity: Investigate a suspicious file hash

*This activity is based on a fictional scenario.*

**References**

* **pyramid-of-pain.pptx:** Pyramid of pain template
* **investigation-findings.pptx:** Sample solution

## Scenario

You are a level one security operations center (SOC) analyst at a financial services company. You have received an alert about a suspicious file being downloaded on an employee's computer.

You investigate this alert and discover that the employee received an email containing an attachment. The attachment was a password-protected spreadsheet file. The spreadsheet's password was provided in the email. The employee downloaded the file, then entered the password to open the file. When the employee opened the file, a malicious payload was then executed on their computer.

You retrieve the malicious file and create a SHA256 hash of the file. You might recall from a previous course that a hash function is an algorithm that produces a code that can't be decrypted. Hashing is a cryptographic method used to uniquely identify malware, acting as the file's unique fingerprint.

Now that you have the file hash, you will use VirusTotal to uncover additional IoCs that are associated with the file.

## Investigate a suspicious file hash

The file hash appears to be malicious.

* It has been flagged as malicious by 59/72 security vendors.
* It has a community score of -276.
* Analysis by security vendors indicates it is a trojan threat category (trojan.flagpro).

Identify **three indicators of compromise (IoCs)** that are associated with this file hash using the tabs in the VirusTotal report.

1. **Hash values:**
  * MD5: 287d612e29b71c90aa54947313810a25
  * SHA-1: 8f35a9e70dbec8f1904991773f394cd4f9a07f5e
  * SHA-256 (provided): 54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b
2. **Domain names:**
  * a.sinkhole.yourtrap.com
  * org.misecure.com
3. **Tools:**
  * Checks user input