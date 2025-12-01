# Module 2: Security Frameworks and Controls

## Overview

* Security Frameworks: Guidelines used for building plans to mitigate risks and threats to data and privacy, supporting compliance with laws and regulations.
* Security Controls: Safeguards designed to reduce specific security risks, including physical, technical, and administrative measures.
* Design principles
* Security audits

## International Organization for Standardization/International Electrotechnical Commission (ISO/IEC) 27001

An internationally recognized and used framework is ISO/IEC 27001. The ISO 27000 family of standards enables organizations of all sectors and sizes to manage the security of assets, such as financial information, intellectual property, employee data, and information entrusted to third parties. This framework outlines requirements for an information security management system, best practices, and controls that support an organization's ability to manage risks. Although the ISO/IEC 27001 framework does not require the use of specific controls, it does provide a collection of controls that organizations can use to improve their security posture.

## Controls

Controls are used alongside frameworks to reduce the possibility and impact of a security threat, risk, or vulnerability. Controls can be physical, technical, and administrative and are typically used to prevent, detect, or correct security issues.

Examples of physical controls:

* Gates, fences, and locks
* Security guards
* Closed-circuit television (CCTV), surveillance cameras, and motion detectors
* Access cards or badges to enter office spaces

Examples of technical controls:

* Firewalls
* MFA
* Antivirus software

Examples of administrative controls:

* Separation of duties
* Authorization
* Asset classification

## The CIA Triad

The CIA triad is a model that helps inform how organizations consider risk when setting up systems and security policies. It is made up of three elements that cybersecurity analysts and organizations work toward upholding: **confidentiality**, **integrity**, and **availability**. Maintaining an acceptable level of risk and ensuring systems and policies are designed with these elements in mind helps establish a successful security posture, which refers to an organization's ability to manage its defense of critical assets and data and react to change.

### Confidentiality

Confidentiality is the idea that only authorized users can access specific assets or data. In an organization, confidentiality can be enhanced through the implementation of design principles, such as the principle of least privilege. The principle of least privilege limits users access to only the information they need to complete work-related tasks. Limiting access is one way of maintaining the confidentiality and security of private data.

### Integrity

Integrity is the idea that the data is verifiably correct, authentic, and reliable. Having protocols in place to verify the authenticity of data is essential. One way to verify data integrity is through cryptography, which is used to transform data so unauthorized parties cannot read or tamper with it (NIST, 2022). Another example of how an organization might implement integrity is by enabling encryption, which is the process of converting data from a readable format to an encoded format. Encryption can be used to prevent access and ensure data, such as messages on an organization's internal chat platform, cannot be tampered with.

### Availability

Availability is the idea that data is accessible to those who are authorized to use it. When a system adheres to both availability and confidentiality principles, data can be used when needed. In the workplace, this could mean that the organization allows remote employees to access its internal network to perform their jobs. It's worth noting that access to data on the internal network is still limited, depending on what type of access employees need to do their jobs. If, for example, an employee works in the organization's accounting department, they might need access to corporate accounts but not data related to ongoing development projects.

## National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF)

* **Identify:** The management of cybersecurity risk and its effect on an organisation's people and assets.
* **Protect:** The strategy used to protect an organisation through the implementaiton of policies, procedures, training, and tools that help mitigate cybersecurity threats.
* **Detect:** Identifying potential security incidents and improving monitoring capabilities to increase the speed and efficiency of detections.
* **Respond:** Making sure that the proper procedures are used to contain, neutralise, and analyse security incidents, and implement improvements to the security process.
* **React:** The process of returning affected systems back to normal operation.
* **Govern:** A significant update in the latest version of the NIST Cybersecurity Framework is the inclusion of a new core function: **Govern**. This function emphasizes the importance of strong cybersecurity governance across all levels of the organization. It's about establishing and maintaining the structures and processes needed to effectively manage cybersecurity risk. This includes things like setting clear cybersecurity objectives, ensuring leadership commitment, developing and implementing a comprehensive risk management strategy, and continuously improving cybersecurity performance.

## OWASP Security Principles

The Open Web Application Security Project, recently renamed Open Worldwide Application Security Project® (OWASP), security principles help keep data safe and reduce risk for an organization.

* **Minimize attack surface area:** Attack surface refers to all the potential vulnerabilities a threat actor could exploit.
* **Principle of least privilege:** Users have the least amount of access required to perform their everyday tasks.
* **Defense in depth:** Organizations should have varying security controls that mitigate risks and threats.
* **Separation of duties:** Critical actions should rely on multiple people, each of whom follow the principle of least privilege.
* **Keep security simple:** Avoid unnecessarily complicated solutions. Complexity makes security difficult.
* **Fix security issues correctly:** When security incidents occur, identify the root cause, contain the impact, identify vulnerabilities, and conduct tests to ensure that remediation is successful.
* **Establish secure defaults:** The optimal security state of an application is also its default state for users; it should take extra work to make the application insecure.
* **Fail securely:** When a control fails or stops, it should do so by defaulting to its most secure option.
* **Don't trust services:** Many organizations work with third-party partners. These outside partners often have different security policies than the organization does. And the organization shouldn't explicitly trust that their partners systems are secure.
* **Avoid security by obscurity:** The security of key systems should not rely on keeping details hidden.

## Security Audit

A security audit is a review of an organization's security controls, policies, and procedures against a set of expectations. Audits are independent reviews that evaluate whether an organization is meeting internal and external criteria. Internal criteria include outlined policies, procedures, and best practices. External criteria include regulatory compliance, laws, and federal regulations.

### Audit checklist

It's necessary to create an audit checklist before conducting an audit. A checklist is generally made up of the following areas of focus:

#### Identify the scope of the audit

* The audit should:
  * List assets that will be assessed (e.g., firewalls are configured correctly, PII is secure, physical assets are locked, etc.)
  * Note how the audit will help the organization achieve its desired goals
  * Indicate how often an audit should be performed
  * Include an evaluation of organizational policies, protocols, and procedures to make sure they are working as intended and being implemented by employees

#### Complete a risk assessment

* A risk assessment is used to evaluate identified organizational risks related to budget, controls, internal processes, and external standards (i.e., regulations).

#### Conduct the audit

* When conducting an internal audit, you will assess the security of the identified assets listed in the audit scope.

#### Create a mitigation plan

* A mitigation plan is a strategy established to lower the level of risk and potential costs, penalties, or other issues that can negatively affect the organization's security posture.

#### Communicate results to stakeholders

* The end result of this process is providing a detailed report of findings, suggested improvements needed to lower the organization's level of risk, and compliance regulations and standards the organization needs to adhere to.

## Glossary: Security Frameworks and Controls

**Asset:** An item perceived as having value to an organization

**Attack vectors:** The pathways attackers use to penetrate security defenses

**Authentication:** The process of verifying who someone is

**Authorization:** The concept of granting access to specific resources in a system

**Availability:** The idea that data is accessible to those who are authorized to access it

**Biometrics:** The unique physical characteristics that can be used to verify a person's identity

**Confidentiality:** The idea that only authorized users can access specific assets or data

**Confidentiality, integrity, availability (CIA) triad:** A model that helps inform how organizations consider risk when setting up systems and security policies

**Detect:** A NIST core function related to identifying potential security incidents and improving monitoring capabilities to increase the speed and efficiency of detections

**Encryption:** The process of converting data from a readable format to an encoded format

**Govern:** A NIST core function related to ensuring an organization establishes, oversees, and improves its cybersecurity strategy, policies, roles, and risk management processes to align with business goals and regulations

**Identify:** A NIST core function related to management of cybersecurity risk and its effect on an organization's people and assets

**Integrity:** The idea that the data is correct, authentic, and reliable

**National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF):** A voluntary framework that consists of standards, guidelines, and best practices to manage cybersecurity risk

**National Institute of Standards and Technology (NIST) Special Publication (S.P.) 800-53:** A unified framework for protecting the security of information systems within the U.S. federal government

**Open Web Application Security Project/Open Worldwide Application Security Project (OWASP):** A non-profit organization focused on improving software security

**Protect:** A NIST core function used to protect an organization through the implementation of policies, procedures, training, and tools that help mitigate cybersecurity threats

**Recover:** A NIST core function related to returning affected systems back to normal operation

**Respond:** A NIST core function related to making sure that the proper procedures are used to contain, neutralize, and analyze security incidents, and implement improvements to the security process

**Risk:** Anything that can impact the confidentiality, integrity, or availability of an asset

**Security audit:** A review of an organization's security controls, policies, and procedures against a set of expectations

**Security controls:** Safeguards designed to reduce specific security risks

**Security frameworks:** Guidelines used for building plans to help mitigate risk and threats to data and privacy

**Security posture:** An organization's ability to manage its defense of critical assets and data and react to change

**Threat:** Any circumstance or event that can negatively impact assets
