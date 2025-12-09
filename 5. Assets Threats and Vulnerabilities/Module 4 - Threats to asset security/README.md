# Module 4: Threats to Asset Security

## Overview

* Social engineering
* Malware
* Web-based exploits
* Threat modelling process

## Social Engineering

Social engineering is a tactic that relies on manipulating individuals rather than sophisticated programming skills to bypass security measures. These attacks can occur online, in person, or through other interactions, often leading to data breaches, malware infections, or unauthorised system access.

Stages of a social engineering attack:

* **Preparation:** Attackers gather information about their target to identify the most effective exploitation methods.
* **Pretexting and Persuasion:** Attackers establish trust by disguising themselves and using gathered information to manipulate targets into revealing sensitive information.
* **Disconnection:** After obtaining the desired information, attackers break communication to cover their tracks.

Common types of social engineering to watch out for:

* **Baiting** is a social engineering tactic that tempts people into compromising their security. A common example is USB baiting that relies on someone finding an infected USB drive and plugging it into their device.
* **Quid pro quo** is a type of baiting used to trick someone into believing that they'll be rewarded in return for sharing access, information, or money.
* **Tailgating** is a social engineering tactic in which unauthorised people follow an authorized person into a restricted area.
* **Watering hole** is a type of attack when a threat actor compromises a website frequently visited by a specific group of users.
* **Phishing** is the use of digital communications to trick people into revealing sensitive data or deploying malicious software.
  * **Phishing kit tools** include malicious attachments, fake data collection forms, fraudulent web links

## Malware

Malware, short for malicious software, is designed to harm devices or networks and can spread through infected USB drives or online connections. Devices connected to the internet are particularly vulnerable, and malware interferes with normal operations, allowing attackers to control systems without user knowledge.

* **Virus:** Malicious code written to interfere with computer operations and cause damage to data and software. This type of malware must be installed by the target user before it can spread itself and cause damage.
* **Worm:** Malware that can duplicate and spread itself across systems on its own. Worms were very popular attacks in the mid 2000s but are less frequently used in recent years.
* **Trojan:** Also called a Trojan horse, is malware that is similar to a virus except that it looks like a legitimate file or program.
* **Adware:** Advertising-supported software, or adware, is a type of legitimate software that is sometimes used to display digital advertisements in applications. Malicious adware falls into a sub-category of malware known as a potentially unwanted application (PUA).
* **Spyware:** Malware that's used to gather and sell information without consent. It's also considered a PUA. PUAs like spyware have become a serious challenge in the open-source software development ecosystem because developers tend to overlook how their software could be misused or abused by others.
* **Scareware:** Another type of PUA that employs tactics to frighten users into infecting their own device by displaying fake warnings that appear to come from legitimate companies.
* **Fileless malware:** Resides in memory where the malware never touches the hard drive. This is unlike the other types of malware, which are stored within a file on disk. Instead, these stealthy infections get into the operating system or hide within trusted applications.
* **Rootkits:** Malware that provides remote, administrative access to a computer. Most attackers use rootkits to open a backdoor to systems, allowing them to install other forms of malware or to conduct network security attack that is often spread by a combination of two components: a dropper and a loader.
* **Botnet:** Short for "robot network", is a collection of computers infected by malware that are under the control of a single threat actor, known as the "bot-herder".
* **Ransomware** Describes a malicious attack where threat actors encrypt an organization's data and demand payment to restore access. According to the Cybersecurity and Infrastructure Security Agency (CISA), ransomware crimes are on the rise and becoming increasingly sophisticated. Ransomware infections can cause significant damage to an organization and its customers.
 * **Cryptojacking** is a recent form of malware that installs software to illegally mine cryptocurrencies.

## Web-Based Exploits

Web-based exploits leverage coding flaws in web applications to gain sensitive information, often targeting the high level of interaction in web apps. These attacks can give cybercriminals access to sensitive information like session cookies, geolocation, webcams, and microphones.

* **Injection attacks** involve inserting malicious code into vulnerable applications, which then runs in the background without the user's knowledge.
* **Cross-Site Scripting (XSS)** is a common and dangerous type of injection attack that inserts malicious code into vulnerable websites or web applications, often exploiting HTML and JavaScript.
* **SQL injection** happens when websites fail to sanitise user input, allowing attackers to insert malicious SQL code into input fields like login forms.

Types of XSS Attacks include:

* **Reflected XSS:** A malicious script is sent to the server and activated in the server's response, often through a malicious link that appears to be from a trusted site.
* **Stored XSS:** Malicious script is directly injected onto the server, often targeting elements like images or buttons, and activates when a user simply visits the infected site.
* **DOM-based XSS:** Malicious script exists within the web page's source code (Document Object Model) and can be seen in the URL, activating without needing to be sent to the server.

### Injection Prevention

A key to preventing SQL injection attacks is to escape user inputs - preventing someone from inserting any code that a program isn't expecting. There are several ways to escape user inputs:

* **Prepared statements:** a coding technique that executes SQL statements before passing them on to a database
* **Input sanitisation:** programming that removes user input which could be interpreted as code.
* **Input validation:** programming that ensures user input meets a system's expectations.

## Threat Modelling Process

Threat modelling is a crucial process in cybersecurity for anticipating and preparing for attacks.

1. **Define the scope** of the model by inventorying and classifying assets.
2. **Identify threats**, categorising them as internal (e.g., employees) or external (e.g., malicious hackers),
3. **Characterise the environment** by creating an attack tree flow chart to map threats to assets.
4. **Analyze threats** by examining existing protections, identifying gaps, and ranking threats based on their risk score.
5. **Mitigate risk** by choosing to avoid, transfer, reduce, or accept it, and then develop a defence plan.
6. Finally, **Evaluate findings** by documenting the entire process, applying fixes, noting successes, and recording lessons learned for future threat models.

When performing threat modelling, there are multiple methods that can be used, such as: **STRIDE**, **PASTA**, **Trike**, **VAST**.

### PASTA

Process of Attack Simulation and Threat Analysis (PASTA) is a popular threat modelling framework that's used across many industries.

1. **Define Business and Security Objectives:** Establish clear goals for the threat model, such as protecting customer data, and understanding how sensitive information is handled.
2. **Define the Technical Scope:** Identify all application components that require evaluation, including data at rest and in use, network protocols, and security controls.
3. **Decompose the Application:** Identify how data moves through the application and how the existing controls protect it.
4. **Perform a Threat Analysis:** Research and gather up-to-date information on current attack vectors and techniques relevant to the application.
5. **Perform a Vulnerability Analysis:** A deeper investigation into potential vulnerabilities by examining the root causes of weaknesses.
6. **Conduct Attack Modelling:** Simulate attacks by creating attack trees to test identified vulnerabilities and validate potential threats.
7. **Analyze Risk and Impact:** All collected information from previous stages is assembled to make informed risk management recommendations to stakeholders.

## Glossary: Threats to Asset Security

**Angler phishing:** A technique where attackers impersonate customer service representatives on social media

**Advanced persistent threat (APT):** Instances when a threat actor maintains unauthorised access to a system for an extended period of time

**Adware:** A type of legitimate software that is sometimes used to display digital advertisements in applications

**Attack tree:** A diagram that maps threats to assets

**Baiting:** A social engineering tactic that tempts people into compromising their security

**Botnet:** A collection of computers infected by malware that are under the control of a single threat actor, known as the "bot-herder"

**Cross-site scripting (XSS):** An injection attack that inserts code into a vulnerable website or web application

**Cryptojacking:** A form of malware that installs software to illegally mine cryptocurrencies

**DOM-based XSS attack:** An instance when malicious script exists in the webpage a browser loads

**Dropper:** A type of malware that comes packed with malicious code which is delivered and installed onto a target system

**Fileless malware:** Malware that does not need to be installed by the user because it uses legitimate programs that are already installed to infect a computer

**Hacker:** Any person or group who uses computers to gain unauthorised access to data

**Identity and access management (IAM):** A collection of processes and technologies that helps organizations manage digital identities in their environment

**Injection attack:** Malicious code inserted into a vulnerable application

**Input validation:** Programming that validates inputs from users and other programs

**Intrusion detection system (IDS):** An application that monitors system activity and alerts on possible intrusions

**Loader:** A type of malware that downloads strains of malicious code from an external source and installs them onto a target system

**Malware:** Software designed to harm devices or networks

**Process of Attack Simulation and Threat Analysis (PASTA):** A popular threat modelling framework that’s used across many industries

**Phishing:** The use of digital communications to trick people into revealing sensitive data or deploying malicious software

**Phishing kit:** A collection of software tools needed to launch a phishing campaign

**Prepared statement:** A coding technique that executes SQL statements before passing them onto the database

**Potentially unwanted application (PUA):** A type of unwanted software that is bundled in with legitimate programs which might display ads, cause device slowdown, or install other software

**Quid pro quo:** A type of baiting used to trick someone into believing that they’ll be rewarded in return for sharing access, information, or money

**Ransomware:** Type of malicious attack where attackers encrypt an organization’s data and demand payment to restore access

**Reflected XSS attack:** An instance when malicious script is sent to a server and activated during the server’s response

**Rootkit:** Malware that provides remote, administrative access to a computer

**Scareware:** Malware that employs tactics to frighten users into infecting their device

**Smishing:** The use of text messages to trick users to obtain sensitive information or to impersonate a known source

**Social engineering:** A manipulation technique that exploits human error to gain private information, access, or valuables

**Spear phishing:** A malicious email attack targeting a specific user or group of users, appearing to originate from a trusted source

**Spyware:** Malware that’s used to gather and sell information without consent

**SQL (Structured Query Language):** A programming language used to create, interact with, and request information from a database

**SQL injection:** An attack that executes unexpected queries on a database

**Stored XSS attack:** An instance when malicious script is injected directly on the server

**Tailgating:** A social engineering tactic in which unauthorised people follow an authorized person into a restricted area

**Threat:** Any circumstance or event that can negatively impact assets

**Threat actor:** Any person or group who presents a security risk

**Threat modelling:** The process of identifying assets, their vulnerabilities, and how each is exposed to threats

**Trojan horse:** Malware that looks like a legitimate file or program

**Vishing:** The exploitation of electronic voice communication to obtain sensitive information or to impersonate a known source

**Watering hole attack:** A type of attack when a threat actor compromises a website frequently visited by a specific group of users

**Whaling:** A category of spear phishing attempts that are aimed at high-ranking executives in an organization

**Web-based exploits:** Malicious code or behaviour that’s used to take advantage of coding flaws in a web application
