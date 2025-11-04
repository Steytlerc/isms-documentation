**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISP013**

**Privileged Access Rights Policy**

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

### Contents {#contents .TOC-Heading}

[References [3](#references)](#references)

[General Information [3](#general-information)](#general-information)

[Document Objective [3](#document-objective)](#document-objective)

[Policy [4](#policy)](#policy)

[1. Scope and principles
[4](#scope-and-principles)](#scope-and-principles)

[2. Identification and classification of privileged access
[4](#identification-and-classification-of-privileged-access)](#identification-and-classification-of-privileged-access)

[3. Granting and managing privileged access rights
[5](#granting-and-managing-privileged-access-rights)](#granting-and-managing-privileged-access-rights)

[4. Privileged access workstations (PAWs)
[6](#privileged-access-workstations-paws)](#privileged-access-workstations-paws)

[5. Monitoring, auditing, and session management
[7](#monitoring-auditing-and-session-management)](#monitoring-auditing-and-session-management)

[6. Break glass and emergency access
[7](#break-glass-and-emergency-access)](#break-glass-and-emergency-access)

[7. User and administrator responsibilities
[7](#user-and-administrator-responsibilities)](#user-and-administrator-responsibilities)

[8. Regulatory requirements
[7](#regulatory-requirements)](#regulatory-requirements)

[9. Consequences of non-compliance
[7](#consequences-of-non-compliance)](#consequences-of-non-compliance)

[Revisions Record Sheet
[8](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [8](#approvals)](#approvals)

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

###  {#section .Heading-3_Green}

### General Information {#general-information .Heading-3_Green}

### Document Objective {#document-objective .Heading-3_Green}

This Privileged Access Rights Policy establishes requirements for
managing privileged access rights at Community Fibre Limited to protect
critical information assets and infrastructure. It supports the
overarching [ISP034-Access Control
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP034-Access%20Control%20Policy.pdf?csf=1&web=1&e=nmI4PN)
by detailing controls for privileged access, while complementing other
supporting policies such as the [ISP011 -- Information Access Rights
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP012-Identity%20Management%20Policy.pdf?csf=1&web=1&e=12e4Yd),
[ISP040-Password Management
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP040-Password%20Management%20Policy.pdf?csf=1&web=1&e=9V8myG),
[ISP012-Identity Management
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP012-Identity%20Management%20Policy.pdf?csf=1&web=1&e=4xDgyR),
and [ISP014-User Registration
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP014-User%20Registration%20Policy.pdf?csf=1&web=1&e=SQXi18).

This policy aligns with NCSC guidance on privileged access management
and secure privileged access workstations ([Use privileged access
management -
NCSC.GOV.UK](https://www.ncsc.gov.uk/collection/secure-system-administration/use-privileged-access-management)),
and addresses regulatory requirements, including The Electronic
Communications (Security Measures) Regulations 2022.

**This document meets the following clauses:**

- ISO/IEC 27001:2022 -- A.5.16: Identity management

- The Electronic Communications (Security Measures) Regulations 2022 --
  Regulation 8 (Access controls for security-critical functions) and
  Code of Practice (3.1--3.7)

### Policy {#policy .Heading-3_Green}

### Scope and principles {#scope-and-principles .Heading-3_Green}

This policy applies to all privileged access rights, including
administrative, root, or elevated privileges used to manage business
systems, network appliances, network management infrastructure,
applications, and other information assets at Community Fibre. It covers
employees, contractors, third parties, and system accounts with
privileged capabilities, throughout the asset lifecycle.

Key principles:

![A white logo with circles and dots AI-generated content may be
incorrect.](media/image1.png){width="0.6666666666666666in"
height="0.6666666666666666in"}

- Grant only necessary privileges, separate from standard user
  activities.

- Continuously verify and validate privileged access.

- Use control proportionate to asset sensitivity ([ISP037-Information
  Classification and Handling
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP037-Information%20Classification%20and%20Handling%20Policy.pdf?csf=1&web=1&e=8hmq6A)).

- Provide temporary, task-specific privileges. (Just-In-Time (JIT) and
  Just-Enough-Administration (JEA))

- Use dedicated devices and monitoring to isolate high-risk activities.

- Log, audit, and review all privileged actions.

Privileged access is managed by Security Operations, Network Technology
and IT Service Desk, with oversight from the ISMS Board.

### Identification and classification of privileged access {#identification-and-classification-of-privileged-access .Heading-3_Green}

- Privileged access is identified through risk assessments and
  classifying and grouping administration into tiers:

  - **Tier 0 -** root of trust that all other administration relies
    upon, examples include:

    - Root domain administrators that can create additional, highly
      privileged accounts.

    - The root account in a cloud service, that manages the privileges
      of all other accounts.

    - Infrastructure that is used to generate cryptographic material
      which other components rely upon.

  - **Tier 1** - infrastructure used to carry out highly privileged
    functions on critical systems, but more constrained than tier 0,
    examples include:

    - Administrators of a critical database used to store a large amount
      of sensitive information.

    - Infrastructure that is used for network management or oversight
      functions.

    - The ability to control and manage critical services in a cloud
      environment.

  - **Tier 2** - infrastructure used to carry out privileged functions,
    but over a small number of components, impact of compromise is
    limited, require extra effort from attackers needing full compromise
    to succeed, example include:

    - Administrator access on an important business support application.

    - Root level access on a front-end web server that forms part of a
      wider cloud architecture.

    - Administration of a dashboard responsible for monitoring network
      infrastructure.

  - **Tier 3** - infrastructure that allows a constrained set of
    functions over a single or small number of components, impact of
    compromise in this tier not catastrophic to business operations,
    examples include:

    - First line support staff issuing a password reset.

    - The ability to trigger a predefined action in a cloud environment,
      such as promotion of new feature code into a live environment.

    - Modification of values in systems that are bound by limits set by
      a component or administrator in a lower tier.

### Granting and managing privileged access rights {#granting-and-managing-privileged-access-rights .Heading-3_Green}

- Requests for privileged access must be submitted via IT Service Desk,
  with explicit approval from the asset owner and either Network
  Technology management or Security Operations, based on business need
  and risk.

- Use RBAC integrated with Identity Providers (per ISP041) for automated
  provisioning; apply JIT/JEA for temporary elevations.

- Privileged accounts must be separate from standard user accounts, no
  reuse of credentials across systems.

- Passwords and secrets must follow [ISP040-Password Management
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP040-Password%20Management%20Policy.pdf?csf=1&web=1&e=4p5kNZ),
  stored in secure vaults (e.g., Bitwarden), with automated rotation
  (e.g., 30 days for Tier 0).

- MFA is mandatory for all privileged access; prohibit hardcoded
  credentials.

- Reviews occur every 6 months or upon changes, revoking unnecessary
  privileges immediately.

### Privileged access workstations (PAWs) {#privileged-access-workstations-paws .Heading-3_Green}

- High-risk privileged access (e.g., Tier 0/1) must use dedicated,
  hardened physical PAWs isolated from general productivity tasks.

- Must be implemented in alignment with NCSC\'s principles for PAWs:

1.  Periodic risk assessments to define scope, including which roles and
    systems that require PAWs.

2.  Must be practical and support administrative tasks without
    compromising security.

3.  Must be built on trusted, verified hardware and software baselines,
    supplied via trusted suppliers, support and use secure boot
    processes, standardise on hardened operating systems (e.g., Windows
    with latest security features) and verified through integrity checks
    and regular patching.

4.  Must use automated provisioning and configuration, defined as code.
    PAW administrators must be limited to authorised staff, no user
    outside of this group should be able to make changes. PAW controls
    must only be managed from another PAW device.

5.  PAW devices should be configured to meet administrative access needs
    only; corporate applications must be blocked. Access to external
    services must be restricted to the services that are essential for
    it to operate. All communication should be established outbound from
    the PAW to the systems and devices it manages. Any unnecessary
    application or functionality must be disabled or removed.

6.  If local virtualisation is used, connectivity between the guest and
    host OS must be limited. Virtualisation features such as clipboard
    and file sharing should be limited. The need for local admin rights
    on the PAW should be limited and designed away, leveraging
    virtualisation if needed.

7.  Monitoring must provide visibility over both the systems that
    support and configure the PAW devices, as well as the PAW's.
    Additional monitoring of privileged accounts must be in place to
    detect anomalies.

8.  Data flows to and from the PAW environment must be controlled,
    access to corporate data file-sharing services must be restricted.
    Transfers must be limited to approved data types, complex data types
    like Word and PDF files should not be used. Audit trails should be
    produced for all data entering and leaving PAW environments, and
    data must be inspected for malicious content.

- Privileged access provided to third-party suppliers requires a
  physical PAW device which complies with Community Fibre's polices on
  PAWs.

- Third-party access must be authenticated through Community Fibre's
  identity provider services.

### Monitoring, auditing, and session management {#monitoring-auditing-and-session-management .Heading-3_Green}

- All privileged sessions must be controlled, monitored, and recorded
  (e.g., video/keystrokes for high-risk), isolated from user
  workstations.

- Logs linked to unique identities [ISP012-Identity Management
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP012-Identity%20Management%20Policy.pdf?csf=1&web=1&e=4xDgyR),
  analysed for anomalies; enable session replay for investigations.

- Protective monitoring detects compromises; audit logs reviewed
  regularly.

### Break glass and emergency access {#break-glass-and-emergency-access .Heading-3_Green}

- Critical systems must have at least two break glass accounts,
  independent of main authentication, with passwords changed after use.

- Usage triggers notifications, full audits, and incident response.

### User and administrator responsibilities {#user-and-administrator-responsibilities .Heading-3_Green}

- Privileged users must use separate accounts for elevated tasks, report
  anomalies, and avoid untrusted devices.

- Complete specialised training on privileged access risks and controls
  annually.

### Regulatory requirements {#regulatory-requirements .Heading-3_Green}

- Privileged access to security-critical functions uses unique
  credentials, MFA, PAWs, and segregation (Reg 8(2) (b-c), 8(5)
  \[**2**\]).

- Remote access via jump boxes only (Reg 4(5) \[**2**\]); assess
  third-party risks (Reg 11(b) \[**2**\]).

- Logging and monitoring align with Code of Practice (para 3.4-3.7
  \[**2**\]).

### Consequences of non-compliance {#consequences-of-non-compliance .Heading-3_Green}

Any non-compliance with or breach of this policy may lead to
investigation and action in line with the organisational Disciplinary
Policy ([Community Fibre - Employee Handbook 2023 -
v3.pdf](https://communityfibre.sharepoint.com/Shared%20Documents/Forms/AllItems.aspx?id=%2FShared%20Documents%2FInfo%20%26%20HR%2FCommunity%20Fibre%20%2D%20Employee%20Handbook%202023%20%2D%20v3%20%281%29%2Epdf&viewid=e786a8f6%2D73e3%2D49ca%2D945e%2D7071d07d760b&parent=%2FShared%20Documents%2FInfo%20%26%20HR)).

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

  ----------------------------------------------------------------------------
  Version   Date         Author         Changes
  --------- ------------ -------------- --------------------------------------
  0.1       12/08/2025   Head of        Initial Draft as supporting policy to
                         Security       ISP034.

  1.0       03/10/2025   Head of        Major version updates, release for
                         Security       approval

                                        

                                        

                                        
  ----------------------------------------------------------------------------

### Approvals {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     03/10/2025     1.0       [CISP-101708](https://communityfibre.atlassian.net/browse/CISP-101708)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
