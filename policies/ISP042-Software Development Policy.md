**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISP042**

**Software development policy**

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

[General Information [3](#general-information)](#general-information)

[Policy [3](#policy)](#policy)

[Secure software design
[4](#secure-software-design)](#secure-software-design)

[Secure development practices
[5](#secure-development-practices)](#secure-development-practices)

[Security testing in development and acceptance
[6](#security-testing-in-development-and-acceptance)](#security-testing-in-development-and-acceptance)

[Software testing and release
[7](#software-testing-and-release)](#software-testing-and-release)

[Outsourced development
[7](#outsourced-development)](#outsourced-development)

[Adherence to policy [7](#adherence-to-policy)](#adherence-to-policy)

[Revisions Record Sheet
[8](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [8](#approvals)](#approvals)

### General Information {#general-information .Heading-3_Green}

**This document meets the following clauses:**

- Information Security Management System BS EN ISO/IEC 27002:2022 --
  A.8.25 Secure development life cycle

- Information Security Management System BS EN ISO/IEC 27002:2022 --
  A.8.26 Application security requirements

- Information Security Management System BS EN ISO/IEC 27002:2022 --
  A.8.28

> Secure coding

- Information Security Management System BS EN ISO/IEC 27002:2022 --
  A.8.29

> Security testing in development and acceptance

### Policy {#policy .Heading-3_Green}

The objective of this policy is to establish principles for the secure
development, acquisition, integration, and maintenance of software,
scripts, and automation tools.

All activities will incorporate security by design, with explicit
consideration of impacts to confidentiality, integrity, availability,
privacy, and network resilience. This aligns with the principle of
building security \"in\" to systems from the outset, as per ISO/IEC
27002:2022 controls A.8.25--A.8.29 and supports regulatory requirements
under the Electronic Communications (Security Measures) Regulations 2022
to reduce risks of security compromises in public electronic
communications networks and services.

Security requirements analysis and specification must be proportionate
to the risk level, size, and scope of the activity, with analysis
conducted as early as feasible to balance security benefits against
project delivery risks.

**Key considerations:**

- Identifying the need for analysis and specifications based on risk
  assessments, including exposure to incoming signals, sensitive data
  (e.g., content of signals or data controlling security-critical
  functions), and security-critical functions (e.g., those with
  significant impact on network operation).

- The timing of analysis - earlier the better from a security
  perspective, but may introduce more risk to project delivery, so both
  sides of the risk equation must be carefully assessed and weighed.

- Security requirements for:

  - Identification, authentication, and authorisation controls,
    including prevention of unauthorised access or interference.

  - Logging, monitoring, and analysis, with protection for tools that
    enable such functions.

  - Data classification and segregation, ensuring protection of
    sensitive data.

  - Controls on information transfer, including encryption for signals
    and data in transit.

  - Audit trails for remediation and recovery preparedness

  - Network architecture design aims to minimise the risks associated
    with the propagation of compromises throughout the network.

  - Trust boundaries must be established and maintained:

    - between areas such as internal and external networks, customer
      networks, partner networks, the internet and international
      networks

    - our networks and third-party administrator networks, such as those
      owned by network equipment suppliers and MSPs

    - between our security critical functions and functions in the
      access network or exposed edge

    - between management networks and other networks, including internal
      networks.

- Integration of business continuity and disaster recovery requirements,
  aligned with service criticality and SLAs, including the ability to
  operate without reliance on overseas persons, equipment, or data where
  risks are identified.

### Secure software design {#secure-software-design .Heading-3_Green}

Threat modelling is a core component of secure design, identifying risks
to software, scripts, and network functions, and enabling proportionate
controls. Designs must consider the business value of information and
processes, potential impacts from inadequate controls, and regulatory
duties to design networks that reduce security compromise risks.
Guidance for Application Security by Design is available on Jira:
Application Security By Design

- Design and requirements specifications must be documented, reviewed,
  and approved, reflecting evaluated security risks.

- Information security designs, requirements, and controls must address:

  - Protection of security-critical functions and sensitive data.

  - Location and exposure of equipment (e.g., minimising reliance on
    assets located overseas).

  - Segregation to prevent compromise propagation.

- Business continuity/disaster recovery must be integrated, ensuring
  restoration aligns with criticality and SLAs.

- For automation scripts, designs must include modelling of impacts on
  provisioning, management, and orchestration or security-critical
  components to avoid unauthorised interference or data exposure.

**Development environments**

Segregating software development, testing and production environments
minimises the likelihood of faulty code in production environments and
networks, aligning with duties to protect critical functions and
maintain architecture that reduces compromise risks.

- Development, testing (including UAT), and production environments must
  be logically segregated.

- Separate environments are mandatory for development, UAT, testing, and
  production, unless explicitly approved by the CIO with documented
  justification.

- Sensitive production data, including network signals or operational
  data, must not be utilised in non-production environments. When
  authorised by the CIO, such data must be anonymised entirely or
  pseudonymised. If anonymisation is impractical, appropriate security
  measures equivalent to production standards must be applied.

- Changes to any environment must follow a documented change management
  process, including verification of no unauthorised access.

- Network Operations scripts should be developed within isolated
  environments that accurately simulate the production environment,
  ensuring that live network components are not exposed.

- Web application frameworks must be used to aid in the development of
  secure web applications. The Open Web Application Security Project
  (OWASP) provides comprehensive resources.

### Secure development practices {#secure-development-practices .Heading-3_Green}

Secure engineering principles must be applied across all development
activities, including scripts for automation.

- Secure system engineering principles, including those from OWASP for
  web applications and telecom-specific standards where applicable, must
  be documented, maintained, and enforced.

- All development staff must undergo role-specific training on secure
  practices, threat modelling, and regulatory requirements.

- The development lifecycle must be documented, with security gates for
  approval at key stages (e.g., design, code, test).

- Secure repositories (e.g., version-controlled with access controls)
  must store all code, scripts, and documentation, ensuring
  confidentiality and integrity.

- Source code and scripts must have versioning, descriptions, and
  documentation; access must adhere to least privilege and separation of
  duties.

- Security hardening guidelines must be implemented across all
  components, including third-party libraries.

- Third-party packages must be sourced from approved, trusted vendors;
  modifications for production use require standards approval and
  vulnerability assessments.

- Robust frameworks must be used (e.g., OWASP-compliant for
  applications; secure scripting practices for automation).

- Supply chain risks must be assessed per the Code of Practice,
  including vendor security assessments and restrictions on high-risk
  suppliers.

### Security testing in development and acceptance {#security-testing-in-development-and-acceptance .Heading-3_Green}

Testing must verify security requirements and reduce vulnerabilities
before production deployment, integrating static/dynamic analysis and
peer reviews. Release processes must be documented and enforced.

- Pre-release verification must include peer approval, UAT, open-source
  dependency scanning, static code analysis and dynamic analysis.

- Developer tools (e.g., IDEs) must enable real-time vulnerability
  detection and remediation.

- Security requirements, including the protection of sensitive data and
  critical functions, must be explicitly tested.

- Internet-facing software and network tools must undergo independent
  penetration testing before launch and regular vulnerability scanning
  thereafter.

- Internal-facing software, scripts, and automation must undergo regular
  vulnerability scanning.

- Security scans and checks should be integrated into CI/CD pipelines,
  automatically preventing deployment when vulnerabilities are found.

Reference: <https://communityfibre.atlassian.net/wiki/x/AgAyQg>
(Application Security By Design)

### Software testing and release {#software-testing-and-release .Heading-3_Green}

To prevent vulnerabilities in production, testing and release must align
with the documented ISD007-Software Release Management procedure.

### Outsourced development {#outsourced-development .Heading-3_Green}

Outsourced activities must comply with vendor management and third-party
risk processes.

- Outsourced development arrangements will follow the vendor management
  process and be subject to the information security third party
  assessment process.

- Outsourced developers will be made aware of this policy and the
  defined secure system engineering principles.

- Outsourced developers are required to adhere to this policy and the
  defined secure system engineering principles.

### Adherence to policy {#adherence-to-policy .Heading-3_Green}

Failure to comply with this policy may result in disciplinary procedures
up to and including termination of employment or contract.

1.  
2.  
3.  
4.  

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

+---------+------------+------------+--------------------------------------+
| Version | Date       | Author     | Changes                              |
+=========+============+============+======================================+
| 0.1     | 26/09/2022 | ISO        | Initial Draft                        |
+---------+------------+------------+--------------------------------------+
| 1.0     | 28/09/2022 | ISO        | Final review, version change to 1.0  |
+---------+------------+------------+--------------------------------------+
| 1.1     | 04/09/2024 | Head of    | Reintroduction of control to         |
|         |            | Security   | mitigate software development risk,  |
|         |            |            | not material changes.                |
|         |            |            |                                      |
|         |            |            | Standard version updated to 2017     |
+---------+------------+------------+--------------------------------------+
| 2.0     | 28/08/2025 | Head of    | Transition to ISO/IEC 27001:2022;    |
|         |            | Security   | expanded scope to network            |
|         |            |            | automation/scripts; integration of   |
|         |            |            | Electronic Communications (Security  |
|         |            |            | Measures) Regulations 2022 and Code  |
|         |            |            | of Practice requirements.            |
+---------+------------+------------+--------------------------------------+

### Approvals {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     17/09/2025     2.0       [CISP-101298](https://communityfibre.atlassian.net/browse/CISP-101298)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
