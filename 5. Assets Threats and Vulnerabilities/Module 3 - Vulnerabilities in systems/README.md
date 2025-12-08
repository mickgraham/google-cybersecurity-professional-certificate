# Module 3: Vulnerabilities in Systems

## Overview

* Vulnerability management process
* Defence in depth model
* The CVE list
* The OWASP top 10
* Attack surfaces
* Common attack vectors

## Vulnerability Management Process

Vulnerability management is the process of finding and patching vulnerabilities. It helps keep assets safe and is a method of stopping threats before they can become a problem. Vulnerability management is a four step process:

1. Identify vulnerabilities
2. Consider potential exploits of those vulnerabilities
3. Prepare defences against threats.
4. Evaluate those defences.

When the last step ends, the process starts again. Vulnerability management happens in a cycle. It's a regular part of what security teams do because there are always new vulnerabilities to be concerned about.

### Common CI/CD Pipeline Vulnerabilities

Continuous Integration, Continuous Delivery, and Continuous Deployment (CI/CD) pipelines are essential for modern software development. Here are some common vulnerabilities to be aware of:

* **Insecure Dependencies: Risks from Third-Party Code:** CI/CD pipelines often use many third-party libraries and components. If these components have known vulnerabilities (Common Vulnerabilities and Exposures, or CVEs), those vulnerabilities can be unknowingly added to your application during the automated build process.
  * **Action Step:** Regularly scan and update your dependencies. Make sure you're using secure versions of all external components.
* **Misconfigured Permissions: Controlling Access:** Weak access controls in CI/CD tools, code repositories, and related systems are a significant vulnerability. Unauthorised access can allow attackers to modify code, pipeline configurations, or inject malicious content.
  * **Action Step:** Implement strong access management using Role-Based Access Control (RBAC). Ensure only authorized individuals can access and change critical pipeline elements.
* **Lack of Automated Security Testing: Missing Critical Checks:** Failing to include automated security testing in your CI/CD pipeline is a serious error. Without tools like SAST and DAST, you are almost guaranteed to release software full of vulnerabilities that will go undetected until after it's live, leading to significantly higher costs and effort to fix..
  * **Action Step:** Integrate automated security testing (SAST and DAST) into your CI/CD pipeline. This should be a core part of your secure CI/CD strategy.
* **Exposed Secrets: Protecting Sensitive Information**
Hardcoding sensitive data like API keys, passwords, and tokens directly into code or pipeline settings is a serious security mistake. If exposed, these secrets can lead to major security breaches.
  * **Action Step:** Never hardcode secrets. Use secure vaults or dedicated secrets management tools to store and manage sensitive information. Enforce this practice across your team.
* **Unsecured Build Environments: Protecting the Pipeline Infrastructure**
The CI/CD environment itself (the servers and systems that run your pipeline) needs to be secure. If this environment is vulnerable, attackers can compromise it to alter builds, inject malicious code, or steal sensitive data.
  * **Action Step:** Harden your build environments. Use secure containers or virtual machines to minimise the risk of a compromised pipeline.

## Defence in Depth Model

Defence in depth is a layered approach to vulnerability management that minimises risk by having multiple barriers. Defence in depth is commonly referred to as the castle approach because it resembles the layered defences of a castle. Each layer presents different challenges to attackers, ensuring that if one defence fails, another is in place to stop the attack.

* **Perimeter Layer:** This initial layer focuses on user authentication, like usernames and passwords, to filter external access and only allow trusted partners to proceed.
* **Network Layer:** This layer deals with authorization and includes technologies such as network firewalls.
* **Endpoint Layer:** This layer protects devices like laptops, desktops, and servers that access the network, often using antivirus software.
* **Application Layer:** Security measures are programmed directly into applications, with multi-factor authentication being a common example.
* **Data Layer:** This final layer protects critical data, such as personally identifiable information, and utilises security controls like asset classification.

Weaknesses and flaws are generally found during a vulnerability assessment, which is the internal review process of an organization's security systems. These assessments work similar to the process of identifying and categorising vulnerabilities on the CVE list. The primary goal is to pinpoint weak points, prevent attacks, and ensure compliance with regulatory standards. Vulnerability assessment is a four step process:

1. **Identification:** This initial step involves using scanning tools and manual testing to discover vulnerabilities, aiming to capture a snapshot of the security system's current state.
2. **Vulnerability Analysis:** Following identification, each discovered vulnerability is thoroughly tested to determine the root cause of the problem.
3. **Risk Assessment:** Vulnerabilities are assigned a severity score based on the potential impact of exploitation and the likelihood of it occurring, which helps prioritise remediation efforts.
4. **Remediation:** The final step involves addressing critical vulnerabilities through actions like enforcing new security procedures, updating operating systems, or implementing system patches, often in collaboration with IT teams.

### Vulnerability Scanning

A vulnerability scanner is software, designed to be non-intrusive, that automatically compares known vulnerabilities against the technologies on a network. These tools scan systems to find misconfigurations or programming flaws across various layers, including perimeter, network, endpoint, application, and data layers.

* **External vs. Internal:** External scans test outward-facing systems like websites, while internal scans examine an organization's internal systems.
* **Authenticated vs. Unauthenticated:** Authenticated scans use real user accounts to check for vulnerabilities, whereas unauthenticated scans simulate external threat actors without system access.
* **Limited vs. Comprehensive:** Limited scans focus on specific devices, while comprehensive scans analyze all devices connected to a network.

Vulnerability scans vary depending on the surfaces that an organization is evaluating.

## The CVE List

A vulnerability is a weakness within a system, such as a software flaw. An exposure is a mistake that can be exploited by a threat, like leaving a sensitive document in an unsecured location.

* The **Common Vulnerabilities and Exposures (CVE) list** is a public dictionary of known vulnerabilities and exposures, created by the MITRE Corporation in 1999.
* It provides a standardised way to identify and categorise these issues, helping organizations improve their security defences.

The main purpose of the CVE list is to offer a standard way of identifying and categorising known vulnerabilities and exposures. Most CVEs in the list are reported by independent researchers, technology vendors, and ethical hackers, but anyone can report one.

* Reported vulnerabilities undergo a strict review by a **CVE Numbering Authority (CNA)** to ensure they meet specific criteria before being assigned a CVE ID.
* The **NIST National Vulnerabilities Database** uses the **Common Vulnerability Scoring System (CVSS)** to score the severity of vulnerabilities, helping security teams prioritise patching efforts.

## The OWASP Top 10

OWASP is a nonprofit foundation that works to improve the security of software. It is an open platform that security professionals from around the world use to share information, tools, and events that are focused on securing the web. One of OWASP's most valuable resources is the OWASP Top 10. The organization has published this list since 2003 as a way to spread awareness of the web's most targeted vulnerabilities.

* The OWASP Top 10 is updated every few years as technologies evolve. Rankings are based on how often the vulnerabilities are discovered and the level of risk they present.
* Auditors also use the OWASP Top 10 as one point of reference when checking for regulatory compliance.

## Attack Surfaces

An attack surface is all the potential vulnerabilities that a threat actor could exploit. Analysing the attack surface is usually the first thing security teams do.

* The **physical attack surface** involves people and their devices, and can be attacked from both inside and outside an organization. Security hardening, which involves strengthening a system to reduce vulnerabilities and limit entry points, is essential for the physical attack surface.
* The **digital attack surface** includes everything beyond an organization's firewall, such as cloud-stored data and online connections. The shift to cloud computing has expanded the digital attack surface, making it more challenging to harden and defend against threats from various entry points.

### Being Prepared for Anything

Having a plan should things go wrong is important. But how do you figure out what to plan for? In this field, teams often conduct simulations of things that can go wrong as part of their vulnerability management strategy. One way this is done is by applying an attacker mindset to the weaknesses they discover. Applying an attacker mindset is a lot like conducting an experiment. It's about causing problems in a controlled environment and evaluating the outcome to gain insights.

One method of applying an attacker mindset is using attack simulations:

* **Proactive simulations** assume the role of an attacker by exploiting vulnerabilities and breaking through defences. This is sometimes called a red team exercise.
* **Reactive simulations** assume the role of a defender responding to an attack. This is sometimes called a blue team exercise.

### Threat Actors

A threat actor is any person or group who presents a security risk. This broad definition refers to people inside and outside an organization. It also includes individuals who intentionally pose a threat, and those that accidentally put assets at risk. Threat actors are normally divided into five categories based on their motivations:

* **Competitors** refers to rival companies who pose a threat because they might benefit from leaked information.
* **State actors** are government intelligence agencies.
* **Criminal syndicates** refer to organised groups of people who make money from criminal activity.
* **Insider threats** can be any individual who has or had authorized access to an organization's resources. This includes employees who accidentally compromise assets or individuals who purposefully put them at risk for their own benefit.
* **Shadow IT** refers to individuals who use technologies that lack IT governance. A common example is when an employee uses their personal email to send work-related communications.

An **advanced persistent threat (APT)** refers to instances when a threat actor maintains unauthorised access to a system for an extended period of time. The term is mostly associated with nation states and state-sponsored actors. Typically, an APT is concerned with surveilling a target to gather information. They then use the intel to manipulate government, defence, financial, and telecom services.

Each threat actor has a unique motivation for targeting an organization's assets. Keeping them out takes more than knowing their intentions and capabilities. It's also important to recognize the types of attack vectors they'll use. For the most part, threat actors gain access through one of these attack vector categories:

* **Direct access**, referring to instances when they have physical access to a system
* **Removable media**, which includes portable hardware, like USB flash drives
* **Social media platforms** that are used for communication and content sharing
* **Email**, including both personal and business accounts
* **Wireless networks** on premises
* **Cloud services** usually provided by third-party organizations
* **Supply chains** like third-party vendors that can present a backdoor into systems

## Common Attack Vectors

Attack vectors are the pathways attackers use to penetrate security defences, similar to doors and windows of a home. Examples include social media and removable media like USB drives. Attack vectors are exploited by malicious hackers to steal information, but also unintentionally by employees (e.g., sharing sensitive company news on social media) or intentionally by disgruntled employees.

Security professionals should think like attackers to identify and stop threats. This involves a step-by-step process:

1. **Identify a target:** This could be specific information, a system, a person, a group, or the organization itself.
2. **Determine access:** Figure out what information an attacker might use to reach the target.
3. **Evaluate attack vectors:** Identify exploitable pathways to gain entry.
4. **Find tools and methods:** Determine what attackers would use to carry out the attack.

Key strategies for defending against attack vectors include:

* **Educating users:** Inform them about security vulnerabilities, such as new phishing exploits.
* **Applying the principle of least privilege:** Limit access rights to only what is necessary for a task.
* **Using the right security controls and tools:** Implement antivirus software and other tools to reduce human error.
* **Building a diverse security team:** A variety of perspectives enhances the team's ability to anticipate and prevent attacks.

## Glossary: Vulnerabilities in Systems

**Advanced persistent threat (APT):** An instance when a threat actor maintains unauthorised access to a system for an extended period of time

**Attack surface:** All the potential vulnerabilities that a threat actor could exploit

**Attack tree:** A diagram that maps threats to assets

**Attack vector:** The pathways attackers use to penetrate security defences

**Bug bounty:** Programs that encourage freelance hackers to find and report vulnerabilities

**Common Vulnerabilities and Exposures (CVE®) list:** An openly accessible dictionary of known vulnerabilities and exposures

**Common Vulnerability Scoring System (CVSS):** A measurement system that scores the severity of a vulnerability

**CVE Numbering Authority (CNA):** An organization that volunteers to analyze and distribute information on eligible CVEs

**Defence in depth:** A layered approach to vulnerability management that reduces risk

**Exploit:** A way of taking advantage of a vulnerability

**Exposure:** A mistake that can be exploited by a threat

**Hacker:** Any person who uses computers to gain access to computer systems, networks, or data

**MITRE:** A collection of non-profit research and development centers

**Security hardening:** The process of strengthening a system to reduce its vulnerability and attack surface

**Threat actor:** Any person or group who presents a security risk

**Vulnerability:** A weakness that can be exploited by a threat

**Vulnerability assessment:** The internal review process of a company’s security systems

**Vulnerability management:** The process of finding and patching vulnerabilities

**Vulnerability scanner:** Software that automatically compares existing common vulnerabilities and exposures against the technologies on the network

**Zero-day:** An exploit that was previously unknown
