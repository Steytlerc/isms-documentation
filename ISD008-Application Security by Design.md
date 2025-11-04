**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISD008**

**Application Security by Design**

+------------------+-------------------------------------------+
| **Business       | 77 Hatton Garden, London, EC1N 8JS        |
| Addresses:**     |                                           |
+==================+===========================================+
|                  | 167-169 Great Portland Street\            |
|                  | 5th Floor\                                |
|                  | London\                                   |
|                  | W1W 5PF                                   |
|                  |                                           |
|                  | **TEL**: **0800 082 0770**                |
+------------------+-------------------------------------------+

### Table of Contents {#table-of-contents .TOC-Heading}

[Glossary [3](#glossary)](#glossary)

[General Information [3](#general-information)](#general-information)

[Policy [3](#policy)](#policy)

[Scope [4](#scope)](#scope)

[Key principles [4](#key-principles)](#key-principles)

[Application Security Requirements
[5](#application-security-requirements)](#application-security-requirements)

[Revisions Record Sheet
[8](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [8](#approvals)](#approvals)

### Glossary {#glossary .Heading-3_Green}

  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  Term              Description                      Reference
  ----------------- -------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Regulations**   The Electronic Communications    [The Electronic Communications Security Measures Regulations
                    Security Measures Regulations    2022.pdf](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Regulatory/The%20Electronic%20Communications%20Security%20Measures%20Regulations%202022.pdf?csf=1&web=1&e=XWHKUS)
                    2022                             

  **Code of         Telecommunications Security Code [E02781980_Telecommunications_Security_CoP_Accessible.pdf](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Regulatory/E02781980_Telecommunications_Security_CoP_Accessible.pdf?csf=1&web=1&e=1XipmF)
  Practice**        of Practice                      

  **OWASP           Provides a basis for testing web [OWASP_Application_Security_Verification_Standard_5.0.0_en](https://github.com/OWASP/ASVS/blob/v5.0.0/5.0/OWASP_Application_Security_Verification_Standard_5.0.0_en.pdf)
  Application       application technical security   
  Security          controls and provides developers 
  Verification      with a list of requirements for  
  Standard**        secure development.              
  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### General Information {#general-information .Heading-3_Green}

The purpose of this control is to ensure all information security and
privacy requirements are identified and addressed when developing or
acquiring applications.

**This document meets the following clauses:**

- ISO/IEC 27001:2022 Annex A.8.26 - Application Security Requirements.

### Policy {#policy .Heading-3_Green}

We operate public electronic communications networks and services and
are subject to UK regulations. Our systems are predominantly hosted on
cloud platforms, and we undertake significant bespoke software
development. This policy integrates secure-by-design principles into our
development lifecycle, referencing our [ISP042-Software Development
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP042-Software%20Development%20Policy.pdf?csf=1&web=1&e=6ESagh)
for processes such as secure coding, testing, and deployment. We adopt a
systematic approach to application security and privacy by:

- Classifying information as 'Confidential' or 'Strictly Confidential'
  in line with the [ISP037-Information Classification and Handling
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP037-Information%20Classification%20and%20Handling%20Policy.pdf?csf=1&web=1&e=iTtSNM)

- Addressing identification, access, authorisation, and segregation
  through:

  - Identity management to ensure entities are who they claim to be.
    [ISP012-Identity Management
    Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/CFL-006%20-%20Process%20Document%20-%20Change%20Management%20-%20Copy.pdf?csf=1&web=1&e=hrA8jk)

  - Authentication information to ensure \'we know who we are dealing
    with before we give them information. [ISP040-Password Management
    Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP040-Password%20Management%20Policy.pdf?csf=1&web=1&e=lktNQo)

  - Privileged access rights. [ISP013-Privileged Access Rights
    Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/CFL-006%20-%20Process%20Document%20-%20Change%20Management%20-%20Copy.pdf?csf=1&web=1&e=5YZp4W)

  - A.8.5: Secure authentication.

- Defining application information and privacy requirements through risk
  assessment, analysis, and treatment (per ISO 27001:2022 Clause 6.1.2
  and 6.1.3).

- Encrypting services in line with [ISP035-Cryptographic Control
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP035-Cryptographic%20Control%20Policy.pdf?csf=1&web=1&e=JoW6T3),
  considering the information classification. We always encrypt where
  any Personally Identifiable Information (PII) or sensitive data will
  be passing over untrusted networks.

- Managing compliance in line with customer and business requirements
  and standards for information security.

- Ensuring that critical services are constantly monitored for attack or
  undesired activity, with appropriate alerting if anomalous activity is
  detected.

**This policy applies to all in-house developed applications, acquired
third-party applications, and cloud-based systems on AWS and Azure.**

### Scope {#scope .Heading-3_Green}

This policy covers:

- Bespoke applications developed internally, including web applications,
  APIs, and backend services.

- Cloud-hosted systems on AWS (e.g., EC2, S3, Lambda) and Azure (e.g.,
  Virtual Machines, Blob Storage, Functions).

- Integration with public electronic communications networks.

- All phases of the software development lifecycle as outlined in
  [ISP042-Software Development
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP042-Software%20Development%20Policy.pdf?csf=1&web=1&e=wngyE4),
  including requirements gathering, design, coding, testing, deployment,
  and maintenance.

**Exclusions**: This does not cover hardware-specific security (e.g.,
routers), which is addressed in separate network security policies.

### Key principles {#key-principles .Heading-3_Green}

**To align with the Regulations:**

- Applications must be designed to reduce risks of security compromises,
  including identifying risks to functions (e.g., whether they handle
  sensitive data or are security-critical), recording exposures to
  incoming signals, and ensuring independence from external dependencies
  (e.g., no reliance on non-UK persons/equipment for risk
  identification).

- Applications must protect stored data and functions using technical
  means appropriate to the data/function (e.g., encryption for sensitive
  data, access controls for security-critical functions).

- Adopt a risk-based approach, ensuring proportionality and
  appropriateness of measures.

- For third-party components (e.g., AWS/Azure services), assess and
  mitigate supply chain risks.

- Integrate logging and monitoring into applications. (Monitoring and
  Analysis

- Ensure timely patching of vulnerabilities.

- Include security testing in development.

### Application Security Requirements {#application-security-requirements .Heading-3_Green}

1.  **Requirements gathering and risk assessment**

- Conduct a security risk assessment at the start of any development or
  acquisition project, identifying \"assessed security risks\" and
  classifying functions as security-critical if they impact
  network/service operation.

- Document risks in a written record (retained for at least 3 years per
  Regulation 3(4)), including exposure to incoming signals (e.g., API
  endpoints).

- For AWS/Azure: Leverage built-in tools like AWS Security Hub or Azure
  Security Center to automate risk identification.

- Reference: [ISP042-Software Development
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP042-Software%20Development%20Policy.pdf?csf=1&web=1&e=qqU7hp)

2.  **Secure design**

- Design applications and systems to minimise attack surfaces, e.g.,
  segment networks/functions to prevent a compromise in one part
  affecting others.

- Design applications and systems to be patched rapidly without the need
  for downtime.

- Ensure security-critical functions are protected and located
  appropriately (e.g., in isolated VPCs on AWS or Virtual Networks on
  Azure).

- Systems and application must not be publicly accessible unless there
  is a clear business justification.

- Test environments must only be accessible from authorise systems
  and/or IP addresses.

- Ensure PII is minimised and protected (e.g., anonymisation where
  possible).

- Do not use production data in test environments.

- Use AWS Well-Architected Framework Security Pillar and Azure
  Well-Architected Framework for design reviews.

- All systems must be recoverable, ensure that backups form part of all
  designs. [ISP043-Information Backup
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP043-Information%20Backup%20Policy.pdf?csf=1&web=1&e=rm3BfU)

- Align designs with OWASP Application Security Verification Standard
  (ASVS) levels, targeting Level 2 for standard applications and Level 3
  for critical ones.

3.  **Secure Coding and Implementation**

- Follow secure coding standards from OWASP Top 10 and align with Code
  of Practice Section 3: Technical Guidance Measures (e.g., Management
  Plane 1 for access controls).

- Implement input validation to protect against injection attacks,
  especially for functions exposed to incoming signals.

- Use least privilege principles for access [ISP013-Privileged Access
  Rights
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/CFL-006%20-%20Process%20Document%20-%20Change%20Management%20-%20Copy.pdf?csf=1&web=1&e=5YZp4W)

- For APIs: Enforce rate limiting, JWT tokens, and API gateways.

- Reference: [ISP042-Software Development
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP042-Software%20Development%20Policy.pdf?csf=1&web=1&e=qqU7hp)

- For cloud environments, use infrastructure as code (IaC) tools like
  Terraform with security scanning (Aikido) to ensure secure
  configurations.

4.  **Authentication and authorisation**

We secure the confidentiality, integrity, and authenticity of
communicating with clients and actions across transport and application
layers.

**Transport layer:**

- All communications must use HTTPS with TLS 1.3 or higher.

- For AWS/Azure: Enable TLS termination at load balancers (e.g., AWS
  ALB, Azure Application Gateway) and enforce HSTS.

**Application layer:**

- Users authenticate via:

  - Username/password plus TOTP (if enabled) for multi-factor
    authentication (MFA).

  - SAML SSO via trusted identity providers (e.g., Azure Entra ID).

- On success, issue session tokens (e.g., JWT) with short expiry
  (configurable, default 30 minutes).

- Implement role-based access control (RBAC) and attribute-based access
  control (ABAC) where appropriate to enforce fine-grained
  authorizations

5.  **Encryption**

- Encrypt all sensitive data in transit and at rest.

- Use AWS KMS or Azure Key Vault for secrets management.

- Personally Identifiable Information must always be encrypted over
  untrusted networks; use AES-256 or equivalent.

- Rotate encryption keys regularly and manage secrets securely, avoiding
  hard coding in applications.

6.  **Monitoring and logging**

- Integrate logging for all critical events (e.g., authentication
  failures, access to sensitive data).

- Use AWS CloudWatch/GuardDuty or Azure Monitor/Sentinel for real-time
  monitoring and anomaly detection.

- Retain logs for at least 13 months (per Code of Practice Section 5).

- Alert on suspicious activity, e.g., via email/SMS to security team.

7.  **Testing and vulnerability management**

- Conduct open-source dependency, static/dynamic application and secrets
  security testing using Aikido.

- Perform penetration testing annually or on major changes.

- For AWS/Azure: Use Security Hub or Defender for automated scans.

- Patch vulnerabilities promptly, prioritising critical findings within
  14 days. [ISP036-Management of technical
  vulnerabilities](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP036-Management%20of%20technical%20vulnerabilities.pdf?csf=1&web=1&e=xWHPOp)

- Reference: [ISP042-Software Development
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP042-Software%20Development%20Policy.pdf?csf=1&web=1&e=KwcXaK)
  Section "Security testing in development and acceptance."

8.  **Secure business logic**

- Design and implement business logic to prevent abuse, such as
  excessive usage, workflow bypassing, or unauthorised state transitions
  (i.e. user to admin), as highlighted in OWASP Business Logic Abuse Top
  10.

- Test for business logic flaws including data validation, ability to
  forge requests, integrity checks, process timing, number of records
  returned, ability to bypass steps, and abuse of functionality.

- Model business processes to identify and mitigate flaws that could
  lead to unintended behaviour.

9.  **Error handling and input/output sanitisation**

- Applications and services must not leak sensitive information in error
  messages.

- Sanitise all inputs and outputs to prevent attacks like XSS or
  injection.

- Use structured exception handling and provide generic error messages
  to users while logging detailed errors internally.

10. **Third-party and supply chain security**

- Assess third-party libraries and services for vulnerabilities using
  Aikido.

- Maintain a software bill of materials (SBOM) for all applications.

- Ensure right-of-use and licensing requirements are met.

11. **Secure deployment and operations**

- Use secure CI/CD pipelines with automated security gates.

- Implement blue-green deployments or canary releases to minimise
  downtime during updates.

- For containerised apps scan images for vulnerabilities and enforce
  runtime security.

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

  ----------------------------------------------------------------------------
  Version   Date         Author        Changes
  --------- ------------ ------------- ---------------------------------------
  0.1       05/08/2025   Head of       Initial Draft
                         Security      

  1.0       06/09/2025   Head of       Major version update, sent for
                         Security      approval.

                                       

                                       

                                       
  ----------------------------------------------------------------------------

### Approvals {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     03/10/2025     1.0       [CISP-101543](https://communityfibre.atlassian.net/browse/CISP-101543)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
