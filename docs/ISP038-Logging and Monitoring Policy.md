**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISP038**

**Logging and Monitoring Policy**

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

[Logging and monitoring
[3](#logging-and-monitoring)](#logging-and-monitoring)

[2.1 Event logging [4](#event-logging)](#event-logging)

[2.2 Protection of log information
[5](#protection-of-log-information)](#protection-of-log-information)

[2.3 Protection of tools enabling monitoring or analysis
[5](#protection-of-tools-enabling-monitoring-or-analysis)](#protection-of-tools-enabling-monitoring-or-analysis)

[2.4 Administrator and operator logs
[6](#administrator-and-operator-logs)](#administrator-and-operator-logs)

[2.5 Clock synchronisation
[6](#clock-synchronisation)](#clock-synchronisation)

[Revisions Record Sheet
[7](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [7](#approvals)](#approvals)

### General Information {#general-information .Heading-3_Green}

### Document Objective {#document-objective .Heading-3_Purple}

This document sets the Logging and Monitoring policy for systems within
scope of the Information Security Management System (ISMS).

**This document meets the following clauses:**

- Information Security Management System BS EN ISO/IEC 27001:2022 --
  A.8.15 Logging, A. 8.16 Monitoring activities, A.8.17 Clock
  synchronisation

- NCSC Cyber Assessment Framework (CAF) v3.1 - Objective C: Detecting
  Cyber Security Events

This document also addresses requirements for the Electronic
Communications (Security Measures) Regulations 2022, particularly
Regulations 5 and 6, which require protection of monitoring tools,
monitoring for anomalous activity in security-critical functions,
investigation of anomalies, record-keeping, data retention for at least
13 months, and prevention of restrictions on monitoring. Guidance from
the Telecommunications Security Code of Practice (December 2022) has
been incorporated, including the use of automated tools where possible
and skilled resources for analysis.

### Logging and monitoring {#logging-and-monitoring .Heading-3_Green}

Community Fibre Limited uses a combination of third-party SaaS, PaaS,
IaaS type services, including the core network. Log collection and
management is therefore complex and realistically only achievable by
using a combination of services for log management and reporting.

Asure Sentinel SIEM is used to collect and store log data from AWS
GuardDuty, Entra ID, Microsoft Defender, Microsoft 365 services, Google
Cloud Platform and core network components (e.g., routers, switches,
firewalls, and security-critical functions). Data sources are selected
to ensure comprehensive coverage for detecting security events affecting
essential functions, including host-based monitoring, network boundary
traffic (e.g., IP connections as a minimum), user activities, and
Indicators of Compromise (IoCs) such as malicious command and control
signatures (per CAF C1.a Monitoring Coverage).

Monitoring is supported by the managed SOC service provider ANS, who has
access to the Sentinel instance via Microsoft Sentinel Lighthouse. ANS
runs their own analytics on event data and generates alerts when
anomalies are detected. ANS access is restricted via role-based access
control (RBAC) and is limited to authorised personnel based in the UK.

### 2.1 Event logging {#event-logging .Heading-3_Purple}

1.  Event logs recording user access and actions/activities, exceptions,
    faults, and information security events shall be produced and kept
    for a minimum duration of 13 months for all information assets,
    including the core network.

2.  System administrators are prohibited from erasing or de-activating
    logs of their own activities.

3.  Audit logs and the audit log reports are classified as Strictly
    Confidential information and must be handled in line with the
    requirements of this ISMS for handling such information.

4.  Monitoring logs/reports are reviewed continuously using automated
    means where possible. Any evidence of system misuse or anomalous
    activity is reported to the Security Operations team, who
    investigates further. Anomalous activity alerts generated by ANS are
    prioritised for investigation, with correlations across data sources
    to identify patterns.

5.  All systems and information assets being monitored must provide
    real-time alerting, including immediate alerts for all manual
    amendments to security-critical functions and automated generation
    of alerts for potential security incidents based on predefined rules
    and thresholds.

6.  A record shall be maintained of all access to security-critical
    functions, including the persons obtaining access.

7.  All cases where a person's access to security-critical functions
    exceeds their security permission shall be identified and recorded.

8.  Activity relating to security-critical functions shall be analysed
    promptly to identify any anomalous activity. Analysis may utilise
    ANS-provided analytics and include impact assessment on essential
    functions.

9.  The type, location, software and hardware information, and
    identifying information of equipment supplied by Community Fibre
    which is used or intended to be used as part of the PECN/PECS shall
    be recorded. ([ISP045-Asset Management
    Policy.pdf](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/CFL-006%20-%20Process%20Document%20-%20Change%20Management%20-%20Copy.pdf?csf=1&web=1&e=iN4mb2))

10. Proactive security event discovery shall be conducted through
    regular threat hunting, vulnerability scanning, and analysis of
    monitoring data to detect hidden threats before they impact
    essential functions.

### 2.2 Protection of log information {#protection-of-log-information .Heading-3_Purple}

1.  Event logs must be protected to deny removal or modification by
    unauthorised persons.

2.  Event logs and logging servers are restricted to authorised IT,
    Security and Network Technology staff only, including authorised ANS
    personnel. Logs are encrypted both in transit and at rest.

3.  Rules that only permit deletion and modification of these logs by
    authorised persons shall be applied. Audit logs that track user
    activities, providing a trail of who accessed the logs and what
    actions were performed shall be maintained. Log data analysis is
    performed on copies, keeping the master copy unaltered.

4.  Disabling audit logs or tampering with audit log information is
    treated as gross misconduct and the disciplinary policy may be
    invoked resulting in immediate dismissal.

5.  Measures shall be taken to prevent activities that would restrict
    monitoring and analysis requirements.

### 2.3 Protection of tools enabling monitoring or analysis {#protection-of-tools-enabling-monitoring-or-analysis .Heading-3_Purple}

1.  If monitoring or analysis tools are stored on equipment located
    outside the United Kingdom, measures shall be taken to identify and
    reduce the risks of security compromises occurring as a result.
    These risks shall be documented in the annual risk assessment.

2.  Monitoring or analysis tools shall not be capable of being accessed
    from countries listed in the Schedule to the Regulations (Iran,
    North Korea, People\'s Republic of China, Russia) and shall not be
    stored on equipment located in those countries.

3.  ANS monitoring tools and analytics are hosted within UK-based
    infrastructure, ensuring compliance with location restrictions.

### 2.4 Administrator and operator logs {#administrator-and-operator-logs .Heading-3_Purple}

1.  All Administrator and operator actions/activities shall be logged
    regardless of the privileges that they have on the systems and be
    made available for reporting and audits. This includes auditing user
    activities related to essential functions to detect policy
    violations or suspicious behaviour.

### 2.5 Clock synchronisation {#clock-synchronisation .Heading-3_Purple}

1.  All information systems that produce event and audit logs must
    record data in UTC.

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

  ----------------------------------------------------------------------------
  Version   Date         Author        Changes
  --------- ------------ ------------- ---------------------------------------
  0.1       12/03/2021   ISO           Initial Draft

  1.0       22/03/2022   ISO           Final review, major version number

  1.1       23/09/2022   ISO           Business address update

  1.2       07/11/2023   Head of       Document template update, minor update
                         Security      to log sources (remove Solarwinds)

  1.3       17/09/2024   Head of       Standard version update, no other
                         Security      changes

  1.4       15/08/2025   Head of       Standard version update, references to
                         Security      ESM, COP and CAF requirements added,
                                       ANS references added. Log retention
                                       changes from 90 days to 13 months.
                                       Administrator and operator logs
                                       requirements added.
  ----------------------------------------------------------------------------

### Approvals {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     17/09/2025     1.4       [CISP-101386](https://communityfibre.atlassian.net/browse/CISP-101386)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
