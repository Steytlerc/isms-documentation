**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISP040**

**Password Management Policy**

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

[2. User password management
[4](#user-password-management)](#user-password-management)

[3. Privileged and administrative passwords
[4](#privileged-and-administrative-passwords)](#privileged-and-administrative-passwords)

[4. System and service account passwords
[4](#system-and-service-account-passwords)](#system-and-service-account-passwords)

[5. Multi-factor authentication (MFA)
[5](#multi-factor-authentication-mfa)](#multi-factor-authentication-mfa)

[6. Password storage and transmission
[5](#password-storage-and-transmission)](#password-storage-and-transmission)

[7. Default passwords [5](#default-passwords)](#default-passwords)

[8. Monitoring and compliance
[6](#monitoring-and-compliance)](#monitoring-and-compliance)

[9. User responsibilities
[6](#user-responsibilities)](#user-responsibilities)

[10. Suspected or actual password compromise
[6](#suspected-or-actual-password-compromise)](#suspected-or-actual-password-compromise)

[11. Consequences of Non-Compliance
[6](#consequences-of-non-compliance)](#consequences-of-non-compliance)

[Revisions Record Sheet
[7](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [7](#approvals)](#approvals)

### General Information {#general-information .Heading-3_Green}

### Document Objective {#document-objective .Heading-3_Purple}

The purpose of this document is to establish best practices and
accountability for the safeguarding of authentication information.
Guidance provided by the UK's National Cyber Security Centre (NCSC) was
used to create this document, we recognise that password use, and
management has changed in recent years and have taken this into account.
This policy supports the [Access Control
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP034-Access%20Control%20Policy.pdf?csf=1&web=1&e=9qEoSf)
and is referenced in related policies such as the [Information Access
Rights
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/CFL-006%20-%20Process%20Document%20-%20Change%20Management%20-%20Copy.pdf?csf=1&web=1&e=SJdfsH)
and [Privileged Access Rights
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISD001-Operational%20Security%20Framework.pdf?csf=1&web=1&e=IJq2gU).

**This document meets the following clauses:**

- Information Security Management System ISO/IEC 27001:2022 -- A.5.17:
  Authentication information

- Telecoms Security Act 2021 -- Regulation 8(2) (d-e): Avoidance of
  default credentials and ensuring unique, non-guessable authentication

### Policy {#policy .Heading-3_Green}

### Scope and principles {#scope-and-principles .Heading-3_Purple}

This policy applies to all employees, contractors, third parties, and
systems using passwords or secret authentication information to access
Community Fibre\'s information assets, networks, systems, and services.
It covers user accounts, privileged accounts, service accounts, and
devices throughout their lifecycle.

Key principles:

- Password policies should be memorable and easy to use to encourage
  secure behaviour.

- Password controls must be proportionate to the sensitivity of assets
  they protect ([Information Classification and Handling
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP037-Information%20Classification%20and%20Handling%20Policy.pdf?csf=1&web=1&e=4olo9d)).

- Passwords must be combined with MFA and other controls.

- Passwords must only be changed on suspicion of compromise.

- Common or guessable passwords shall be restricted where possible.

- Tools for secure password storage must be approved.

### User password management {#user-password-management .Heading-3_Purple}

- Passwords must be unique, non-guessable, and at least 8 characters
  long. Use techniques like \"three random words\" (e.g.,
  \"applenemobiro\") to make them memorable but hard to crack.

- Avoid complexity requirements (e.g., mandatory special characters)
  unless risk-assessed as necessary for high-sensitivity assets
  (Strictly Confidential per [Information Classification and Handling
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP037-Information%20Classification%20and%20Handling%20Policy.pdf?csf=1&web=1&e=4olo9d)).

- Systems must enforce blacklisting of common passwords (e.g.,
  \"password123\", lists from known breaches).

- Passwords must not be reused across accounts, especially between
  personal and work systems.

- Temporary passwords must be changed immediately upon first login.

- Password changes are required only if compromised or suspected, no
  forced periodic changes.

### Privileged and administrative passwords {#privileged-and-administrative-passwords .Heading-3_Purple}

- Privileged accounts (e.g., admin, root) must use passwords of at least
  20 characters, unique per account, and not shared.

- Separate accounts and passwords for administrative and standard user
  roles; privileged accounts shall not be used for routine tasks (e.g.,
  email, internet browsing).

- Access to privileged passwords must be controlled via an approved
  password vault (e.g., Bitwarden); logging and auditing shall be
  enabled on systems where these accounts are used.

- For security-critical functions (e.g., network infrastructure),
  passwords shall be unique, non-guessable, and protected by MFA and
  privileged access workstations (PAWs) per the [Privileged Access
  Rights
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISD001-Operational%20Security%20Framework.pdf?csf=1&web=1&e=IJq2gU).

### System and service account passwords {#system-and-service-account-passwords .Heading-3_Purple}

- Service accounts shall use long, randomly generated passwords (at
  least 20 characters) stored securely in a password vault.

- Rotate passwords for service accounts annually or upon suspicion of
  compromise; automate rotation where possible.

- Avoid embedded hardcoded passwords in code, scripts or configurations;
  use secure vaults or API keys where possible.

- Responsibility for review and audit of service accounts and passwords
  is with associated system administrative function (i.e. DevOps) and
  shall be conducted every 6 months.

### Multi-factor authentication (MFA) {#multi-factor-authentication-mfa .Heading-3_Purple}

- MFA must be enabled for all remote access, privileged accounts, and
  access to Confidential or Strictly Confidential information (per
  [Information Classification and Handling
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP037-Information%20Classification%20and%20Handling%20Policy.pdf?csf=1&web=1&e=4olo9d)).

- Where MFA is not feasible, compensating controls (e.g., longer
  passwords, monitoring) must be approved by Security Operations.

- Users must use hardware tokens, authenticator apps, or biometrics;
  SMS-based MFA should be avoided where possible due to risks.

### Password storage and transmission {#password-storage-and-transmission .Heading-3_Purple}

- Passwords must be hashed with strong algorithms (e.g., bcrypt, Argon2)
  and never stored in plain text.

- Transmission must use encrypted channels (e.g., HTTPS, SSH).

- Approved password managers (e.g., Bitwarden) must be used for storage;
  request installation via IT Service Desk.
  (<itsupport@communityfibre.co.uk>)

- Physical storage of passwords (e.g., written down) is discouraged but,
  if necessary, must be in secure locations (e.g., locked cabinets).

### Default passwords {#default-passwords .Heading-3_Purple}

- All default passwords on devices, software, and systems must be
  changed before deployment.

- Regular scans must be conducted to identify and remediate unchanged
  defaults, prioritising critical infrastructure (e.g., routers,
  firewalls).

- Assume default credentials are publicly known and treat them as
  compromised.

**\**

### Monitoring and compliance {#monitoring-and-compliance .Heading-3_Purple}

- Systems must implement account lockout after 5 failed attempts (lock
  for 10 minutes) and throttling to prevent brute-force attacks.

- All password-related events (e.g., changes, failures) must be logged
  and monitored by the SOC and Security Operations.

- Password policies will be reviewed annually or following significant
  changes (e.g., new threats, regulations).

### User responsibilities {#user-responsibilities .Heading-3_Purple}

- Never share passwords, even with IT staff.

- Report suspected compromises immediately to Security Operations.

- Use password managers for complex passwords.

- Set screen locks on devices with PINs, biometrics, or strong
  passwords.

- Complete annual training on password best practices.

### Suspected or actual password compromise {#suspected-or-actual-password-compromise .Heading-3_Purple}

> If you suspect that your password has been compromised you must
> immediately report this to the **IT Service Desk**
> (<itsupport@communityfibre.co.uk>) and/or **Security Operations**
> (<security@communityfibre.co.uk>).

### Consequences of Non-Compliance {#consequences-of-non-compliance .Heading-3_Purple}

> Any non-compliance with or breach of this policy may lead to
> investigation and action in line with the organisational Disciplinary
> Policy ([Community Fibre - Employee Handbook 2023 -
> v3](https://communityfibre.sharepoint.com/:b:/r/Shared%20Documents/Info%20%26%20HR/Community%20Fibre%20-%20Employee%20Handbook%202023%20-%20v3%20(1).pdf#page=26)).

**\**

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

  ----------------------------------------------------------------------------
  Version   Date         Author         Changes
  --------- ------------ -------------- --------------------------------------
  0.1       17/02/2021   ISO            Initial Draft

  1.0       23/09/2022   ISO            Final review, sent for approval

  1.1       07/11/2023   Head of        Document template update
                         Security       

  1.2       17/09/2024   Head of        Standard version update, TOC added, no
                         Security       other changes

  2.0       12/08/2025   Head of        Major update to align with NCSC
                         Security       guidance, ISO 27001:2022, and Telecoms
                                        Security Act 2021; expanded sections
                                        for comprehensiveness as supporting
                                        policy.
  ----------------------------------------------------------------------------

### Approvals {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     07/10/2025     2.0       [CISP-100769](https://communityfibre.atlassian.net/browse/CISP-100769)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
