**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISP012**

**Identity Management Policy**

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

[Document Objective [3](#document-objective)](#document-objective)

[Policy [3](#policy)](#policy)

[1. Scope and principles
[3](#scope-and-principles)](#scope-and-principles)

[2. Identity Lifecycle Management
[4](#identity-lifecycle-management)](#identity-lifecycle-management)

[3. Authentication, authorisation and audit
[5](#authentication-authorisation-and-audit)](#authentication-authorisation-and-audit)

[4. Technologies and systems
[5](#technologies-and-systems)](#technologies-and-systems)

[5. User and administrator responsibilities
[6](#user-and-administrator-responsibilities)](#user-and-administrator-responsibilities)

[6. Regulatory requirements
[6](#regulatory-requirements)](#regulatory-requirements)

[Revisions Record Sheet
[7](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [7](#approvals)](#approvals)

### General Information {#general-information .Heading-3_Green}

### Document Objective {#document-objective .Heading-3_Purple}

This Identity Management Policy outlines the requirements for managing
user and system identities at Community Fibre Limited, ensuring secure
provisioning, maintenance, and deprovisioning of identities. It supports
the overarching [ISP034-Access Control
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP034-Access%20Control%20Policy.pdf?csf=1&web=1&e=NVohJG)
by focusing on identity lifecycle management, while complementing other
supporting policies such as the Information Access Rights Policy
(ISP011), Password Management Policy (ISP040), User Registration Policy
(ISP014-User Registration Policy), and Privileged Access Rights Policy
(ISP013-Privileged Access Rights Policy).

**This document meets the following clauses:**

- ISO/IEC 27001:2022 -- A.5.16: Identity management

- The Electronic Communications (Security Measures) Regulations 2022 --
  Regulation 8 (Access controls for security-critical functions) and
  Code of Practice (3.1--3.7)

### Policy {#policy .Heading-3_Green}

### Scope and principles

This policy applies to all identities (user, system, and service
accounts) used to access Community Fibre\'s information assets,
networks, systems, and services, including those managed for employees,
contractors, third parties, and automated processes. It covers the full
identity lifecycle and applies throughout the asset lifecycle.

Key principles, informed by NCSC guidance:

- All users and systems must have unique, traceable identities to ensure
  accountability.

- Identity controls are proportionate to the sensitivity of assets (per
  ISP037 -- Information Classification and Handling Policy) and assessed
  risks.

- Identities are bound to roles with minimal access required.

- Automation should be used for provisioning and deprovisioning to
  reduce errors and delays.

- Prevent conflicts by separating identity management functions.

- Regularly review, auditing of identities and threat hunting to detect
  anomalies.

Identity management is handled by IT Service Desk, Security Operations,
Network Technology and HR, with oversight from the ISMS Board.

### Identity Lifecycle Management

The identity lifecycle includes provisioning, management, and
deprovisioning, aligned with joiners, movers, and leavers processes.

1.  **Provisioning**

- New identities are created upon formal request (e.g., from HR for
  employees or contracts for third parties), with verification of the
  individual\'s or system\'s legitimacy.

- Background checks are completed by HR.

- Identities are bound to roles via Role-Based Access Control (RBAC),
  integrated with an Identity Provider (e.g., Microsoft Entra ID) for
  automated provisioning.

- Third-party identities require contracts and/or NDAs before
  provisioning.

- All new identities must use unique credentials, avoid default
  password, and enable MFA where applicable (reference [ISP040-Password
  Management
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP040-Password%20Management%20Policy.pdf?csf=1&web=1&e=qpvx60)).

  1.  **Management and Maintenance**

- Identities are maintained through regular reviews (at least every 6
  months) to ensure alignment with current roles and business needs.

- Changes (e.g., role movers) trigger immediate updates via formal
  requests, adjusting access rights accordingly (reference -
  [ISD006-Joiner Mover Leaver
  Process](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISD006-Joiner%20Mover%20Leaver%20Process.pdf?csf=1&web=1&e=HSFx0x)).

- Authentication methods must match risk levels: Passwords for low-risk;
  MFA, certificates, or biometrics for higher-risk (e.g., remote access,
  privileged functions).

- Privileged identities require separate accounts from standard ones,
  with additional controls like privileged access workstations (PAWs)
  for security critical functions (reference Privileged Access Rights
  Policy).

- System and service identities (e.g., for APIs, operational technology
  systems) must be restricted, logged, and reviewed periodically.

  1.  **Deprovisioning**

- Identities are revoked immediately upon termination, role change, or
  contract end, triggered by HR notifications or security incidents.

- Automated deprovisioning is used where possible; manual processes must
  be logged and confirmed.

- Dormant identities (inactive for 90 days) are disabled and reviewed
  for deletion.

- Ensure all associated access rights, credentials, and data are removed
  or transferred securely.

### Authentication, authorisation and audit

- Authentication or verification of an identity claim shall use factors
  including passwords, MFA, certificates, or biometrics. Strength must
  align with asset classification (e.g., MFA mandatory for Confidential
  and Strictly Confidential access).

- Authorisation or determination of what the authenticated identity can
  do, shall be based on RBAC, least privilege, and need-to-know.
  Independent confirmation required for critical actions (e.g., code
  reviews, support tickets).

- Operational technology in network infrastructure must be isolated from
  IT systems; avoid \"browse up\" (accessing higher-trust from lower)
  and monitor cross-boundary communications.

- Remote authentication must consider device and location trust, with
  restrictions for non-UK or unmanaged devices.

- All identity-related activities (e.g., logins, changes) must be
  logged, linked to unique users, and monitored for anomalies by the SOC
  and Security Operations.

- Conduct periodic audits (every 6 months) and continuous vulnerability
  assessments on IAM systems.

- Suspicious activity (e.g., unusual access times) must trigger alerts
  and investigations.

### Technologies and systems

- Business systems shall use centralised identity systems (e.g., Entra
  ID), following best practise secure administration recommendations and
  Privileged Identity Management to manage access to privileged roles.

- Operational systems utilising LDAP and RADIUS for authentication and
  authorisation, ensuring secure configurations such as encryption
  (e.g., LDAPS, protected RADIUS communications) to mitigate risks like
  interception or unauthorised access.

- Privileged Access Management (PAM) with integration to Identity
  Provider solutions shall be used for access to security critical
  (including network oversight functions) and network management
  services.

- Implement Single Sign-On (SSO) and federated access (e.g., SAML) with
  trusted validation.

- External-facing IAM components must be isolated, patched promptly, and
  monitored as high-value targets.

- For OT-IT integration, push data one-way (OT to IT) and use
  inspectable protocols (e.g., web application firewalls).

### User and administrator responsibilities

- Users must safeguard their identities, report anomalies, and comply
  with authentication requirements.

- Administrators must enforce policies, use separate accounts for
  privileged tasks, and avoid untrusted devices for sensitive
  operations.

- Identified staff shall receive training on IAM best practices upon
  onboarding and annually.

### Regulatory requirements

- Identities for security critical functions must use unique
  credentials, MFA, and segregation (Regulation 8(2)(b-c), 8(5)).

- Remote access is restricted to managed devices via jump boxes
  (Regulation 3(3)(a),(d),(e), 3(5)).

- Risks from third-party identities are assessed (Regulation 7(1)), with
  logging of all access (Code of Practice para 3.4-3.7).

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

  -----------------------------------------------------------------------------
  Version   Date         Author         Changes
  --------- ------------ -------------- ---------------------------------------
  0.1       12/08/2025   Head of        Initial Draft as supporting policy to
                         Security       ISP034.

  1.0       17/09/2025   Head of        Review complete, major version update,
                         Security       sent for approval

                                        

                                        

                                        
  -----------------------------------------------------------------------------

### Approvals {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     03/10/2025     1.0       [CISP-101300](https://communityfibre.atlassian.net/browse/CISP-101300)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
