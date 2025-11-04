**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISP011**

**Information Access Rights Policy**

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

[References [2](#references)](#references)

[General Information [3](#general-information)](#general-information)

[Document Objective [3](#document-objective)](#document-objective)

[Policy [3](#policy)](#policy)

[1. Scope and principles
[3](#scope-and-principles)](#scope-and-principles)

[2. Access rights based on information classification
[4](#access-rights-based-on-information-classification)](#access-rights-based-on-information-classification)

[3. Access right process
[5](#access-right-process)](#access-right-process)

[4. User Responsibilities
[5](#user-responsibilities)](#user-responsibilities)

[5. Regulatory requirements
[6](#regulatory-requirements)](#regulatory-requirements)

[Revisions Record Sheet
[7](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [7](#approvals)](#approvals)

###  {#section .Heading-3_Green}

### References {#references .Heading-3_Green}

  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  Ref#    Document                        Reference
  ------- ------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **1**   ISO/IEC 27001:2022              [[BS EN ISO_IEC 27001_2023+A1_2024 (7 Apr 2025 9-38am
                                          UTC).pdf]{.underline}](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Standards%20Documentation/27000%20-%202022/BS%20EN%20ISO_IEC%2027001_2023+A1_2024%20(7%20Apr%202025%209-38am%20UTC).pdf?csf=1&web=1&e=oPNJ1I)

  **2**   The Electronic Communications   [[The Electronic Communications (Security Measures) Regulations 2022]{.underline}](https://www.legislation.gov.uk/uksi/2022/933/contents/made)
          Security Measures Regulations   
          2022 (ECR)                      

  **3**   Telecommunications Security     [[Telecommunications Security Code of Practice]{.underline}](https://assets.publishing.service.gov.uk/media/6384d09ed3bf7f7eba1f286c/E02781980_Telecommunications_Security_CoP_Accessible.pdf)
          Code of Practice (CoP)          

  **4**   NCSC Cyber Assessment Framework <https://www.ncsc.gov.uk/collection/cyber-assessment-framework>
          (CAF) v4.0                      
  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### General Information {#general-information .Heading-3_Green}

### Document Objective

This Information Access Rights Policy outlines the requirements for
managing access rights to Community Fibre Limited\'s information assets,
ensuring they are granted, reviewed, and revoked in a controlled manner.
It supports the overarching Access Control Policy (ISP010-Access Control
Policy) by focusing specifically on information access rights, while
complementing other supporting policies:

- ISP012-Identity Management Policy

- ISP040-Password Management Policy

- ISP014-User Registration Policy

- ISP013-Privileged Access Rights Policy

**This document meets the following clauses:**

- ISO/IEC 27001:2022 -- A.5.15: Access control

- ISO/IEC 27002:2022 -- A.5.18: Access rights

- The Electronic Communications (Security Measures) Regulations 2022 --
  Regulation 8 (Access controls for security-critical functions) and
  Code of Practice (3.1--3.7)

Access rights to information assets are managed to protect
confidentiality, integrity, and availability, based on the principles of
\"need-to-know,\" \"least privilege,\" and role-based access control
(RBAC). This policy applies to all employees, contractors, third
parties, and systems handling Community Fibre information assets
throughout their lifecycle.

### Policy {#policy .Heading-3_Green}

The purpose of this policy is to ensure appropriate access to
information networks and systems are provided in line with identified
requirements and are adequate and proportionate for assessed information
security risks.

### Scope and principles

This policy applies to all access rights related to information assets,
including electronic and physical forms, across Community Fibre\'s
networks, systems, and services. It encompasses user access, privileged
access, and third-party access, with references to supporting policies
for detailed procedures.

Key principles:

- Need-to-Know

- Least Privilege

- Role-Based Access Control (RBAC)

- Segregation of Duties

- Information Classification Alignment

All access rights must consider the value, sensitivity, and risks
associated with information assets, as identified through risk
assessments.

### Access rights based on information classification

Access to information assets is governed by their classification
(**ISP037 -- Information Classification and Handling Policy**). The
following guidelines apply:

- **Public**: Access is unrestricted but must be approved for release.
  No specific controls beyond standard authentication are required, but
  usage must comply with business policies.

- **Confidential**: Access is limited to authorised personnel on a
  need-to-know basis. Default for most business-sensitive data (e.g.,
  draft work, customer communications).

  - Requires RBAC with multi-factor authentication for remote access.

  - Storage and transfer must use approved systems (e.g., SharePoint,
    Teams), with encryption for removable media if approved.

  - Third-party sharing requires NDAs, DPAs (for PII), and owner
    approval.

- **Strictly Confidential**: Access is restricted due to potential
  severe impact (e.g., PII, PCI data, intellectual property, critical
  infrastructure details).

  - Limited to essential personnel; requires explicit approval from the
    asset owner.

  - MFA mandatory; privileged access must use privileged access
    workstations (PAWs) for security-critical functions.

  - Storage on personal devices restricted; hard copies must be secured
    (e.g., locked cabinets) and not removed off site without permission.

  - PCI data handling follows PCI DSS guidelines in ISP037-Information
    Classification and Handling Policy, with no storage of sensitive
    elements (e.g., CVV) and encryption for transmission.

  - Passwords must be stored in an approved password manager.

  - Third-party access requires NDAs, DPAs, risk assessments, and logged
    approvals.

Information owners (**ISP037 -- Information Classification and Handling
Policy**) are responsible for classifying assets and approving access
rights.

### Access right process

1.  **Granting Access**

- Access requests must be submitted via the IT Service Desk
  (<itsupport@communityfibre.co.uk>) or the Network Technology team with
  approval from the information asset/system owner or line manager.

- Access is provisioned using RBAC and automated tools where possible,
  aligned with user roles (ISP014-User Registration Policy for
  onboarding).

- For privileged access, follow the ISP013-Privileged Access Rights
  Policy, including segregation of duties and PAW usage.

- Third-party access requires signed NDA, contract and risk assessment.

  1.  **Reviewing Access:**

- Access rights are reviewed at least every 6 months by IT Service Desk,
  Security Operations and Network Technology team, or upon role changes,
  or incidents.

- Reviews include validation against business needs, classification
  levels, and compliance with Electronic Communications (Security
  Measures) Regulations requirements (e.g., logging of privileged access
  per Regulation 8(5)).

- Exceptions (e.g., shared IDs) must be documented, justified, and
  re-approved.

  1.  **Revoking Access:**

<!-- -->

- Access is revoked immediately upon termination, role change, or
  security incident notification (e.g., from HR or Security Operations).

- Automated de-provisioning is used where integrated; manual revocation
  is logged.

- Unused accounts are disabled after 90 days of inactivity.

All actions are logged, auditable, and aligned with the ISP012-Identity
Management Policy for user identities.

### User Responsibilities

- Users must only access information required for their roles and report
  any unauthorised access or anomalies immediately to Security
  Operations.

- Authentication information (e.g., passwords) must be kept confidential
  (reference [ISP040-Password Management
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP040-Password%20Management%20Policy.pdf?csf=1&web=1&e=zYTtvK)).

- Users are accountable for actions under their assigned IDs and must
  comply with training on access controls.

### Regulatory requirements

Access requirements under the Electronic Communications (Security
Measures) Regulations and its Code of Practice include:

- **Security-critical functions**: Access is restricted using least
  privilege, phishing resistant MFA, and privileged access workstations
  for high-risk activities (Reg 8(2)(b), 8(4), Reg 4(4)(a) \[**2**\];
  CoP para 3.4--3.13, M11.08 \[**3**\])

- **Remote administrative access**: Limited to UK-based or managed
  devices; third-party remote administration via jump boxes only (Reg
  3(3)(f), 4(4)(a) \[**2**\], 5(2); CoP M2.01, M10.30 \[**3**\])

- **Logging and Monitoring**: All access to security-critical
  information is logged, with unique credentials and regular reviews
  (Reg 6(3)(a-d), 8(2)(b),(d), 8(4), 8(5)(b),(c)) \[**2**\].

- **Risk-Based Controls**: Access rights are proportionate to risks,
  including from third parties (Reg 8(2) (d-e), Reg 11(b)) \[**2**\].

**Non-compliance with these requirements will result in regulatory
reporting obligations.**

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

  --------------------------------------------------------------------------
  Version   Date         Author           Changes
  --------- ------------ ---------------- ----------------------------------
  0.1       12/08/2025   Head of Security Initial Draft as supporting policy
                                          to ISP010.

  1.0       03/10/2025   Head of Security Major version update, references
                                          added, release for approval

                                          
  --------------------------------------------------------------------------

### Approvals {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     03/10/2025     1.0       [CISP-101694](https://communityfibre.atlassian.net/browse/CISP-101694)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
