# Activity: Identify the attack vectors of a USB drive

*This activity is based on a fictional scenario.*

## Activity Overview

In this activity, you will assess the attack vectors of a USB drive. You will consider a scenario of finding a USB drive in a parking lot from both the perspective of an attacker and a target.

USBs, or flash drives, are commonly used for storing and transporting data. However, some characteristics of these small, convenient devices can also introduce security risks. Threat actors frequently use USBs to deliver malicious software, damage other hardware, or even take control of devices. USB baiting is an attack in which a threat actor strategically leaves a malware USB stick for an employee to find and install to unknowingly infect a network. It relies on curious people to plug in an unfamiliar flash drive that they find.

## Step-By-Step Instructions

### Step 1: Access the template

* [Parking lot USB exercise template](./parking-lot-usb-exercise.docx) (parking-lot-usb-exercise.docx)

### Step 2: Inspect the contents of the USB stick

You create a virtual environment and plug the USB drive into the workstation. The contents of the device appear to belong to Jorge Bailey, the human resource manager at Rhetorical Hospital.

Jorge's drive contains a mix of personal and work-related files. For example, it contains folders that appear to store family and pet photos. There is also a new hire letter and an employee shift schedule.

Review the types of information that Jorge has stored on this device. Then, in the **Contents** row of the activity template, write **2-3 sentences** (40-60 words) about the type of information that's stored on the USB drive.

_**Note:** USB drives often contain an assortment of personally identifiable information (PII). Attackers can easily use this sensitive information to target the data owner or others around them._

### Step 3: Apply an attacker mindset to the contents of the USB drive

The flash drive appears to contain a mixture of personal and work-related files. Consider how an attacker might use this information if they obtained it. Also, consider whether this whole event was staged.

For example, an attacker could have placed these files on the USB drive as a distraction. They might have targeted Jorge or someone he knows, hoping they would find the device and plug it into their workstation. In doing so, the attacker could establish a backdoor into the company's systems while the unsuspecting target browsed through the files.

In the **Attacker mindset** row of the activity template, write **2-3 sentences** (40-60 words) about how this information could be used against Jorge or the hospital.

### Step 4: Analyse the risks of finding a parking lot USB

You have _not_ opened any of the files on the device, which is best practice.

Attackers sometimes conduct USB baiting attacks to deliver malicious code that they've crafted.

However, this USB drive was still a security risk even though it did not contain malicious code. It could have easily been found by an attacker who might have used its contents to plan a variety of attacks.

Consider some of the risks associated with USB baiting attacks:

* What types of malicious software could be hidden on these devices? What could have happened if the device were infected and discovered by another employee?
* What sensitive information could a threat actor find on a device like this?
* How might that information be used against an individual or an organization?

In the **Risk analysis** row of the activity template, write **3 or 4 sentences** (60-80 words) describing any technical, operational, or managerial controls that could mitigate USB baiting attacks.
