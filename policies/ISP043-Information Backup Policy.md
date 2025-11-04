**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISP043**

**Information Backup Policy**

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

# Table of Contents {#table-of-contents .TOC-Heading}

[Roles and Responsibilities
[3](#roles-and-responsibilities)](#roles-and-responsibilities)

[General Information [3](#general-information)](#general-information)

[Scope [3](#scope)](#scope)

[Purpose [4](#purpose)](#purpose)

[Data classification [4](#data-classification)](#data-classification)

[Backup Schedule [4](#backup-schedule)](#backup-schedule)

[Backup Storage [5](#backup-storage)](#backup-storage)

[Backup Testing [5](#backup-testing)](#backup-testing)

[Recovery point and time objectives
[5](#recovery-point-and-time-objectives)](#recovery-point-and-time-objectives)

[Security [6](#security)](#security)

[Revisions Record Sheet
[7](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [7](#approvals)](#approvals)

### Roles and Responsibilities {#roles-and-responsibilities .Heading-3_Green}

  -----------------------------------------------------------------------
  Term            Description
  --------------- -------------------------------------------------------
  ISMS Board      Approve the policy, ensure resources for
                  implementation, and review compliance annually.

  Head of         Compliance monitoring, and annual review.
  Security        

  DevOps          Responsible for overseeing the business backup
                  processes, ensuring backups are performed according to
                  schedule, managing backup storage, and coordinating
                  data restoration efforts for IT systems.

  Technology      Assists in implementing and maintaining backup systems,
  Department      provides technical support for backup procedures, and
                  ensures the security of backup storage across all
                  scopes.

  Network         Responsible for backups of operational network assets,
  Operations      including configurations and logs, and supporting
                  restoration to maintain network resilience.

  Employees and   Responsible for ensuring that their data is backed up
  contractors     as per the policy, particularly if they handle critical
                  information. Employees must report any issues with
                  backups or data loss to the relevant department.
  -----------------------------------------------------------------------

#### 

### General Information {#general-information .Heading-3_Green}

> This backup policy is designed to ensure the protection and
> availability of critical data and essential functions for Community
> Fibre. It establishes guidelines and procedures for backing up data,
> storing backups securely, and restoring data in the event of loss or
> corruption. By implementing this policy, Community Fibre aims to
> minimise the risk of data loss, maintain business continuity, and
> safeguard sensitive information.

#### This document meets the following clauses:

- Information Security Management System BS EN ISO/IEC 27001:2022 --
  A.8.13: Information backup

### Scope {#scope .Heading-3_Green}

> This policy applies to all employees, contractors, and third parties
> who have access to Community Fibre\'s data and information systems. It
> covers all data and essential functions deemed critical to the
> organisation\'s operations, including but not limited to core network
> functions, customer information, financial records, intellectual
> property, network configurations, operational logs, and data related
> to security critical functions. The policy applies to data stored on
> subscription model services (SaaS), cloud infrastructure (AWS, Azure),
> physical devices, servers, databases, workstations, routers, switches,
> management systems, and other information systems managed by IT,
> Network Technology and Network Operations teams.

### Purpose {#purpose .Heading-3_Green}

The purpose of this backup policy is to safeguard Community Fibre\'s
data against loss, corruption, or unauthorised access. By establishing
clear procedures for data backup and restoration, this policy ensures
that critical information is available and secure, supporting business
continuity and compliance with relevant regulations.

### Data classification {#data-classification .Heading-3_Green}

Data is classified based on its importance to business operations and
regulatory definitions:

- **Strictly confidential data**: Essential for business operations and
  includes sensitive data as per regulations (e.g., data controlling
  security-critical functions, customer databases, financial records,
  intellectual property). Requires frequent backups.

- **Confidential data**: Valuable but not critical (e.g., internal
  communications, project files,). Backed up less frequently.

- **Non-essential data**: Easily recreated or not necessary for
  operations (e.g., temporary files). May not require regular backups.

### Backup Schedule {#backup-schedule .Heading-3_Green}

- **Strictly confidential data (critical):** Full backup daily, full
  backup monthly, full annual backup, with online and offline copies
  replaced with reasonable frequency appropriate to the risk.

- **Confidential data (important)**: Full backup daily, full backup
  monthly, full annual backup.

- **Public (non-essential data)**: Backed up as needed or upon request.

**Note**: Backup procedures may vary depending on the type of system or
data being backed up. Specific procedures for different systems are
detailed in
[AWS+Backup](https://communityfibre.atlassian.net/wiki/spaces/DSCC/pages/658702337/AWS+Backup)
and
[Rubrik](https://communityfibre.my.rubrik.com/inventory_hierarchy/all).
Backups must include information necessary to maintain normal operation
of the network/service.

### Backup Storage {#backup-storage .Heading-3_Green}

Backups are stored in multiple locations to ensure redundancy, disaster
recovery:

- **Cloud**: For additional redundancy and accessibility, using a secure
  cloud storage provider. Cloud-based backup storage must be duplicated
  across availability zones.

- **On-Site**: For quick access and restoration (e.g., local servers or
  storage devices).

- **Off-Site**: For disaster recovery, stored in a secure,
  geographically separate location within the UK.

- **Offline Copies**: Proportionate offline copies (not exposed to
  network signals) must be maintained for critical information to enable
  recovery without risk of further compromise.

Retention periods are determined by system and data criticality and
recovery requirements.

- **AWS**: Full backups are retained for 35 days.

- **M365**: Full backups are retained for 30 days. Monthly backups are
  retained for 12 months. Annual backups are retained for 3 years.

All copies of information necessary for normal operation must be
retained within the UK.

### Backup Testing {#backup-testing .Heading-3_Green}

- Regular testing is conducted to ensure backups can be restored
  successfully, including verification of online and offline copies.

- Testing is performed quarterly, and results are documented.

- Any issues identified during testing must be addressed promptly to
  maintain backup integrity and resilience.

### Recovery point and time objectives {#recovery-point-and-time-objectives .Heading-3_Green}

Recovery Point Objective (RPO) and Recovery Time Objective (RTO) are
defined to ensure timely recovery from security compromises or
disruptions, which requires preparation for remediation and recovery,
including maintaining backups and procedures to replace damaged
information without further risk.

**RPO**: The maximum acceptable data loss period, determined by backup
frequency and system criticality.

- **Strictly confidential (critical) systems/data**: RPO ≤ 24 hours
  (achieved through daily full backups for security critical functions).

- **Confidential (important) systems/data**: RPO ≤ 24 hours (achieved
  through daily full backups).

- **Non-essential systems/data**: RPO ≤ 24 hours (aligned with daily
  backups).

**RTO**: The maximum acceptable time to restore operations, based on
assessed security risks and business impact.

- **Strictly confidential (critical) systems/data**: RTO ≤ 2 hours

- **Confidential (important) systems/data**: RTO ≤ 24 hours.

- **Non-essential systems/data**: RTO ≤ 48 hours.

These objectives must be reviewed annually or following risk assessments
and prioritised accordingly. Procedures must ensure no further security
compromise during recovery, using offline copies where proportionate.

### Security {#security .Heading-3_Green}

- All backups must be encrypted both in transit and at rest using
  industry-standard encryption methods.

- Immutable backups must be used for data which is critical to business
  operations. Immutability is defined as configuration which provides
  read-only/write many storages, and protected from deletion, even by
  highest level permissions or authorised personnel or backup vendor.

- Access to backups is restricted to authorised personnel only, in line
  with [ISP011-Information Access Rights
  Policy.pdf](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP011-Information%20Access%20Rights%20Policy.pdf?csf=1&web=1&e=mBG2XV)

- Physical backup media (if used) must be stored in a secure, locked
  facility.

- Offline backups must be digitally disconnected when not in use to
  prevent exposure.

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

  --------------------------------------------------------------------------
  Version   Date         Author     Changes
  --------- ------------ ---------- ----------------------------------------
  0.1       21/01/2025   Head of    Initial Draft 
                         Security   

  0.2       15/03/2025   Head of    Recovery point and time objectives added
                         Security   

  1.0       16/03/2025   Head of    Update to major version
                         Security   

  1.1       22/08/2025   Head of    Added section for backup testing
                         Security   
  --------------------------------------------------------------------------

### Approvals  {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name          Role    Signature      Date         Version    Ticket no. 
  ------------- ------- -------------- ------------ ---------- ------------------------------------------------------------------------
  Chris         CIO                    03/10/2025   1.1        [CISP-101478](https://communityfibre.atlassian.net/browse/CISP-101478)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
