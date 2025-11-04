**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISD007**

**Software Release Management**

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

[Purpose [3](#purpose)](#purpose)

[Scope [3](#scope)](#scope)

[Glossary [3](#glossary)](#glossary)

[Role and responsibilities
[4](#role-and-responsibilities)](#role-and-responsibilities)

[Release management process
[4](#release-management-process)](#release-management-process)

[Documentation requirements
[6](#documentation-requirements)](#documentation-requirements)

[Tools and resources [7](#tools-and-resources)](#tools-and-resources)

[Risk management and security integration
[7](#risk-management-and-security-integration)](#risk-management-and-security-integration)

[Appendix A: Release Note Template
[8](#appendix-a-release-note-template)](#appendix-a-release-note-template)

[Appendix B: Change classification matrix
[10](#appendix-b-change-classification-matrix)](#appendix-b-change-classification-matrix)

[Appendix C: Approval workflow diagram
[10](#appendix-c-approval-workflow-diagram)](#appendix-c-approval-workflow-diagram)

[Revisions Record Sheet
[11](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [11](#approvals-1)](#approvals-1)

### General Information {#general-information .Heading-3_Green}

**Related Policies:**

- [CFL-006 - Process Document - Change
  Management](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/CFL-006%20-%20Process%20Document%20-%20Change%20Management.pdf?csf=1&web=1&e=JanDNK)

- [ISP042-Software Development
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP042-Software%20Development%20Policy.pdf?csf=1&web=1&e=EQrce5)

### Purpose {#purpose .Heading-3_Green}

This document outlines the standardised process for managing software
releases to ensure controlled, secure, and efficient deployment of
changes to production environments. It addresses ISO 27001 Annex A
Control 8.32 (Change Management) by providing clear steps,
documentation, and accountability for all release types.

### Scope {#scope .Heading-3_Green}

This procedure applies to all software releases within the organisation,
including:

- New features or major enhancements.

- Code fixes (e.g., bug resolutions).

- Minor changes such as data updates, script modifications, or queries.

- Emergency releases.

It covers systems like HOBS and any other production software, including
development, testing, staging, and production environments. BAU tasks
not involving code or data changes (e.g., monitoring) are not covered by
this procedure.

### Glossary {#glossary .Heading-3_Green}

+-----------------+----------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| Term            | Description                      | Reference                                                                                                                                                                                                                 |
+=================+==================================+===========================================================================================================================================================================================================================+
| **Release       | The practice of making new and   | [Management Practices: The Purposes of the 34 ITIL 4                                                                                                                                                                      |
| management**    | changed services and service     | Practices](https://itsm.tools/34-itil-4-management-practices/#:~:text=Release%20management%20%E2%80%93%20%E2%80%9CThe%20purpose%20of,and%20features%20available%20for%20use.%E2%80%9D)                                    |
|                 | components available for use in  |                                                                                                                                                                                                                           |
|                 | line with the organisation\'s    |                                                                                                                                                                                                                           |
|                 | policies and agreements with its |                                                                                                                                                                                                                           |
|                 | users and sponsors.              |                                                                                                                                                                                                                           |
+-----------------+----------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **Change        | - **Planned**: Not done before,  | [CFL-006 - Process Document - Change                                                                                                                                                                                      |
| Types**         |   risk associated, has an        | Management.pdf](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/CFL-006%20-%20Process%20Document%20-%20Change%20Management.pdf?csf=1&web=1&e=75kNZh) |
|                 |   impact, must be raise 48hrs in |                                                                                                                                                                                                                           |
|                 |   advance.                       |                                                                                                                                                                                                                           |
|                 |                                  |                                                                                                                                                                                                                           |
|                 | - **Standard**: Has been         |                                                                                                                                                                                                                           |
|                 |   performed before and is        |                                                                                                                                                                                                                           |
|                 |   pre-authorised, with an        |                                                                                                                                                                                                                           |
|                 |   established procedure.         |                                                                                                                                                                                                                           |
|                 |                                  |                                                                                                                                                                                                                           |
|                 | - **Emergency**: intended to     |                                                                                                                                                                                                                           |
|                 |   repair an error in a service   |                                                                                                                                                                                                                           |
|                 |   that is impacting the business |                                                                                                                                                                                                                           |
|                 |   to a high degree.              |                                                                                                                                                                                                                           |
+-----------------+----------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **Release       | Formal records capturing the     |                                                                                                                                                                                                                           |
| Documentation** | release lifecycle, including     |                                                                                                                                                                                                                           |
|                 | risk assessments, testing        |                                                                                                                                                                                                                           |
|                 | results, and approvals.          |                                                                                                                                                                                                                           |
+-----------------+----------------------------------+---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

### Role and responsibilities {#role-and-responsibilities .Heading-3_Green}

  -------------------------------------------------------------------
  Role                   Responsibilities
  ---------------------- --------------------------------------------
  **Release Manager**    Oversees the release process; coordinates
                         teams; ensures documentation completeness;
                         schedules releases.

  **Developer**          Prepares changes; conducts initial testing;
                         creates release notes and documentation.

  **Change Owner**       Validates release notes and overseas the
                         change implementation and reviews the
                         deployment by DevOps Team

  **Tester/QA Team**     Performs independent testing; verifies
                         security and functionality.

  **Change Advisory      Reviews and approves releases; assesses
  Board (CAB)**          risks and impacts.

  **Information Security Evaluates security implications; ensures
  Officer (ISO)**        compliance with ISO 27001 controls (e.g.,
                         8.29 for testing, 8.32 for changes).

  **DevOps Team**        Deploys releases on SIT/UAT/prod Environment
                         and executes rollback if needed.

  **Operations Team**    Performs Sanity and Monitors post-release
                         performance

  **TCS Team (if         Provides specialised support for
  applicable)**          HOBS-related changes; maintains
                         documentation.
  -------------------------------------------------------------------

### Release management process {#release-management-process .Heading-3_Green}

The process follows a structured Software Development Lifecycle (SDLC)
with risk-based scaling. All releases must be initiated via a change
ticket in Jira.

##### Initiation and planning

- Identify the change type and scope.

- Create a change ticket with details: description, rationale, affected
  components, and potential impacts.

- Conduct an initial risk assessment (qualitative for minor changes;
  quantitative for major ones) covering security, availability, and
  business impacts.

- For HOBS changes: Reference system-specific guidelines.

- Output: Updated change ticket; preliminary release plan.

##### 

##### Development and preparation

- Develop/code the changes in a segregated environment (development
  branch).

- For minor changes (e.g., data scripts): Ensure version control and
  basic peer review.

- For code fixes: Implement unit tests and integrate with existing
  codebase.

- DevOps team move the changes to SIT/UAT from Dev branch.

- Prepare release artifacts: Binaries, scripts, configuration files.

- Output: Code committed to GIT Lab repository; initial release notes
  drafted.

##### Testing and quality assurance (QA)

- Perform testing in isolated environments:

  - Unit/Integration Testing: Automated where possible.

  - Security Testing: Vulnerability scans performed in Aikido tool

  - User Acceptance Testing (UAT): For major releases.

- Scale by type: Minor changes require basic functional tests; major
  changes need full regression testing.

- Document test results, including pass/fail criteria and evidence
  (e.g., screenshots, logs).

<!-- -->

- Output: Test report attached to change ticket.

##### Review and approval

- Submit for CAB review: Present release documentation, risks, and
  mitigation plans, Only UAT passed changes are considered.

- Obtain approvals: Electronic sign-off from relevant roles (e.g., ISO
  for security).

- For emergency releases: Use fast-track approval with post-release
  review.

- Developer provides prod Notes after peer review and then DevOps team
  reviews the prod notes and plan accordingly.

- Output: Approved release plan; scheduled deployment window.

##### 

##### Deployment

- Deploy during approved windows as per the release deployment notes
  (e.g., off-peak hours). Currently release is manually deployed onto
  servers by DevOps Team. Gitlab CI/CD pipeline is in progress.

- Follow deployment checklist: Backup production data; implement
  changes; verify post-deployment.

- Output: Deployment log, updated system status, Sanity test results.

- In case of any issue, rollback all the changes according to plan
  provided by Dev Team.

- Close the change with Sanity report.

##### 

##### Post-release review and closure

- Monitor for issues (e.g., via logging tools) for a defined period
  (min. 12 hours).

- Conduct a post-implementation review: Assess success, capture lessons
  learned.

- Ops Team will mark the ticket in Monitoring status.

- Output: Post-release report; updated knowledge base and related
  tickets in JIRA.

##### 

##### Emergency release process

- Bypass non-essential steps (e.g., full testing) with ISO/CAB verbal
  approval.

- Complete full documentation retrospectively within 24 hours.

- Follow all steps of standard CR related to code, testing and
  deployment process except point 1.

### Documentation requirements {#documentation-requirements .Heading-3_Green}

All releases require formal documentation to ensure traceability and
auditability. Use standardised templates stored in a central repository
(e.g., Jira or Confluence).

- Release Note Template (Mandatory for all changes):

  - Change ID/Ticket Number.

  - Description and Type.

  - Risk/Impact Assessment.

  - Development Lifecycle Steps Taken (e.g., \"Developed in dev env;
    tested via unit tests\").

  - Testing Evidence.

  - Approvals and signoffs.

  - Deployment Details (steps, timestamp, rollback plan).

  - Post-Release Monitoring Results.

- For Minor Changes (e.g., data queries/scripts): One-page checklist.

- For Code Fixes/Normal Changes: Detailed report with code diffs and
  test logs.

- Retention: Maintain records for at least 2 years or as per legal
  requirements.

### Tools and resources {#tools-and-resources .Heading-3_Green}

- Ticketing System: Jira

- Version Control: Gitlab

- CI/CD Tools: Gitlab

- Testing Tools: Aikido

- Monitoring: Datadog, CloudWatch monitoring

### Risk management and security integration {#risk-management-and-security-integration .Heading-3_Green}

- Development practices are in alignment with CFL [ISP042-Software
  Development
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP042-Software%20Development%20Policy.pdf?csf=1&web=1&e=nRiae8)

- Escalate high-risk releases to senior management.

- Invoke incident response if issues arise post-release.

**\**

### Appendix A: Release Note Template {#appendix-a-release-note-template .Heading-3_Green}

##### Release Notes Template

##### Document Information

- Title: Release Notes - \[e.g., HOBS\]

- Release Version: \[e.g., v1.2.3\]

- Release Date:

- Prepared By: \[Name/Role, e.g., Release Manager\]

- Approved By: \[Name/Role, e.g., Security Officer and Stakeholders\]

- Revision History:

  -------------------------------------------------------------------
  Version          Date      Description of Changes  Author
  ---------------- --------- ----------------------- ----------------
  1.0                        Initial release notes   

  -------------------------------------------------------------------

##### Introduction

This Release Notes document provides a summary of the changes included
in this software release. It details the purpose, scope, and key
elements of the release to ensure stakeholders understand the
modifications, associated risks, and implementation details. This aligns
with Community Fibre's Software Release Management Document and ISO
27001 requirements for change control (Annex A Control 8.32).

##### Release Overview

- Release Type: \[Major/Minor/Patch/Hotfix/Data Change\]

- Affected Components: \[List systems, modules, or areas impacted, e.g.,
  Database scripts, Application code\]

- Purpose: \[Brief description of the release goals, e.g., \"To address
  critical bug fixes and minor data adjustments for improved performance
  and security.\"\]

- Deployment Environment: \[Development/Staging/Production\]

##### Changes Included

  --------------------------------------------------------------------------
  **Change ID /  **Description**        **Type** (e.g.,  **Impact Level**
  Ticket**                              Feature/Bug      (Low/Medium/High)
                                        Fix/Data Change) 
  -------------- ---------------------- ---------------- -------------------
  \[e.g.,        \[Brief description,   \[Bug Fix\]      \[Medium\]
  Ticket-123\]   e.g., \"Fixed                           
                 authentication                          
                 vulnerability in login                  
                 module.\"\]                             

  \[e.g.,        \[Brief description,   \[Data Change\]  \[Low\]
  Ticket-456\]   e.g., \"Updated data                    
                 query script to                         
                 optimise                                
                 performance.\"\]                        
  --------------------------------------------------------------------------

- New Features: \[List and describe any new additions, or state \"None\"
  if inapplicable.\]

- Bug Fixes: \[List resolved issues, including references to tickets or
  known problems.\]

- Improvements/Enhancements: \[List optimisations or minor updates.\]

- Security Updates: \[Detail any security-related changes, e.g.,
  \"Patched CVE-XXXX-XXXX for encryption strength.\" Include references
  to vulnerability scans or tests.\]

- Deprecations/Removals: \[List any removed features or
  backward-incompatible changes.\]

##### Testing Summary

- Testing Performed: \[Types of tests, e.g., Unit, Integration, System,
  Security, User Acceptance.\]

- Test Results: \[Overall pass rate, e.g., \"95% pass; 2 minor defects
  resolved.\"\]

- Defects Found and Resolved: \[List or reference, e.g., \"Defect-001:
  Resolved in retest.\"\]

- Testing Evidence: \[Reference to Test Report or attachments, e.g.,
  \"See attached Test Report v1.0.\"\]

- For minor changes (e.g., data scripts), testing may be scaled: \[e.g.,
  \"Automated regression tests only.\"\]

##### Deployment Instructions

- Prerequisites: \[e.g., \"Backup production database; Ensure downtime
  window approved.\"\]

- Step-by-Step Deployment:

  - \[Step 1: e.g., \"Deploy to staging environment.\"\]

  - \[Step 2: e.g., \"Run validation scripts.\"\]

  - \[Step 3: e.g., \"Promote to production.\"\]

  - \[Step 4: e.g., \"Monitor logs for errors.\"\]

- Rollback Plan: \[Detailed steps to revert, e.g., \"Restore from
  backup; Notify stakeholders.\"\]

- Estimated Downtime: \[e.g., \"15 minutes.\"\]

- Post-Deployment Verification: \[Checks to confirm success, e.g., \"Run
  health check queries.\"\]

##### Known Issues

- \[List any unresolved issues, workarounds, and planned fixes, e.g.,
  \"Issue-789: Minor UI glitch; Workaround: Refresh page; Fix in next
  release.\"\]

- If none, state: \"No known issues.\"

##### Dependencies and Compatibility

- Required Versions: \[e.g., \"Compatible with OS v10+; Requires
  Database v5.7.\"\]

- Third-Party Impacts: \[e.g., \"TCS-provided components updated; No
  vendor dependencies affected.\"\]

- Backward Compatibility: \[e.g., \"Fully compatible with previous
  versions.\"\]

##### Approvals

+----------------+----------------+----------------+----------------+
| > Role         | Name           | Signature/Date | Comments       |
+================+================+================+================+
| > Release      |                |                |                |
| > Manager      |                |                |                |
+----------------+----------------+----------------+----------------+
| > Development  |                |                |                |
| > Lead         |                |                |                |
+----------------+----------------+----------------+----------------+
| > Security     |                |                |                |
| > Officer      |                |                |                |
+----------------+----------------+----------------+----------------+
| > Business     |                |                |                |
| > Stakeholder  |                |                |                |
+----------------+----------------+----------------+----------------+

##### Additional Notes

- \[Any other relevant information, e.g., \"Contact
  x@communityfibre.co.uk for issues.\"\]

- References: \[List related documents, e.g., \"Change Ticket Logs; Full
  Test Report.\"\]

This template should be customised for each release. Store completed
Release Notes in the central document repository for audit purposes. For
minor releases, sections may be abbreviated as appropriate.

### Appendix B: Change classification matrix {#appendix-b-change-classification-matrix .Heading-3_Green}

[CFL-006 - Process Document - Change
Management](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/CFL-006%20-%20Process%20Document%20-%20Change%20Management.pdf?csf=1&web=1&e=JanDNK)

### Appendix C: Approval workflow diagram {#appendix-c-approval-workflow-diagram .Heading-3_Green}

[CFL-006 - Process Document - Change
Management](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/CFL-006%20-%20Process%20Document%20-%20Change%20Management.pdf?csf=1&web=1&e=JanDNK)

1.  
2.  
3.  

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

  ----------------------------------------------------------------------------
  Version   Date         Author        Changes
  --------- ------------ ------------- ---------------------------------------
  0.1       28/08/2025   Head of       Initial Draft
                         Security      

  1.0       15/09/2025   Head of       Major version update, sent for approval
                         Security      

                                       
  ----------------------------------------------------------------------------

### Approvals {#approvals-1 .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     03/10/2025     1.0       [CISP-101545](https://communityfibre.atlassian.net/browse/CISP-101545)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
