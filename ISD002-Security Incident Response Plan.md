> **INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISD002**

**Security Incident Response Plan**

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

[General Information [4](#general-information)](#general-information)

[1. Acronyms [4](#acronyms)](#acronyms)

[2. Glossary [4](#glossary)](#glossary)

[3. References and Related Documents
[6](#references-and-related-documents)](#references-and-related-documents)

[Introduction [7](#introduction)](#introduction)

[1. Overview [7](#overview)](#overview)

[2. Scope [7](#scope)](#scope)

[Incident Guidance [8](#incident-guidance)](#incident-guidance)

[1. What Constitutes an Incident?
[8](#what-constitutes-an-incident)](#what-constitutes-an-incident)

[2. Information Security Incidents
[9](#information-security-incidents)](#information-security-incidents)

[3. IT Incidents [10](#it-incidents)](#it-incidents)

[4. Business Incidents [10](#business-incidents)](#business-incidents)

[5. Network Incidents [11](#network-incidents)](#network-incidents)

[Reporting Incident and Weaknesses
[11](#reporting-incident-and-weaknesses)](#reporting-incident-and-weaknesses)

[1. Incident Detection and Reporting
[11](#incident-detection-and-reporting)](#incident-detection-and-reporting)

[2. Reporting IT Incidents
[12](#reporting-it-incidents)](#reporting-it-incidents)

[3. Prohibited Actions -- IT incidents
[12](#prohibited-actions-it-incidents)](#prohibited-actions-it-incidents)

[Roles and Contact Details
[13](#roles-and-contact-details)](#roles-and-contact-details)

[1. Internal [13](#internal)](#internal)

[2. External [13](#external)](#external)

[3. Information Security Officer
[14](#information-security-officer)](#information-security-officer)

[4. Information Security Management Board
[14](#information-security-management-board)](#information-security-management-board)

[5. External Support Contacts
[14](#external-support-contacts)](#external-support-contacts)

[Detecting a Compromise
[15](#detecting-a-compromise)](#detecting-a-compromise)

[1. Assigning a category and severity
[16](#assigning-a-category-and-severity)](#assigning-a-category-and-severity)

[Triage [18](#triage)](#triage)

[Lessons Learned [19](#lessons-learned)](#lessons-learned)

[Incident Response Improvements
[20](#incident-response-improvements)](#incident-response-improvements)

[Legal Requirements [20](#legal-requirements)](#legal-requirements)

[1. Data Protection [20](#data-protection)](#data-protection)

[2. When to report? [21](#when-to-report)](#when-to-report)

[1. What to report? [21](#what-to-report)](#what-to-report)

[2. Where to report? [21](#where-to-report)](#where-to-report)

[Revisions Record Sheet
[23](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [23](#approvals)](#approvals)

### General Information {#general-information .Heading-3_Green}

### Acronyms 

+-------------+---------------------------------------------------------+
| **Acronym** | > **Description**                                       |
+=============+=========================================================+
| CMA         | > Computer Misuse Act                                   |
+-------------+---------------------------------------------------------+
| CPS         | > Crown Prosecution Service                             |
+-------------+---------------------------------------------------------+
| DPA         | > Data Protection Act 2018                              |
+-------------+---------------------------------------------------------+
| DSL         | > Digital Subscriber Line                               |
+-------------+---------------------------------------------------------+
| GDS         | > Global Distribution Service                           |
+-------------+---------------------------------------------------------+
| ICO         | > Information Commissioner's Office                     |
+-------------+---------------------------------------------------------+
| ISO         | > Information Security Officer                          |
+-------------+---------------------------------------------------------+
| NSI         | > New Site Introduction                                 |
+-------------+---------------------------------------------------------+
| ISA         | > Information Security Analyst                          |
+-------------+---------------------------------------------------------+
| PII         | > Personally Identifiable Information                   |
+-------------+---------------------------------------------------------+
| PoC         | > Point of Contact                                      |
+-------------+---------------------------------------------------------+
| SOCA        | > Serious and Organised Crime Agency                    |
+-------------+---------------------------------------------------------+
| TSA         | > Telecommunications (Security) Act 2021                |
+-------------+---------------------------------------------------------+

### Glossary

+----------------------+-------------------------------------------------------+
| **Term**             | > **Description**                                     |
+======================+=======================================================+
| **Availability**     | > The property of being accessible and usable upon    |
|                      | > demand by an authorised entity.                     |
| ISO 27000:2014       |                                                       |
+----------------------+-------------------------------------------------------+
| **Confidentiality**  | > The property that information is not made available |
|                      | > or disclosed to unauthorised individuals, entities, |
| ISO 27000:2014       | > or processes.                                       |
+----------------------+-------------------------------------------------------+
| **Data Controller**  | > '...a person who (either alone or jointly or in     |
|                      | > common with other persons) determines the purposes  |
|                      | > for which and the manner in which any personal data |
|                      | > are, or are to be, processed'                       |
+----------------------+-------------------------------------------------------+
| **Event handling     | > An event is any observable occurrence in a system   |
| guide**              | > or network. Events include a user connecting to a   |
|                      | > file share, a server receiving a request for a web  |
| NIST SP 800-61       | > page, a user sending email, and a firewall blocking |
|                      | > a connection attempt. Adverse events are events     |
|                      | > with a negative consequence, such as system         |
|                      | > crashes, packet floods, unauthorised use of system  |
|                      | > privileges, unauthorised access to sensitive data,  |
|                      | > and execution of malware that destroys data.        |
+----------------------+-------------------------------------------------------+
| **Information        | > An identified occurrence of a system, service or    |
| security event** ISO | > network state indicating a possible breach of       |
| 27000:2014           | > information security policy or failure of controls, |
|                      | > or a previously unknown situation that may be       |
|                      | > security relevant.                                  |
+----------------------+-------------------------------------------------------+
| **Information        | > A single or a series of unwanted or unexpected      |
| security incident**  | > ***information security events*** that have a       |
| ISO 27000:2014       | > significant probability of compromising business    |
|                      | > operations and threatening information security.    |
+----------------------+-------------------------------------------------------+
| **Information        | > The processes for detecting, reporting, assessing,  |
| security incident    | > responding to, dealing with, and learning from      |
| management** ISO     | > ***information security incidents***.               |
| 27000:2014           |                                                       |
+----------------------+-------------------------------------------------------+
| **Integrity**        | > The property of accuracy and completeness.          |
|                      |                                                       |
| ISO 27000:2014       |                                                       |
+----------------------+-------------------------------------------------------+
| **Threat**           | > The potential cause of an unwanted incident, which  |
|                      | > may result in harm to a system or organisation.     |
| ISO 27000:2014       |                                                       |
+----------------------+-------------------------------------------------------+
| **Vulnerability**    | > The weakness of an asset or control that can be     |
|                      | > exploited by one or more ***threats***.             |
| ISO 27000:2014       |                                                       |
+----------------------+-------------------------------------------------------+
| **Telecommunications | Provides guidance and support for The Electronic      |
| Security Act Code of | Communications Security Measures Regulations 2022 and |
| Practice**           | is based on draft guidance developed by experts in    |
|                      | the National Cyber Security Centre (NCSC).            |
+----------------------+-------------------------------------------------------+
| **NCSC Cyber         | A systematic and comprehensive approach to assessing  |
| Assessment Framework | the extent to which cyber risks to essential          |
| (CAF) v3.1**         | functions are being managed by the organisation       |
|                      | responsible.                                          |
+----------------------+-------------------------------------------------------+

### References and Related Documents

+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **Ref  | > **Document**     | > **Reference**                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| \#**   |                    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+========+====================+==================================================================================================================================================================================================================================================================================================================================================================================================================================================================+
| **1**  | > Operational      | > [ISD001-Operational Security Framework.pdf](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISD001-Operational%20Security%20Framework.pdf?csf=1&web=1&e=hNl01c)                                                                                                                                                                                                                           |
|        | > Security         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | >                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | > Framework        |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **2**  | > Incident         | > [IMS15.01 TMBS IT Incident Management](https://communityfibre.sharepoint.com/sites/IMS_home/IMS%20Manual/Forms/AllItems.aspx?id=%2Fsites%2FIMS%5Fhome%2FIMS%20Manual%2FIMS15%20TMBS%2FIMS15%2E01%20IT%20Incident%20Management%20%2D%20Jul25%20v1%2Epdf&parent=%2Fsites%2FIMS%5Fhome%2FIMS%20Manual%2FIMS15%20TMBS)                                                                                                                                             |
|        | > Response and     | >                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|        | > Business         | > [IMD13.02 NETWORK INCIDENT                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|        | > Continuity Plan  | > MANAGEMENT](https://communityfibre.sharepoint.com/sites/IMS_home/IMS%20Manual/Forms/AllItems.aspx?viewid=a94d27c9%2Dbfb6%2D44c2%2Da5b7%2Dab0cdea785d9&FolderCTID=0x012000A4B2E690CD1183439382F087CBA13285&id=%2Fsites%2FIMS%5Fhome%2FIMS%20Manual%2FIMS13%20Outage%20Process%2FIMD13%20Documents%2FIMD13%2E02%20Network%20Incident%20Management%20Oct24%20v3%2Epdf&parent=%2Fsites%2FIMS%5Fhome%2FIMS%20Manual%2FIMS13%20Outage%20Process%2FIMD13%20Documents) |
|        |                    | >                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|        |                    | > [ISPR001-Business Continuity Plan_v2.2.pdf](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISPR001-Business%20Continuity%20Plan_v2.2.pdf?csf=1&web=1&e=7tZ227)                                                                                                                                                                                                                           |
+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **3**  | > EU GDPR          | > [General Data Protection Regulation (GDPR) -- Official Legal Text (gdpr-info.eu)](https://gdpr-info.eu/)                                                                                                                                                                                                                                                                                                                                                       |
+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **4**  | > NIST Computer    | > [Computer Security Incident Handling Guide (nist.gov)](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf)                                                                                                                                                                                                                                                                                                                             |
|        | >                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | > Security         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | > Incident         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | >                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | > Handling Guide   |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **5**  | The Data           | [Data Protection Act 2018 (legislation.gov.uk)](https://www.legislation.gov.uk/ukpga/2018/12/contents/enacted)                                                                                                                                                                                                                                                                                                                                                   |
|        | Protection Act     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **6**  | ICO Notification   | [Data breach reporting \| ICO](https://ico.org.uk/for-organisations/report-a-breach/personal-data-breach/)                                                                                                                                                                                                                                                                                                                                                       |
|        | of data security   |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | breaches to the    | [Report a data security breach (PECR) \| ICO](https://ico.org.uk/for-organisations/report-a-breach/data-security-breach-pecr/)                                                                                                                                                                                                                                                                                                                                   |
|        |                    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | Information        | [ico-nis-reporting-form.docx (live.com)](https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fico.org.uk%2Fmedia%2Freport-a-concern%2Fforms%2F2618561%2Fico-nis-reporting-form.docx&wdOrigin=BROWSELINK)                                                                                                                                                                                                                                              |
|        |                    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | Commissioner's     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | Office             |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **7**  | ICO Data           | [report-a-personal-data-breach-form.doc (live.com)](https://view.officeapps.live.com/op/view.aspx?src=https%3A%2F%2Fico.org.uk%2Fmedia%2Freport-a-concern%2Fforms%2F4019685%2Freport-a-personal-data-breach-form.doc&wdOrigin=BROWSELINK)                                                                                                                                                                                                                        |
|        | protection breach  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | notification form  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **8**  | The Computer       | [Computer Misuse Act 1990 (legislation.gov.uk)](https://www.legislation.gov.uk/ukpga/1990/18/crossheading/computer-misuse-offences)                                                                                                                                                                                                                                                                                                                              |
|        | Misuse Act 1990    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **9**  | CPS Computer       | [Computer Misuse Act \| The Crown Prosecution Service (cps.gov.uk)](https://www.cps.gov.uk/legal-guidance/computer-misuse-act)                                                                                                                                                                                                                                                                                                                                   |
|        | Misuse Act 1990    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **10** | Information        | [ISD003-Incident Reporting and Management Framework.pdf](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISD003-Incident%20Reporting%20and%20Management%20Framework.pdf?csf=1&web=1&e=CDw0LO)                                                                                                                                                                                               |
|        | Security           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        |                    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | Incident Reporting |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | and Management     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | Framework          |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **11** | Network Incident   | [IMD13.02 Network Incident Management Oct24 v3.pdf](https://communityfibre.sharepoint.com/:b:/r/sites/IMS_home/IMS%20Manual/IMS13%20Outage%20Process/IMD13%20Documents/IMD13.02%20Network%20Incident%20Management%20Oct24%20v3.pdf?csf=1&web=1&e=z71xCJ)                                                                                                                                                                                                         |
|        | Management Plan    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **12** | NCSC Cyber         | <https://www.ncsc.gov.uk/files/NCSC-CAF-v3-1.pdf>                                                                                                                                                                                                                                                                                                                                                                                                                |
|        | Assessment         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | Framework (CAF)    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | v3.1               |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **13** | Telecommunications | [Telecommunications_Security_CoP_Accessible.pdf](https://assets.publishing.service.gov.uk/media/6384d09ed3bf7f7eba1f286c/E02781980_Telecommunications_Security_CoP_Accessible.pdf)                                                                                                                                                                                                                                                                               |
|        | Security Code of   |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|        | Practice           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+--------+--------------------+------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

### Introduction {#introduction .Heading-3_Green}

### Overview

The handling of information security incidents is treated as a separate
element of the IT Incident Management Plan
\[[2](#references-and-related-documents)\] and Network Incident
Management Plan \[[11](#references-and-related-documents)\] given the
considerably more targeted and confidential nature of information
security incidents. Currently there is a definite focus on Data
Protection and The Electronic Communications Security Measures
Regulations 2022 due to the prevailing compliance efforts, though not at
the expense of generic applicability.

The objectives of Incident Management are:

- Identify Incidents as early as possible to limit the impact on
  Community Fibre's information assets and clients.

- Isolate the affected processes and / or systems to prevent further
  spread within the company.

- Enable evidence to be gathered in accordance with company or legal
  requirements to enable the enforcement of formal disciplinary
  procedures and criminal proceedings if appropriate.

- Maintain information on incidents to enable trend analysis to be
  undertaken.

- Refine policies and procedures as necessary to reduce exposures.

- Ensure that any new risk reduction measures identified as part of the
  investigation of an Incident are discussed and where appropriate,
  implemented.

- Provide feedback into the threat assessments for the company.

Elements of the following sources of Incident Response requirements have
been integrated (it [should]{.underline} be the case that further
coverage is delivered as a result of feedback during live operation):

- Data Protection requirement within reference
  \[[3](#references-and-related-documents)\]

- NCSC Cyber Assessment Framework (CAF) v3.1
  \[[12](#references-and-related-documents)\]

- Telecommunications Security Code of Practice
  \[[13](#references-and-related-documents)\]

- NIST SP 800-35 reference, see reference
  \[[4](#references-and-related-documents)\]

### Scope

The Security Incident Response Plan is applicable to all Community Fibre
employees (staff, contracted third parties and agents of Community Fibre
who have access to Community Fibre's systems, networks or information).
It applies to all networks systems and systems that store, hold, process
or transmit critical Community Fibre data.

**Information Security is the responsibility of every employee and with
your help and co-operation we can all contribute to making Community
Fibre a safe and secure working environment.**

Community Fibre staff should be aware that any breach of these
responsibilities may result in disciplinary action and possible
dismissal. Contractors, associates, temporary and service provider
staff, and other persons who have been authorised to use Community Fibre
Information Assets, must be aware that failure to comply with the
requirements of this Framework may result in termination of contracts,
contractual penalties and/or legal action, depending on the
circumstances.

Community Fibre have partnered with ANS for a managed Security
Operations Service. This service augments and extends our incident
detection and response capabilities and provide expert knowledge that
would otherwise have been difficult to build and implement.

Further responsibilities are placed on specific members of Community
Fibre staff for the management of Incidents and Weaknesses once they
have been reported.

### Incident Guidance {#incident-guidance .Heading-3_Green}

### What Constitutes an Incident?

In a wider context, an Incident is defined as any event or action
occurring within Community Fibre that results in a compromise of
financial or information assets, the communications infrastructure and
IT services or equipment, or in harm to people, either within Community
Fibre or one of our clients.

A Weakness is a situation where there is potential for an Incident to
occur but where no Incident has yet occurred.

Incidents are the result of errors in the management systems, failures
in IT or network infrastructure or they might be caused by human error.
All Incidents should be recorded, even if the cause of Incidents may be
apparent and might be addressed without the need for further
investigation.

### Information Security Incidents

An Information Security Incident is defined as an event that compromises
the Confidentiality, Integrity or Availability of one or more
Information Assets, having an adverse impact on performance or ability
to meet regulatory or legal obligations, or on Community Fibre's
reputation or brand.

+-------------------+--------------------------------------------------+
| > Category        |                                                  |
+:=================:+==================================================+
|                   | - Unauthorised access to premises                |
|                   |                                                  |
|                   | - Unauthorised access to systems or applications |
|                   |   i.e. externally by hacking or internally       |
|                   |   through circumvention of access privileges     |
|                   |                                                  |
|                   | - Loss or theft of computer equipment and/or     |
|                   |   sensitive information                          |
|                   |                                                  |
|                   | - User ID and/or password compromise             |
|                   |                                                  |
|                   | - Misdirection of sensitive mail / fax / email   |
|                   |                                                  |
|                   | - Accidental broadcast of sensitive email        |
|                   |                                                  |
|                   | - Theft or deliberate leaks of information       |
+-------------------+--------------------------------------------------+
|                   | - Data input, operator or program error          |
|                   |                                                  |
|                   | - Virus or malicious code                        |
|                   |                                                  |
|                   | - Hacking - unauthorised use of systems,         |
|                   |   applications or hacking tools                  |
|                   |                                                  |
|                   | - Inappropriate use of corporate resources, such |
|                   |   as the internet                                |
|                   |                                                  |
|                   | - Fraudulent activities - unauthorised           |
|                   |   manipulation of data                           |
|                   |                                                  |
|                   | - Absence of, or poor, change control            |
+-------------------+--------------------------------------------------+
|                   | - Fire, flood or power failure                   |
|                   |                                                  |
|                   | - Hardware/software/communications failure       |
|                   |                                                  |
|                   | - Failure of environmental controls              |
|                   |                                                  |
|                   | - Sabotage or vandalism                          |
|                   |                                                  |
|                   | - Loss or failure of backup media                |
|                   |                                                  |
|                   | - Equipment theft                                |
|                   |                                                  |
|                   | - Force majeure                                  |
+-------------------+--------------------------------------------------+

Some Incidents are normal day-to-day activities such as the resetting of
a password, or a printing error. These do not qualify as Information
Security Incidents, and such cases need to be logged with the IT
Helpdesk in the regular manner.

An Information Security Incident or Weakness may be identified by any
employee. All suspected or detected breaches of security must be
reported to an appropriate contact as soon as possible after
identification. Information Security Incidents can be divided into three
categories: **IT Incidents, Business or Network Incidents**.

### IT Incidents

This will include (but will not be limited to):

- Breaches of the Community Fibre Access Control Policy or any of the
  sub policies (i.e., Privileged Access Rights Policy).

- Inappropriate use of IT Assets including harassment or illegal
  material.

- Malicious code attacks e.g. viruses, worms, etc.

- Hoaxes

- Unauthorised access to Community Fibre information.

- Network attacks or Denial of Service Attacks (DoS).

- Suspected probing or scanning of the network.

- Telephone system failure.

- Compromise of information or asset integrity.

- Any alerts / suspicious activity on security critical systems,
  internal systems, or applications and application platforms that prove
  to be a real security alert.

- Any illegal activity.

- The potential for any of the above to occur.

### Business Incidents

This will include (but will not be limited to):

- Breaches of the Community Fibre Acceptable Usage Policy e.g. email /
  web abuse.

- Power outages

- Harm to an individual because of the compromise of Community Fibre
  Information Asset.

- Damage or disaster.

- Theft and loss of IT hardware and software applications.

- The theft or loss of Community Fibre information (including documents
  and files).

- Racist, sexist or other material which seeks to denigrate any class of
  individuals.

- Defamatory or other illegal material.

- The loss of a Community Fibre site, at which processing, and storage
  of Community Fibre information takes place, for more than one working
  day.

- The likelihood that Community Fibre will be brought into disrepute or
  might suffer reputational damage.

- A significant impact on the ability of Community Fibre to perform its
  duties.

- An event that is of interest to local or national press.

- The potential for any of the above to occur.

### Network Incidents

This will include (but will not be limited to):

- Breaches of the Community Fibre Access Control Policy or any of the
  sub policies (i.e., Privileged Access Rights Policy).

- Deviation from the Physical Security Standard.

- Routing anomalies, such as BGP route leaks, unauthorised prefix
  announcements.

- Network attacks or Denial of Service Attacks (DoS)

- Failures in customer network provisioning, such as misconfiguration of
  ONTs or CPEs leading to service degradation or outages.

- Congestion or capacity issues in core network segments, such as
  overloaded aggregation switches, transit links, or peering exchanges.

- Security vulnerabilities in network protocols, including exploits
  targeting core elements like DNS or DHCP servers.

- Physical tampering or unauthorised access to network infrastructure,
  such as at street cabinets, data centres, or customer installation
  points.

- Environmental impacts on network assets, including flooding,
  overheating, or electromagnetic interference affecting core fibre runs
  or customer modems.

- Integration failures with third-party networks, such as issues at
  internet exchange points or upstream provider interconnects.

- Monitoring and alerting system failures specific to networks.

- Compliance-related network events, such as failures to enforce traffic
  shaping under net neutrality rules or data retention obligations for
  customer sessions.

- SLA violations due to core or customer network performance issues.

- Regulatory non-compliance incidents, such as failures to report data
  breaches involving customer network data under UK GDPR or TSA/Ofcom
  guidelines.

- The potential for any of the above to occur.

### Reporting Incident and Weaknesses {#reporting-incident-and-weaknesses .Heading-3_Green}

### Incident Detection and Reporting

When first detecting or suspecting an Incident or security weakness, you
must follow these steps:

- Ensure that immediate actions are taken to safeguard peoples' Health &
  Safety.

- Immediately stop working on any affected IT asset.

- Without delay, report the Incident to an appropriate point of contact.

- If you feel that impact of the Incident is, or might become
  significant, ensure you report this directly to a contact. Do not send
  an e-mail or leave a message.

- Follow the instructions of the person to whom you report the Incident,
  and any further instructions that are given by those who are managing
  resolution of the Incident.

- Do not tell anyone else about the Incident, unless they have a
  justifiable need to know, or if you are following specific
  instructions from a manager or the Incident Reporting Contact.

### Reporting IT Incidents

When reporting an IT Incident, in addition to the above, ensure you have
the following information available to support prompt investigation.

- Your contact details.

- Your location.

- ID of the affected Asset(s) (if known).

- What the symptoms are; i.e. what makes you think this is an Incident;

- What actions you have taken so far.

- Any information as to what could have triggered the Incident.

- Any symptoms of the problem or any messages appearing on the screen.

### Prohibited Actions -- IT incidents

- If an Incident occurs, do not attempt any of the following.

- Do not try to investigate an Incident yourself.

- Do not try to prove a suspected weakness -- testing weaknesses might
  be interpreted as a potential misuse of the system.

- Do not try to shut down an infected machine but wait until you receive
  advice from IT staff.

- Do not try to have "a quick look" as this can invalidate evidence.

- Do not forward any emails containing a suspected virus or malicious
  software.

- Do not copy or forward any material that could be considered offensive
  or obscene.

- Do not try to remove any suspect software. This must only be done by
  IT staff.

- Do not transfer any files or removable IT assets to other computers.

- Do not tell anyone outside Community Fibre of the Incident, all client
  / media contact must be referred to the dedicated point of contact.

### Roles and Contact Details {#roles-and-contact-details .Heading-3_Green}

### Internal

Contact the IT Service Desk (available on weekdays from 9.00am --
5.30pm):

**Phone: +44 (0) 7485 323 664**

**Emergency Out of Hours +44 (0) 7949 052 591**

**Email:** <itsupport@communityfibre.co.uk> **OR**
<security@communityfibre.co.uk>

[For network incident:]{.mark}

The following table is the Information Security incident focused
addition to the role list defined within
\[[2](#references-and-related-documents)\].

+--------------------------------+------------------+-----------------+
| Role                           | > Named          | > 24x7 contact  |
|                                | > individual     |                 |
+================================+==================+=================+
| Head of Security               | Chris Steytler   | > 07896 288 620 |
+--------------------------------+------------------+-----------------+
| CIO                            | Chris Williams   | > 07980 867 656 |
+--------------------------------+------------------+-----------------+
| Director of Service and Data   | Kirsty Goddard   | > 07966 137 256 |
+--------------------------------+------------------+-----------------+
| IT Service & Delivery Manager  | Rob Goddard      | > 07794 212 583 |
+--------------------------------+------------------+-----------------+
| Service Operations Manager     | > Alan Dickson   | > 07957 669 235 |
+--------------------------------+------------------+-----------------+
|                                |                  |                 |
+--------------------------------+------------------+-----------------+
|                                |                  |                 |
+--------------------------------+------------------+-----------------+
|                                |                  |                 |
+--------------------------------+------------------+-----------------+

### External

ANS SOC Team (available 24 x 7 x 365)

**Phone: +44 (0)** **333 014 2999 (to raise P1 call this number)**

**Email:** <support@ansgroup.co.uk>

### Information Security Officer

The Information Security Officer (Head of Security) is responsible for:

- Reviewing and filing logs for all Information Security Incidents that
  occur, thus acting as the 'incident scribe'.

- Completing and then maintaining the associated Incident Response
  report.

- Presenting a summary of all reported Incidents and actions taken at
  each ISMS Board meeting.

- Conducting analysis (or provide information required) of Incidents, to
  identify trends and notable lessons learned from successes and
  failures, and report these to the ISMS Board (not less than annually).

- Analysing available external threat/vulnerability/Incident information
  to identify trends and notable lessons from both successes and
  failures and report findings to the ISMS Board (not less than
  annually).

### Information Security Management Board

The Information Security Management Forum is responsible for:

- Presenting a summary of all reported Incidents at each ISMS Board
  meeting.

- Determining if any remediation actions have resolved the Incident to a
  satisfactory conclusion.

- Receiving periodic analysis reports from the Information Security
  Officer and determining if existing controls are sufficient, to
  protect the organisation against identified or emergent threats or
  vulnerabilities.

- Consider Incidents and any identified Weaknesses against the Risk
  Assessment and Treatment Plan.

### External Support Contacts

+--------------------------+----------------+------------------------------------------------------------------------------------+
| Health & Safety          | 0300 790 6787  | > [[Ways to contact                                                                |
| Executive                |                | > HSE]{.underline}](https://www.hse.gov.uk/contact/contact.htm#report-an-incident) |
+==========================+================+====================================================================================+
| Environment Agency       | 03708 506 506  | > National Customer Contact                                                        |
|                          |                | >                                                                                  |
|                          |                | > Centre                                                                           |
|                          |                | >                                                                                  |
|                          |                | > PO Box 544                                                                       |
|                          |                | >                                                                                  |
|                          |                | > Rotherham                                                                        |
|                          |                | >                                                                                  |
|                          |                | > S60 1BY                                                                          |
+--------------------------+----------------+------------------------------------------------------------------------------------+

+--------------------------+----------------+------------------------+
| Ofcom                    | 0300 123 3333  | > Riverside House      |
|                          |                | >                      |
|                          |                | > 2a Southwark Bridge  |
|                          |                | > Rd                   |
|                          |                | >                      |
|                          |                | > London               |
|                          |                | >                      |
|                          |                | > SE1 9HA              |
+==========================+================+========================+
| Information              | 0303 123 1113  | > Wycliffe House       |
| Commissioner's Office    |                | >                      |
|                          |                | > Water Lane           |
|                          |                | >                      |
|                          |                | > Wilmslow             |
|                          |                | >                      |
|                          |                | > Cheshire             |
|                          |                | >                      |
|                          |                | > SK9 5AF              |
+--------------------------+----------------+------------------------+

### Detecting a Compromise {#detecting-a-compromise .Heading-3_Green}

The following is a small subset of the possible security events that
would require investigation:

- Malware detection

- File integrity monitor alert

- Log monitor alert

- Unknown or unexpected outgoing Internet network traffic from data
  processing environments

- Presence of unexpected IP addresses or routing

- Unknown or unexpected network traffic

- Unknown or unexpected services and applications configured to launch
  automatically on system boot

- Unknown files, software and devices installed on systems

- Unexplained modification or deletion of data

- Anti-virus programs malfunctioning or becoming disabled for unknown
  reasons

- Excessive failed login attempts in system authentication and event
  logs

- Vendor or third-party connections made to any CFL environment without
  prior consent and/or a ticket

- SQL Injection attempts or strange code in web server logs

- Authentication event log modifications (i.e., unexplained event logs
  are being deleted)

- Suspicious after-hours file system activity

- Systems rebooting or shutting down for unknown reasons

- Unexpected file lengths, sizes or dates, especially for system files

- Unexplained new user accounts

- Presence of archived/compressed or unknown encrypted files in system
  directories

- Variances in log chronology or timestamps

### Assigning a category and severity

The generation of 1 or more **Information Security Events** needs to be
assigned a **Severity** with an associated **Scope**, before the correct
resources that are required to mitigate the incident can be allocated in
a timely manner.

The **Scope** can be of any scale e.g., from a single laptop, a site, a
data centre, the head-office and may well change during the incident.
The **Severity** assignment is dependent on the prevailing **Scope**.
For example, the resources allocated to a malware hit on a single laptop
might be limited to disabling its access (with subsequent handling
within the Service Desk). At the other end of the scale the infection of
an entire site forming a botnet would all but instantaneously be
allocated the maximum available resources.

The actual publication of the severity must bear in mind that the
audience is likely to be non-technical and so the following color scheme
is planned:

+---+----------------------------+-----------+----------------------------------------------------------------+
|   | **Reporting timeframe**    | > **'P'** | **Severity** examples based on the associated **Scope**        |
|   +----------------------------+           |                                                                |
|   | > **Escalation**           |           |                                                                |
|   +---------+--------+---------+           |                                                                |
|   |         |        |         |           |                                                                |
+===+:=======:+:======:+:=======:+:=========:+===============================+================================+
|   | Service | > ISO  | > ISMS  |           |                                                                |
|   | Desk    |        | > Board |           |                                                                |
+---+---------+--------+---------+-----------+-------------------------------+--------------------------------+
|   | > 15 minutes               | > **P1**  | Physical/logical data centre  |                                |
|   |                            |           | breach or malware infection   |                                |
|   |                            |           |                               |                                |
|   |                            |           | Wide-scale Denial-of-Service  |                                |
|   |                            |           | or malware infection          |                                |
|   |                            |           |                               |                                |
|   |                            |           | Critical business service     |                                |
|   |                            |           | disruption                    |                                |
+---+---------+--------+---------+           |                               |                                |
|   | **X**   | **X**  | **X**   |           |                               |                                |
+---+---------+--------+---------+-----------+-------------------------------+--------------------------------+
|   | > 1 hour                   | > **P1**  | Physical/logical site breach  | Site/multi-host malware        |
|   |                            |           |                               | infection                      |
|   |                            |           | Business service disruption   |                                |
|   |                            |           |                               | Major unauthorised disclosure  |
|   |                            |           | High profile email/web abuse  | of personal, client or company |
|   |                            |           | match                         | information                    |
|   |                            |           |                               |                                |
|   |                            |           |                               | H/NIDS significant signature   |
|   |                            |           |                               | match log filter               |
+---+---------+--------+---------+           |                               |                                |
|   | **X**   | **X**  | **X**   |           |                               |                                |
+---+---------+--------+---------+-----------+-------------------------------+--------------------------------+
|   | > 1 day                    | > **P2**  | Device malware infection      | Unlicensed/unauthorised        |
|   |                            |           |                               | software installations         |
|   |                            |           | Stolen lap-top or mobile      |                                |
|   |                            |           |                               | Major unauthorised disclosure  |
|   |                            |           | Low profile email/web abuse   | of personal, client or company |
|   |                            |           |                               | information                    |
+---+---------+--------+---------+           |                               |                                |
|   | **X**   | **X**  |         |           |                               |                                |
+---+---------+--------+---------+-----------+-------------------------------+--------------------------------+
|   | > 1 week                   | > **P3**  | Shared password, generic or test account detection             |
|   |                            |           | Scans/Probes/Attempted Access                                  |
+---+---------+--------+---------+           |                                                                |
|   | **X**   | **X**  |         |           |                                                                |
+---+---------+--------+---------+-----------+----------------------------------------------------------------+
|   | > N/A                      | > **P4**  | > Upon investigation the observation or apparent incident from |
|   |                            |           | > above was then found not to be a security incident, but is   |
|   |                            |           | > logged for future awareness upon re-occurrence of the        |
|   |                            |           | > original symptoms                                            |
+---+----------------------------+-----------+----------------------------------------------------------------+

### Triage {#triage .Heading-3_Green}

Confirmed or even suspected loss or theft of any material must be
immediately investigated so that '**Containment and Exposure
limitation**' is the order of the day.

![Diagram Description automatically
generated](media/image3.jpg){width="6.5in" height="3.25in"}

Members of the IT Operations and Security Operations team act on alerts
collated via the systems detailed within
\[[1](#references-and-related-documents)\]. Security Operations team
will work closely with colleagues in the Technology, Network Technology
or Operations teams. It may be the case that a true security incident is
rapidly escalated to where contacts need to be made external and
potentially to the company.

All actions are priority based dependent on the assigned severity
\[[1](#references-and-related-documents)\]. It should be kept in mind
that a full scale (e.g., denial of service) attack on 1 company target
may be used to obscure a low-grade attack on another target. The central
monitoring platform must be kept under constant review to separate out
the actual targets that are under attack at any given point in time.

- Breaches relating to customer data or other data protection issues may
  well need to be reported in a short timescale.

- Significant outages or incidents of network infrastructure may well
  need to be reported to Ofcom in a short timescale.

- Wherever there is any suspicion of criminal activity then the Incident
  Response Team must rapidly decide as to whether forensics specialists
  are to be called in, though the affected systems can be isolated.

The preservation of evidence:

1.  Do not access or alter compromised systems (i.e., do not log on at
    all to the machine and change passwords, do not log in as root or
    Administrator).

2.  Do not turn the compromised machine off. Instead, isolate
    compromised systems from the network (i.e., unplug cable).

3.  Preserve logs and electronic evidence, ensuring that records are
    complete, unaltered, and collected in a form admissible for legal or
    disciplinary proceedings (e.g., maintain chain of custody
    documentation).

4.  Log all actions taken, including timestamps, personnel involved, and
    verification that collection systems were operational and
    functioning correctly.

5.  Be on 'high' alert and monitor all critical business systems with
    customer and other critical data.

6.  Ensure evidence is identified, collected, acquired, and preserved by
    qualified and certified personnel who are legally entitled to handle
    digital evidence, without making assumptions about its future
    relevance in litigation.

7.  Where applicable, create electronic replicas that are identical to
    physical evidence counterparts.

8.  Seek legal advice or involve law enforcement authorities as soon as
    possible to prevent accidental or intentional destruction of
    evidence and to align with regulatory, contractual, and
    jurisdictional requirements

- Specifically for cases of suspected fraud then the CFO must be
  contacted.

- The Media representative may well need to be brought in for cases that
  affect customer data and Community Fibre's corporate profile.

- Technology or Network Technology or Operations team members may be
  called upon to isolate systems and recover them from back-up or create
  further virtual machines if the original ones are under forensic
  analysis.

### Lessons Learned {#lessons-learned .Heading-3_Green}

All completed security incident analysis reports are completed by the
ISO (Head of Security) and stored and maintained by the ISO (OneDrive)
and may include:

- Associated documented processes require updating and propagation.

- New hardware or software defenses need to investigate as a priority.

- Further formal training is required.

- Disciplinary action must be taken.

- Whether third party analysis and associated penetration testing is
  required to provide assurance that the incident has been successfully
  resolved.

- All security incidents would be raised in the next bi-weekly Security
  Operations stand-up; or an out-of-cycle meeting may be called for
  serious incidents.

- Ongoing trends analysis is essential to ensure that lessons can be
  learned over time so that resources can be appropriately focused.

### Incident Response Improvements {#incident-response-improvements .Heading-3_Green}

The Incident Response Processes can be tested as part of business
continuity planning and in any event on an ongoing ad-hoc basis as part
of normal operations. Post-incident reviews must be conducted. This
review will identify lessons learned, assess the effectiveness of the
response, and evaluate any gaps or improvements needed. The outcomes of
the review will be considered at an appropriate governance level (e.g.,
by the nominated board-level person or committee responsible for
security oversight) and used to inform and update the incident response
policy, procedures, and processes as necessary to enhance future
preparedness and resilience.

### Legal Requirements {#legal-requirements .Heading-3_Green}

The Technology department must call on legal expertise at the earliest
indication that a breach of criminal or civil legislation is underway or
indeed has occurred, to determine the correct course of action. That
said all personnel must also have a base understanding e.g., in terms of
the preservation of forensic evidence so that any subsequent judicial
proceedings are not prejudiced.

### Data Protection

The **6^th^ principle** of the DPA (see reference
\[[5](#references-and-related-documents)\]) states:

Personal data shall be processed in a manner that ensures appropriate
security of the personal data, including protection against unauthorised
or unlawful processing and against accidental loss, destruction or
damage, using appropriate technical or organisational measures
('integrity and confidentiality')."

###  When to report?

+----------------------------------------------------------------------+
| Reference \[[6](#references-and-related-documents)\] states: When a  |
| personal data breach has occurred, you need to establish the         |
| likelihood of the risk to people's rights and freedoms. If a risk is |
| likely, you must notify the ICO; if a risk is unlikely, you don't    |
| have to report it. However, if you decide you don't need to report   |
| the breach, you need to be able to justify this decision, so you     |
| should document it.                                                  |
|                                                                      |
| - The UK GDPR introduces a duty on all organisations to report       |
|   certain personal data breaches to the relevant supervisory         |
|   authority. You must do this within 72 hours of becoming aware of   |
|   the breach, where feasible.                                        |
|                                                                      |
| - If the breach is likely to result in a high risk of adversely      |
|   affecting individuals' rights and freedoms, you must also inform   |
|   those individuals without undue delay.                             |
|                                                                      |
| - You should ensure you have robust breach detection, investigation  |
|   and internal reporting procedures in place. This will facilitate   |
|   decision-making about whether you need to notify the relevant      |
|   supervisory authority or the affected individuals, or both.        |
|                                                                      |
| - You must also keep a record of any personal data breaches,         |
|   regardless of whether you are required to notify.                  |
|                                                                      |
| If a breach is likely to result in a high risk to the rights and     |
| freedoms of individuals, the UK GDPR says you must inform those      |
| concerned directly and without undue delay. In other words, this     |
| should take place as soon as possible.                               |
|                                                                      |
| A 'high risk' means the requirement to inform individuals is higher  |
| than for notifying the ICO. Again, you will need to assess both the  |
| severity of the potential or actual impact on individuals because of |
| a breach and the likelihood of this occurring. If the impact of the  |
| breach is more severe, the risk is higher; if the likelihood of the  |
| consequences is greater, then again, the risk is higher. In such     |
| cases, you will need to promptly inform those affected, particularly |
| if there is a need to mitigate an immediate risk of damage to them.  |
| One of the main reasons for informing individuals is to help them    |
| take steps to protect themselves from the effect of a breach.        |
+======================================================================+

###  What to report?

Reference \[[6](#references-and-related-documents)\] states that the
data security breach reporting form should be submitted.

### Where to report?

- casework@ico.gsi.gov.uk

- Wycliffe House, Water Lane, Wilmslow, Cheshire SK9 5AF

**\**

3.  **The Computer Misuse Act**

References \[[8](#references-and-related-documents)\] and
\[[9](#references-and-related-documents)\] detail the following crimes
that should be reported to the local constabulary or SOCA as relevant:

1.  Unauthorised access to computer material.

2.  Unauthorised access with intent to commit or facilitate a crime.

3.  Unauthorised modification of computer material.

4.  Making, supplying or obtaining anything which can be used in
    computer misuse offences.

Report to Action Fraud at https://www.actionfraud.police.uk/ or by
calling 0300 123 2040. For serious or organised crime, contact the NCA
at https://www.nationalcrimeagency.gov.uk/.

4.  **Telecommunications Security Framework**

Under the Telecommunications (Security) Act 2021, which amends the
Communications Act 2003, and in alignment with The Electronic
Communications (Security Measures) Regulations 2022 and the associated
Telecommunications Security Code of Practice, providers of public
electronic communications networks or services have duties to report
security compromises. Section 105I of the Communications Act 2003
requires providers to inform Ofcom as soon as reasonably practicable of
any security compromise that has a significant impact on the network or
service, including:

- Network or service outages affecting availability, performance, or
  functionality (resilience incidents).

- Cyber-security incidents.

- Pre-positioning attacks (e.g., preparatory actions by threat actors
  that could lead to future compromises).

A security compromise is considered significant if it has a material
impact on the operation of the network or service, such as widespread
outages, exposure of sensitive data, or risks to national security.

Section 105J requires providers to inform affected users without undue
delay if the compromise is likely to adversely affect them, to enable
them to take protective steps. Section 105K requires providers to take
specified measures in response to a security compromise to remedy or
mitigate its effects.

Providers must also maintain records of all security compromises and
cooperate with other providers under Regulation 15 of the 2022
Regulations if a compromise may cause a connected security compromise in
another network or service.

Refer to Ofcom\'s guidance for details on significance thresholds and
reporting formats. Reports should be submitted to the Ofcom Network
Security team via the secure portal or email at
network.security@ofcom.org.uk. For further information, see
<https://www.ofcom.org.uk/internet-based-services/network-security/guidance-for-operators>.

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

  ----------------------------------------------------------------------------
  Version   Date         Author        Changes
  --------- ------------ ------------- ---------------------------------------
  0.1       28/06/2022   ISO           Initial Draft

  0.2       30/09/2022   ISO           Submit for review

  1.0       18/10/2022   ISO           Major version update.

  1.1       17/09/2024   Head of       Standard version update, TOC added, no
                         Security      other changes

  2.0       05/09/2025   Head of       Significant updates to include network
                         Security      incident specific considerations, and
                                       incident reporting requirements for the
                                       TSA.
  ----------------------------------------------------------------------------

### Approvals {#approvals .Heading-3_Green}

  --------------------------------------------------------------------------------------------------------------------------------------
  Name        Role       Signature     Date           Version   Ticket no. 
  ----------- ---------- ------------- -------------- --------- ------------------------------------------------------------------------
  Chris       Head of                  05/09/2025     2.0       [CISP-101629](https://communityfibre.atlassian.net/browse/CISP-101629)
  Steytler    Security                                          

  --------------------------------------------------------------------------------------------------------------------------------------
