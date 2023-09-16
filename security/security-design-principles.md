# Security Design Principles

Secure designs are built upon a solid groundwork of secure design principles:

* **Good enough security**
  * There is an appropriate level of required security for systems
* **Least privilege**
  * Users and applications should have only the necessary rights and privileges to perform their current tasks.&#x20;
* **Separation of duties**
  * Software components should require multiple conditions to pass before a task can be considered as complete. This ensures no single individual can abuse the system&#x20;
* **Defense in depth**
  * Defense in depth is a security principle involving the use of multiple overlapping layers of protection to enhance security, with the understanding that no single defense mechanism is foolproof, and the goal is to make compromising a system more costly and time-consuming for adversaries.
* **Fail-safe**
  * Fail-safe, in the context of system design, means that when a system encounters a failure, it should transition to a secure and stable state.
* **Economy of mechanism**
  * Systems and security mechanisms should be kept as simple as possible because complexity increases the potential for vulnerabilities and makes troubleshooting more challenging.
* **Complete mediation**
  * Complete mediation is the security principle that requires continuous verification of a subject's authorization for each access request to an object and action.
* **Open design**
  * Open design is the principle that a system's security should not rely on the secrecy of its design or algorithms but instead on elements like keys, making the security independent of the design's obscurity.
* **Least common mechanism**
  * Least common mechanism is a design approach aimed at preventing unintentional information sharing among processes by minimizing shared components, favoring separate processes for distinct functions to enhance security.
* **Psychological acceptability**
  * A security system should not burden users as it will cause them to work around security aspects.
* **Weakest link**
  * Common point of failure of a system. A system is only as strong as the weakest link.
* **Leverage existing components**
  * New components increase the chances of new vulnerabilities being added. Therefore, reusing components should decrease the chances.
* **Single point of failure**
  * Software systems should not have a single point of failure.
