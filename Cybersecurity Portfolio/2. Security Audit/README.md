# Security Audit

*This security audit is based on a scenario for a fictional company using the information provided in Security-audit-botium-toys.docx*

**References**

* **Security-audit-control-categories.docx:** Defines security audit controls.
* **Security-audit-controls-and-compliance-checklist.docx:** Provides a template for conducting a security audit.
* **Security-audit-exemplar.docx:** Sample solution for Botium Toys.
* **Security-audit-sample.docx:** Sample internal security audit.

## Scenario

Botium Toys is a small U.S. business that develops and sells toys. The business has a single physical location, which serves as their main office, a storefront, and warehouse for their products. However, Botium Toy's online presence has grown, attracting customers in the U.S. and abroad. As a result, their information technology (IT) department is under increasing pressure to support their online market worldwide.

The manager of the IT department has decided that an internal IT audit needs to be conducted. She's worried about maintaining compliance and business operations as the company grows without a clear plan. She believes an internal audit can help better secure the company's infrastructure and help them identify and mitigate potential risks, threats, or vulnerabilities to critical assets. The manager is also interested in ensuring that they comply with regulations related to internally processing and accepting online payments and conducting business in the European Union (E.U.).

The IT manager starts by implementing the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF), establishing an audit scope and goals, listing assets currently managed by the IT department, and completing a risk assessment. The goal of the audit is to provide an overview of the risks and/or fines that the company might experience due to the current state of their security posture.

Your task is to review the IT manager's scope, goals, and risk assessment report. Then, perform an internal audit by completing a controls and compliance checklist.

## Controls Checklist

Select "yes" (✅) or "no" (❌) to answer the question: *Does Botium Toys currently have this control in place?*

### Controls assessment checklist

| Yes | No  | Control                                                             |
| --- | --- | :------------------------------------------------------------------ |
|     | ❌ | Least Privilege                                                     |
|     | ❌ | Disaster recovery plans                                             |
| ✅ |     | Password policies                                                   |
|     | ❌ | Separation of duties                                                |
| ✅ |     | Firewall                                                            |
|     | ❌ | Intrusion detection system (IDS)                                    |
|     | ❌ | Backups                                                             |
| ✅ |     | Antivirus software                                                  |
| ✅ |     | Manual monitoring, maintenance, and intervention for legacy systems |
|     | ❌ | Encryption                                                          |
|     | ❌ | Password management system                                          |
| ✅ |     | Locks (offices, storefront, warehouse)                              |
| ✅ |     | Closed-circuit television (CCTV) surveillance                       |
| ✅ |     | Fire detection/prevention (fire alarm, sprinkler system, etc.)      |

---

### Compliance Checklist

Select "yes" (✅) or "no" (❌) to answer the question: *Does Botium Toys currently adhere to this compliance best practice?*

#### Payment Card Industry Data Security Standard (PCI DSS)

| Yes | No  | Best practice                                                                                                |
| --- | --- | :----------------------------------------------------------------------------------------------------------- |
|     | ❌ | Only authorized users have access to customers' credit card information.                                     |
|     | ❌ | Credit card information is stored, accepted, processed, and transmitted internally, in a secure environment. |
|     | ❌ | Implement data encryption procedures to better secure credit card transaction touchpoints and data.          |
|     | ❌ | Adopt secure password management policies.                                                                   |

#### General Data Protection Regulation (GDPR)

| Yes | No  | Best practice                                                                                                     |
| --- | --- | :---------------------------------------------------------------------------------------------------------------- |
| ✅ |     | E.U. customers' data is kept private/secured.                                                                     |
| ✅ |     | There is a plan in place to notify E.U. customers within 72 hours if their data is compromised/there is a breach. |
|     | ❌ | Ensure data is properly classified and inventoried.                                                               |
| ✅ |     | Enforce privacy policies, procedures, and processes to properly document and maintain data.                       |

#### System and Organizations Controls (SOC type 1, SOC type 2)

| Yes | No  | Best practice                                                                              |
| --- | --- | :----------------------------------------------------------------------------------------- |
|     | ❌ | User access policies are established.                                                      |
|     | ❌ | Sensitive data (PII/SPII) is confidential/private.                                         |
| ✅ |     | Data integrity ensures the data is consistent, complete, accurate, and has been validated. |
| ✅ |     | Data is available to individuals authorized to access it.                                  |

---

## Recommendations (optional):

This section provides recommendations, related to controls and/or compliance needs, that your IT manager could communicate to stakeholders to reduce risks to assets and improve Botium Toys' security posture.

### Controls

* Access controls pertaining to least privilege should be implemented.
* A disaster recovery plan should be put in place.
* Access controls pertaining to separation of duties should be implemented.
* The IT department dshould install an intrusion detection system (IDS).
* Critical data should be backed up.
* Encryption should be used to ensure confidentiality of customers credit card information.
* A centralized password management system that enforces the password policy's minimum requirements should be used.

### Compliance

* User access policies should be implemented to ensure Only authorized users have access to customers credit card information.
* Encryption should be used to ensure confidentiality of customers credit card information.
* Ensure secure password management policies are adopted.
* Ensure data is properly classified and inventoried.
