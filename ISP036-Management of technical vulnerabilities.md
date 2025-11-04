**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISP036**

**Management of technical vulnerabilities**

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

[Document Objective [3](#document-objective)](#document-objective)

[Scope [4](#scope)](#scope)

[Roles and Responsibilities - General
[4](#roles-and-responsibilities---general)](#roles-and-responsibilities---general)

[Scoring and Priority Ranking
[4](#scoring-and-priority-ranking)](#scoring-and-priority-ranking)

[Vulnerability Patching
[5](#vulnerability-patching)](#vulnerability-patching)

[Reporting and Verification
[7](#reporting-and-verification)](#reporting-and-verification)

[Configuration Vulnerabilities
[7](#configuration-vulnerabilities)](#configuration-vulnerabilities)

[Anti-virus and Anti-malware
[8](#anti-virus-and-anti-malware)](#anti-virus-and-anti-malware)

[Revisions Record Sheet [8](#_Toc210220345)](#_Toc210220345)

[Approvals [8](#approvals)](#approvals)

### Glossary {#glossary .Heading-3_Green}

  ----------------------------------------------------------------------------------------------------------------------------
  Term            Description                          Reference
  --------------- ------------------------------------ -----------------------------------------------------------------------
  Common          Provides an open framework for       <https://www.first.org/cvss/v3.1/user-guide>
  Vulnerability   communicating the characteristics    
  Scoring System  and impacts of IT vulnerabilities    
  (CVSS)          and is composed of three metric      
                  groups: Base, Temporal, and          
                  Environmental. More information can  
                  be found at                          

  Exploitable     A vulnerability that could be        
  vulnerability   exploited to gain unauthorised       
                  access to the Community Fibre        
                  environment.                         

  Offensive       A method of testing where testers    [NIST - penetration
  testing         target individual binary components  testing](https://csrc.nist.gov/glossary/term/penetration_testing)
  (penetration    or the application to determine      
  test)           whether intra or intercomponent      
                  vulnerabilities can be exploited to  
                  compromise the application, its      
                  data, or its environment resources.  

  Security        Any change to a system's             [NIST - security-relevant
  relevant change configuration, environment,          change](https://csrc.nist.gov/glossary/term/security_relevant_change)
                  information content, functionality,  
                  or users which has the potential to  
                  change the risk imposed upon its     
                  continued operations.                

  Vendor          Personnel/Team from Community Fibre  
  relationship    assigned with overall responsibility 
  owner           for ensuring the requirements of     
                  Community Fibre Policies are met     
                  when engaging with, maintaining and  
                  generally dealing with vendors/third 
                  parties that have access to, or      
                  manage Community Fibre information   
                  assets and IT Resources.             
  ----------------------------------------------------------------------------------------------------------------------------

###  {#section .Heading-3_Green}

### General Information {#general-information .Heading-3_Green}

### Document Objective {#document-objective .Heading-3_Purple}

The purpose of this policy is to govern the controls that will be
established and maintained to effectively manage and mitigate security
vulnerabilities from malicious software, misconfiguration and other
sources that may pose a risk to Community Fibre business systems. It
sets the requirements for the identification and remediation of
vulnerabilities on Community Fibre systems including the requirements
for patching. The types of patches covered by this policy include
Security patches, Bug fixes and Enhancements. The secure configuration
of systems such as operating systems are also covered.

**This document meets the following clauses:**

- Information Security Management System BS EN ISO/IEC 27001:2022 --
  A.8.8

Management of technical vulnerabilities

- The Electronic Communications (Security Measures) Regulations 2022

  - Regulations 3 (Network architecture - identify/reduce risks, annual
    records)

  - Regulation 4 (Protection of data/functions)

  - Regulation 6 (Monitoring)

- Code of Practice, Section 11 (Patching and updates - rapid patching
  for oversight functions, issue tracking, PSIRT) and Section 5
  (Vulnerability scanning)

### Scope {#scope .Heading-3_Purple}

This policy applies globally to all Community Fibre staff, contractors
and vendors responsible for any systems. It excludes scanning/pen
testing (covered in ISP017-Vulnerability Detection and Testing Policy).

### Roles and Responsibilities - General {#roles-and-responsibilities---general .Heading-3_Green}

1.  Security Operations and Network Technology teams are responsible for
    the monitoring of compliance and reporting to Executive Management.

2.  Respective technology teams are responsible for sourcing, testing
    and distributing patches and updates, updating configurations and
    compiling compliance reports.

3.  Team leader shall ensure adherence to this policy.

4.  Executive Management shall ensure service acquisitions comply with
    this policy.

5.  Vendor relationship owners shall ensure the requirements of this
    policy are incorporated into contracts and service level agreements
    with service, software and equipment providers of Community Fibre
    systems.

### Scoring and Priority Ranking {#scoring-and-priority-ranking .Heading-3_Green}

1.  Priority ranking will depend on the CVSS v3.1 score of a
    vulnerability as provided by the vendor of the patch in question.
    The CVSS v3.1 score is determined based on access conditions and
    impact of a vulnerability, as well as time dependant qualities of a
    vulnerability, such as patch and exploit availability.

2.  All patches and vulnerabilities will be ranked as P0 through to P4
    based on the following chart:

+----------------+-------------------------+--------------------------+
| **CVSS Score   | **Priority**            | > **Patching SLA**       |
| (Risk Score)** |                         |                          |
+:==============:+:=======================:+==========================+
| \>=4.5         | P2 -- Medium            | Within 12 Weeks of the   |
|                |                         | vendor releasing the     |
|                |                         | patch                    |
+----------------+-------------------------+--------------------------+
| \>7.5          | P1 -- High              | Within 4 Weeks of the    |
|                |                         | vendor releasing the     |
|                |                         | patch                    |
+----------------+-------------------------+--------------------------+
| 10.0           | P0 -- Critical          | Immediate patching as    |
|                |                         | soon as the patch is     |
|                |                         | released                 |
+----------------+-------------------------+--------------------------+

3.  Where a vendor does not provide a CVSS v3.1 score, the priority will
    be determined based on the priority the vendor has provided using
    similar terminology. The Community Fibre Security Operations Team
    will determine the priority should it still not be explicitly
    stipulated by the vendor.

4.  Any borderline scores / priorities will be given a scoring as
    advised by the Community Fibre Security Operations Team and the
    relevant Community Fibre Technology Operational Teams.

5.  The priority of a vulnerability may be revised at the discretion of
    the Community Fibre Security Operations Team.

### Vulnerability Patching {#vulnerability-patching .Heading-3_Green}

1.  All system components will be protected against identified software
    security vulnerabilities by applying vendor-supplied security
    patches. This includes all firmware, operating systems and
    applications, irrespective of the device type, e.g., servers,
    firewalls, routers, PC's, mobile devices.

2.  All systems and devices will have a regular patch cycle as defined
    and managed by the relevant Community Fibre business unit.

3.  Security patches will be applied within an acceptable time from
    their release by the vendor, as determined by risk assessment
    considering: 

    1.  The Base CVSS v3.1 score

    2.  The value of the assets impacted by the vulnerability; and 

    3.  Any explicit business or contractual requirements governing
        patch deployment

    4.  Patches only need to be applied if they are applicable to the
        target system component. In some cases, vendors may release
        patches for an operating system or technology platform that is
        in use in Community Fibre, but which addresses a service or
        software component that has not been installed. In this case,
        patching is not required. If a patch addresses a vulnerability
        within a software component that is disabled but not removed on
        the target system, the patch will still be installed.

    5.  System and network administrators shall deploy software patches
        according to the criteria defined in section 4 Scoring and
        Priority Ranking. 

    6.  Teams responsible for system and network administration will
        establish and document patching procedures which detail the
        steps that will be taken to prepare, test and deploy security
        patches. 

    7.  Where possible, patch management systems shall be used to
        automate and control the distribution of patches. Patch
        management systems may help Community Fibre teams meet the
        requirements of this policy by:

<!-- -->

a)  Providing a detailed inventory of all system components within the
    production environment;

b)  Providing reports on the status of vulnerabilities and patches;

c)  Scheduling and controlling the deployment of patches to targeted
    'distribution groups'; and

d)  Initiating rollback of patch installations if necessary. 

    1.  Patches must be tested prior to deployment. Testing may take the
        form of isolated testing in a dedicated test environment that
        mimics the production environment or pilot testing on a small
        sample of systems.

    2.  A Change Request will be raised to seek authorisation for the
        installation of software patches to production systems, in
        accordance with the requirements of the Community Fibre Change
        Management Policy.

    3.  Other controls will be established and maintained to provide
        'defence in depth' and to protect IT resources against zero-day
        vulnerabilities - vulnerabilities for which the vendor has yet
        to supply a patch. Examples include: 

- System and network access controls

- Deployed and maintained; and 

- Security hardening.

### Reporting and Verification {#reporting-and-verification .Heading-3_Green}

1.  Community Fibre Technical (Service Desk, Development, DevOps) and
    Operational Teams, (Network Technology and Operations) will provide
    monthly summary reports to the Community Fibre Security Operations
    Team outlining the level of compliance with this policy as well as
    highlighting any new or outstanding P1 and P0 vulnerabilities that
    require rectification. 

2.  The Community Fibre Security Operations Team will facilitate
    vulnerability scans to verify adherence to this policy at a minimum
    at the following intervals:

  ------------------------------------------
           **Zone**           **Frequency**
  -------------------------- ---------------
     External interfaces        Quarterly

  Internal virtual networks     Quarterly

       Web Applications         Quarterly

        Mobile devices          Quarterly
  ------------------------------------------

3.  Ad-hoc scans may be performed at the discretion of the Community
    Fibre Security Operations Team or delegated function. Community
    Fibre Technology and Operational teams may request ad-hoc scans at
    any time outside the regular scanning frequency.

### Configuration Vulnerabilities {#configuration-vulnerabilities .Heading-3_Green}

Vulnerability scans may identify configuration vulnerabilities.
Configuration vulnerabilities are vulnerabilities introduced because of
misconfiguration, as opposed to software vulnerabilities that are
introduced because of programming flaws.

1.  Configuration vulnerabilities will be addressed by hardening system
    components in accordance with industry accepted best practice
    guidelines (such as the CIS Benchmarks).

2.  Teams responsible for network and system administration must
    document and maintain Security Configuration Standards for the
    system components that they are responsible for. Security
    Configuration Standards will align with industry and vendor best
    practice guidelines and be consistent with the requirements of
    Community Fibre policies and standards. 

3.  Security Configuration Standards will be updated to reflect any
    configuration change that is implemented because of an identified
    vulnerability.

### Anti-virus and Anti-malware {#anti-virus-and-anti-malware .Heading-3_Green}

1.  Anti-virus software must be deployed, maintained, and updated with
    latest definitions on all Community Fibre owned equipment. 

2.  Periodic virus scans must be performed at least on a weekly basis.

3.  Personal devices connected to the network must be running an
    appropriate anti-virus product and be up to date with the latest
    definitions. Users must ensure that adequate anti-virus protection
    is in place for privately owned devices.

4.  Users must not uninstall or disable anti-virus products on Community
    Fibre owned devices.

5.  Users must not install unapproved anti-virus products on Community
    Fibre owned devices.

6.  Community Fibre reserves the right to disconnect any device from the
    network if an infection is confirmed or suspected.

[]{#_Toc210220345 .anchor}

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

+---------+------------+------------+--------------------------------------+
| Version | Date       | Author     | Changes                              |
+=========+============+============+======================================+
| 0.1     | 12.03.2021 | ISO        | Initial Draft                        |
+---------+------------+------------+--------------------------------------+
| 1.0     | 08/03/2022 | ISO        | Final review, major version number   |
|         |            |            | assigned.                            |
+---------+------------+------------+--------------------------------------+
| 1.1     | 21/09/2022 | ISO        | Updated business address, document   |
|         |            |            | classification                       |
+---------+------------+------------+--------------------------------------+
| 1.2     | 07/11/2023 | Head of    | Document template update, employee   |
|         |            | Security   | handbook version update              |
+---------+------------+------------+--------------------------------------+
| 1.3     | 17/09/2024 | Head of    | Standard version update, TOC added,  |
|         |            | Security   | no other changes                     |
+---------+------------+------------+--------------------------------------+
| 2.0     | 12/09/2025 | Head of    | Major version update                 |
|         |            | Security   |                                      |
|         |            |            | Expanded scope to cover Network      |
|         |            |            | Technology and Operations.           |
|         |            |            |                                      |
|         |            |            | New sub policies create in support   |
|         |            |            | of this policy:                      |
|         |            |            |                                      |
|         |            |            | ISP017-Vulnerability Detection and   |
|         |            |            | Testing Policy                       |
|         |            |            |                                      |
|         |            |            | ISP016-Threat Intelligence Policy    |
+---------+------------+------------+--------------------------------------+

### Approvals {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     29/09/2025     2.0       [CISP-101378](https://communityfibre.atlassian.net/browse/CISP-101378)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
