# Module 2: Protect Organisational Assets

## Overview

* Effective data handling processes
* The role of encryption and hashing in safeguarding information
* Standard access controls

## Effective data handling processes

### Types of Security Controls

* **Technical Controls:** These involve technology to protect assets, such as encryption and authentication systems.
* **Operational Controls:** These are day-to-day security tasks performed by people, like awareness training and incident response.
* **Managerial Controls:** These focus on how technical and operational controls reduce risk, including policies, standards, and procedures.

Least privilege is closely related to another fundamental security principle, the **separation of duties** - a security concept that divides tasks and responsibilities among different users to prevent giving a single user complete control over critical business functions.

* **Information Privacy:** This is about protecting data from unauthorised access and distribution, giving individuals and organizations the right to control how their private information is shared.
* **Principle of Least Privilege:** Security controls should limit access to information based on the user and situation, ensuring that individuals only have access to what is necessary for their role.

### The data lifecycle

The data lifecycle is a five-stage model that security teams use to protect information, influencing policies and technology choices. The stages are: **Collect**, **Store**, **Use**, **Archive**, and **Destroy**.

### Data governance

Data governance is a set of processes that define how an organization manages information. Governance often includes policies that specify how to keep data private, accurate, available, and secure throughout its lifecycle. Data governance policies commonly categorise individuals into a specific role:

* **Data owner:** the person that decides who can access, edit, use, or destroy their information.
* **Data custodian:** anyone or anything that's responsible for the safe handling, transport, and storage of information.
* **Data steward:** the person or group that maintains and implements data governance policies set by an organization.

### Notable privacy regulations

* General Data Protection Regulation (GDPR): An EU regulation giving data owners control over their personal information, applicable to any business handling EU citizens' data.
* **Payment Card Industry Data Security Standard (PCI DSS):** A set of security standards for securing credit and debit card transactions against fraud.
* **Health Insurance Portability and Accountability Act (HIPAA):** A U.S. law protecting sensitive patient health information, prohibiting disclosure without consent.

## The role of encryption and hashing in safeguarding information

Cryptography protects Personally Identifiable Information (PII) online, using encryption and decryption to secure data. Cryptography transforms readable information (plaintext) into an unreadable format (ciphertext) through encryption.

* **Encryption:** the process of converting data from a readable format to an encoded format
* **Public key infrastructure (PKI):** an encryption framework that secures the exchange of online information
* **Cipher:** an algorithm that encrypts information

**Caesar's Cipher:** Is an early example of a cryptographic algorithm that shifts letters in the alphabet by a fixed number of spaces. This method is not widely used today due to its simplicity and reliance on a single key and its vulnerability to brute-force attacks, where all possible shifts can be tried to crack the message.

* **Symmetric encryption** is the use of a single secret key to exchange information. Because it uses one key for encryption and decryption, the sender and receiver must know the secret key to lock or unlock the cipher.
* **Asymmetric encryption** is the use of a public and private key pair for encryption and decryption of data. It uses two separate keys: a public key and a private key. The public key is used to encrypt data, and the private key decrypts it. The private key is only given to users with authorized access.

### Approved algorithms

Many web applications use a combination of symmetric and asymmetric encryption. This is how they balance user experience with safeguarding information. Examples include:

* **Symmetric algorithms:** Triple DES (3DES), Advanced Encryption Standard (AES).
* **Asymmetric algorithms:** Rivest Shamir Adleman (RSA), Digital Signature Algorithm (DSA).

### Obscurity is not security

In the world of cryptography, a cipher must be proven to be unbreakable before claiming that it is secure. According to **Kerckhoff's principle**, cryptography should be designed in such a way that all the details of an algorithm (except for the private key) should be knowable without sacrificing its security. For example, you can access all the details about how AES encryption works online and yet it is still unbreakable.

**Note:** A cryptographic system should not be considered secure if it requires secrecy around how it works.

### The evolution of hash functions

Hash functions are algorithms that produce a code that can't be decrypted. They convert information into a unique value that can then be used to determine its integrity.

Hash functions have been around since the early days of computing. They were originally created as a way to quickly search for data. Since the beginning, these algorithms have been designed to represent data of any size as small, fixed-size values, or digests. One of the earliest hash functions is Message Digest 5, more commonly known as **MD5**. Professor Ronald Rivest of the Massachusetts Institute of Technology (MIT) developed MD5 in the early 1990s as a way to verify that a file sent over a network matched its source file.

MD5 values are limited to 32 characters in length. Due to the limited output size, the algorithm is considered to be vulnerable to hash collision, an instance when different inputs produce the same hash value. Because hashes are used for authentication, a hash collision is similar to copying someone's identity. Attackers can carry out collision attacks to fraudulently impersonate authentic data.

To avoid the risk of hash collisions, functions that generated longer values were needed. MD5's shortcomings gave way to a new group of functions known as the Secure Hashing Algorithms, or SHAs. Five functions make up the SHA family of algorithms: **SHA-1**, **SHA-224**, **SHA-256**, **SHA-384**, **SHA-512**.

* **A rainbow table** is a file of pre-generated hash values and their associated plaintext. They're like dictionaries of weak passwords.
* **Salting** is an additional safeguard that's used to strengthen hash functions by adding a random string of characters data before it's hashed to produce a more unique hash value that is resilient to rainbow table attacks.

## Standard access controls

Access controls are security controls that manage access, authorisation, and accountability of information. They are commonly structured around the **Authentication**, **Authorization**, and **Accounting** **(AAA)** framework. Single sign-on (SSO) and multi-factor authentication (MFA) are two technologies that have become popular for implementing these authentication factors.

**Single sign-on (SSO)** is a technology that combines several different logins into one. This technology became available in the mid-1990s as a way to combat password fatigue, which refers to people's tendency to reuse passwords across services. More companies are turning to SSO as a solution to their authentication needs for three reasons:

* **SSO improves the user experience** by eliminating the number of usernames and passwords people have to remember.
* **Companies can lower costs** by streamlining how they manage connected services.
* **SSO improves overall security** by reducing the number of access points attackers can target.

Usernames and passwords alone are not always the most secure way of protecting sensitive information. SSO provides useful benefits, but there's still the risk associated with using one form of authentication. For example, a lost or stolen password could expose information across multiple services. Thankfully, there's a solution to this problem.

**Multi-factor authentication (MFA)** requires a user to verify their identity in two or more ways to access a system or network. MFA builds on the benefits of SSO. It works by having users prove that they are who they claim to be. The MFA process asks users to provide these proofs, such as:

* **Something a user knows:** most commonly a username and password
* **Something a user has:** normally received from a service provider, like a one-time passcode (OTP) sent via SMS
* **Something a user is:** refers to physical characteristics of a user, like their fingerprints or facial scans

Requiring multiple forms of identification is an effective security measure, especially in cloud environments. It can be difficult for businesses in the cloud to ensure that the users remotely accessing their systems are not threat actors. MFA can reduce the risk of authenticating the wrong users by requiring forms of identification that are difficult to imitate or brute force.

### Identity and access management

Identity and access management (IAM) is a collection of processes and technologies that helps organizations manage digital identities in their environment. Both AAA and IAM systems are designed to authenticate users, determine their access privileges, and track their activities within a system. A key to doing this is implementing two fundamental security principles that limit access to organizational resources:

* The **principle of least privilege** in which a user is only granted the minimum level of access and authorization required to complete a task or function.
* **Separation of duties**, which is the principle that users should not be given levels of authorization that would allow them to misuse a system.

* **User Provisioning:** is a process of creating and maintaining a user's digital identity, including granting and revoking access rights, which security analysts are routinely involved in.
* **Authorization Frameworks:** Organizations use frameworks like Mandatory Access Control (MAC), Discretionary Access Control (DAC), and Role-Based Access Control (RBAC) to determine what resources authenticated users can access.

## Glossary: Protect Organisational Assets

**Access controls:** Security controls that manage access, authorization, and accountability of information

**Algorithm:** A set of rules used to solve a problem

**Application programming interface (API) token:** A small block of encrypted code that contains information about a user

**Asymmetric encryption:** The use of a public and private key pair for encryption and decryption of data

**Basic auth:** The technology used to establish a user's request to access a server

**Bit:** The smallest unit of data measurement on a computer

**Brute force attack:** The trial and error process of discovering private information

**Cipher:** An algorithm that encrypts information

**Cryptographic key:** A mechanism that decrypts ciphertext

**Cryptography:** The process of transforming information into a form that unintended readers can't understand

**Data custodian:** Anyone or anything that's responsible for the safe handling, transport, and storage of information

**Data owner:** The person that decides who can access, edit, use, or destroy their information

**Digital certificate:** A file that verifies the identity of a public key holder

**Encryption:** The process of converting data from a readable format to an encoded format

**Hash collision:** An instance when different inputs produce the same hash value

**Hash function:** An algorithm that produces a code that can't be decrypted

**Hash table:** A data structure that's used to store and reference hash values

**Identity and access management (IAM):** A collection of processes and technologies that helps organizations manage digital identities in their environment

**Information privacy:** The protection of unauthorised access and distribution of data

**Multi-factor authentication (MFA):** A security measure that requires a user to verify their identity in two or more ways to access a system or network

**Non-repudiation:** The concept that the authenticity of information can't be denied

**OAuth:** An open-standard authorization protocol that shares designated access between applications

**Payment Card Industry Data Security Standards (PCI DSS):** A set of security standards formed by major organizations in the financial industry

**Personally identifiable information (PII):** Any information used to infer an individual's identity

**Principle of least privilege:** The concept of granting only the minimal access and authorization required to complete a task or function

**Protected health information (PHI):** Information that relates to the past, present, or future physical or mental health or condition of an individual

**Public key infrastructure (PKI):** An encryption framework that secures the exchange of online information

**Rainbow table:** A file of pre-generated hash values and their associated plaintext

**Salting:** An additional safeguard that's used to strengthen hash functions

**Security assessment:** A check to determine how resilient current security implementations are against threats

**Security audit:** A review of an organization's security controls, policies, and procedures against a set of expectations

**Security controls:** Safeguards designed to reduce specific security risks

**Separation of duties:** The principle that users should not be given levels of authorization that would allow them to misuse a system

**Session:** A sequence of network HTTP basic auth requests and responses associated with the same user

**Session cookie:** A token that websites use to validate a session and determine how long that session should last

**Session hijacking:** An event when attackers obtain a legitimate user's session ID

**Session ID:** A unique token that identifies a user and their device while accessing a system

**Single Sign-On (SSO):** A technology that combines several different logins into one

**Symmetric encryption:** The use of a single secret key to exchange information

**User provisioning:** The process of creating and maintaining a user's digital identity
