# Activity: Identify the attack vectors of a USB drive

*This activity is based on a fictional scenario.*

**References**

* **parking-lot-usb-exercise.docx:** Parking lot USB exercise template
* **parking-lot-usb-exercise-exemplar.docx:** Sample solution

## Scenario

You are part of the security team at Rhetorical Hospital and arrive to work one morning. On the ground of the parking lot, you find a USB stick with the hospital's logo printed on it. There's no one else around who might have dropped it, so you decide to pick it up out of curiosity.

You bring the USB drive back to your office where the team has virtualization software installed on a workstation. Virtualization software can be used for this very purpose because it's one of the only ways to safely investigate an unfamiliar USB stick. The software works by running a simulated instance of the computer on the same workstation. This simulation isn't connected to other files or networks, so the USB drive can't affect other systems if it happens to be infected with malicious software.

## Identify the attack vectors of a USB drive

### Contents

* Are there files that can contain PII?
  * Yes
* Are there sensitive work files?
  * Yes
* Is it safe to store personal files with work files?
  * No

The contents of the USB drive contain files that appear to belong to a specific person. It contains a mixture of personal and business-related information that should not be stored in the same place.

### Attacker mindset

* Could the information be used against other employees?
  * Yes
* Could the information be used against relatives?
  * Yes
* Could the information provide access to the business?
  * Not directly, however a malicious actor could perform a social engineering attack using information in the the shift schedules or new hire letter.

Any information that an attacker obtains can be used against someone. Information on a USB drive should be encrypted regardless of whether it's personal or work-related.

### Risk analysis

* What types of malicious software could be hidden on these devices? What could have happened if the device were infected and discovered by another employee?
  * Spyware or ransomware would be the most likely types of malware. A hacker could gain access to sensitive data or perform a ransomware attack.
* What sensitive information could a threat actor find on a device like this?
  * Data that comes under HIPAA regulations could be found on a device like this.
* How might that information be used against an individual or an organization?
  * A social engineering attack could be used to impersonate employees to gain access into the system.

It's unsafe to plug an unfamiliar USB drive into your computer because of the wide range of attacks that can be hidden on them. Promoting employee awareness of USB baiting attacks is a managerial control that can reduce the risks of a negative event. Routinely scanning for viruses is an example of an operational control that can be implemented. And disabling Autoplay on all PCs is a technical precaution that can be taken.
