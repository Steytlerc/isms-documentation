**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISP016**

**Threat Intelligence Policy**

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

[Scope [3](#scope)](#scope)

[Roles and Responsibilities
[3](#roles-and-responsibilities)](#roles-and-responsibilities)

[Procedure [4](#procedure)](#procedure)

[1. Gathering intelligence
[4](#gathering-intelligence)](#gathering-intelligence)

[2. Processing and analysis
[4](#processing-and-analysis)](#processing-and-analysis)

[Revisions Record Sheet
[5](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [5](#approvals)](#approvals)

### General Information {#general-information .Heading-3_Green}

### Document Objective {#document-objective .Heading-3_Purple}

The purpose of this policy is to establish a systematic approach for
collecting, processing, analyzing, and disseminating threat intelligence
to proactively identify and mitigate emerging information security
threats and vulnerabilities. This supports the Community Fibre's risk
management, incident response, and overall security posture.

**This document meets the following clauses:**

- Information Security Management System BS EN ISO/IEC 27002:2022 --
  A.5.7 Threat intelligence

### Scope {#scope .Heading-3_Purple}

This policy applies to all employees, contractors and suppliers of
Community Fibre who are involved in information security activities. It
covers internal and external sources relevant to Community Fibre\'s
assets in cloud (e.g., AWS, Azure, GCP) and operational environments.

### Roles and Responsibilities {#roles-and-responsibilities .Heading-3_Green}

1.  The Community Fibre Security Operations team will oversee the threat
    intelligence program, monitor compliance, report to Executive
    Management, and integrate findings into the Risk Treatment Plan
    (RTP) and vulnerability management processes (per [ISP036-Management
    of technical
    vulnerabilities](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP036-Management%20of%20technical%20vulnerabilities.pdf?csf=1&web=1&e=BRnEHr))

2.  Community Fibre Technology and Network Operations and Network
    Technology teams are responsible for implementing mitigations based
    on analysed intelligence.

3.  The managed SOC service team will provide threat intelligence to
    their analytics platform by using subscriptions and industry
    collaborations and share any relevant intelligence with the
    Community Fibre Security Operations team as appropriate.

4.  The Security Operations team will subscribe to and stay updated with
    reputable external sources (e.g., NCSC advisories, Microsoft threat
    intelligence, industry publications, etc.)

### Procedure {#procedure .Heading-3_Green}

### Gathering intelligence

1.  Continuous monitoring with daily reviews of high-priority sources;
    weekly for others; monthly integration of Orange Moldova reports.

2.  **Internal sources**: Microsoft Defender Threat Intelligence and
    analytics: Integrated feeds from Defender XDR for triage, incident
    response, and vulnerability management data sets. Threat detection
    alerts and intelligence from AWS environments, including ML-based
    anomaly detection and integrated threat feeds.

3.  **External sources**: Vulnerability scans and threat reports;
    managed SOC industry collaborations and subscriptions; public feeds
    (CISA, NIST CVE, NCSC, ENISA).

4.  Sources must be credible and relevant (e.g., cloud threats for AWS
    or network exploit information from Palo Alto) and aligned with
    assessed security risks. Prioritise automated feeds (e.g., APIs from
    Defender and GuardDuty) for proactive threat hunting (Code of
    Practice Sec 5.21-5.23).

### Processing and analysis

1.  Processing of feeds will be automated as far as possible for
    relevance using predefined criteria in integrated tools (e.g., CVSS
    score \>7, matches organizational assets like AWS workloads).

2.  Enrichment will be automated where possible using internal data
    across trusted sources (e.g., cross-reference GuardDuty alerts with
    Microsoft Defender logs).

3.  Findings will be mapped to the ISMS risk register or used to update
    existing risks if new threats elevate likelihood/impact (Regulation
    3(3)(a)); inform vulnerability prioritization in [ISP036-Management
    of technical
    vulnerabilities](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP036-Management%20of%20technical%20vulnerabilities.pdf?csf=1&web=1&e=BRnEHr).

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

  ----------------------------------------------------------------------------
  Version   Date         Author        Changes
  --------- ------------ ------------- ---------------------------------------
  0.1       05/08/2025   Head of       Initial Draft
                         Security      

  1.0       03/10/2025   Head of       Major version update, released for
                         Security      approval

                                       

                                       

                                       
  ----------------------------------------------------------------------------

### Approvals {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     07/10/2025     1.0       [CISP-101698](https://communityfibre.atlassian.net/browse/CISP-101698)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
