# Core Concepts

The Secure Software Concepts domain encompasses essential principles from information security that are crucial for secure software development, including **confidentiality**, **integrity and** **availability** (CIA).

To fully describe operational security elements, authentication, authorization, auditability and nonrepudiation have been incorporated into the existing CIA framework.

* **Confidentiality**: Ensuring that information is only accessible to those with the proper authorization.
* **Integrity**: Maintaining the accuracy and reliability of data and systems, preventing unauthorized tampering or alterations.
* **Availability**: Ensuring that systems and data are consistently accessible and operational when needed.
* **Authentication**: Verifying the identity of users or entities accessing a system or data.
* **Authorization**: Granting or denying specific permissions and access rights to users or entities based on their authenticated identity.
* **Auditability**: The capability to track and record actions and events within a system for monitoring and accountability purposes.
* **Nonrepudiation**: Preventing individuals from denying their actions or transactions, ensuring accountability and trustworthiness.

### Secure Development Lifecycle

Adding team awareness and education, gates and security requirements, bug tracking, threat modeling, fuzzing, security reviews and mitigations to the software development lifecycle makes it more secure.

#### Team Awareness & Education

All team members should undergo ongoing role-specific training in both basic security knowledge, essential for the entire team, and advanced topics tailored to their specific roles to ensure they remain up-to-date and equipped to address evolving security challenges throughout their careers.

#### Gates & Security Requirements

During the development process, periodic security reviews, known as gates, are conducted to ensure adherence to security requirements.

#### Bug Tracking

As code is being developed, it's common to uncover bugs, which are code components exhibiting problematic behaviors, occasionally presenting exploitable vulnerabilities, and necessitating tracking and resolution.

#### Threat Modeling

Threat modeling serves to comprehensively identify and describe system threats while recording mitigation strategies.

#### Fuzzing

Fuzzing is an automated testing technique involving the application of diverse inputs to an interface, examining the outputs for unexpected behaviors, commonly used by both security testers and hackers to discover vulnerabilities and potential exploits.

#### Security Reviews

Security reviews serve as checkpoints within the process to ensure these steps are not bypassed and are functioning correctly.

#### Mitigations

Adopting a risk assessment model like DREAD, which calculates risk as a product of impact and probability, aids in prioritizing bug fixes, with the mitigation process offering four standard options for addressing security bugs: **do nothing**, **warn the user**, **remove the problem**, and **fix the problem**.

#### Software Security vs Quality

High-quality software can be defect-free but may not necessarily be secure. Conversely, the critical concern is that if software lacks quality and contains defects, it is unlikely to be secure.

<figure><img src="../.gitbook/assets/image (9).png" alt=""><figcaption><p>Security vs Quality</p></figcaption></figure>
