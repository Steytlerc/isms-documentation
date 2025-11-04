**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISP045**

**Asset Management Policy**

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

[Responsibilities [3](#responsibilities)](#responsibilities)

[General Information [4](#general-information)](#general-information)

[Scope [4](#scope)](#scope)

[Policy [4](#policy)](#policy)

[Revisions Record Sheet
[6](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [6](#approvals)](#approvals)

### Glossary {#glossary .Heading-3_Green}

  ----------------------------------------------------------------------------------------------------------------------------------------
  Term                  Description                           Reference
  --------------------- ------------------------------------- ----------------------------------------------------------------------------
  **Asset**             Any item of value to the              
                        organisation, including information,  
                        hardware, software, facilities, and   
                        personnel.                            

  **Information asset** Data or knowledge that has value,     
                        such as customer data, network        
                        configurations, or operational logs.  

  **Asset management**  Identifying and recording of an       [Asset management -
                        organisation\'s physical assets,      NCSC.GOV.UK](https://www.ncsc.gov.uk/collection/10-steps/asset-management)
                        software, data, essential staff and   
                        utilities.                            

  **Sensitive data**    As defined in the regulations, data   
                        controlling or contributing to        
                        security-critical functions, or the   
                        content of signals.                   

  **Security-critical   A function whose operation materially 
  function**            impacts the proper operation of the   
                        network or service.                   

  **Asset owner**       The individual or team responsible    
                        for the asset\'s lifecycle, risk      
                        management, and protection.           

  **Asset custodian**   The individual or team handling       
                        day-to-day management and maintenance 
                        of the asset.                         
  ----------------------------------------------------------------------------------------------------------------------------------------

### Responsibilities {#responsibilities .Heading-3_Green}

  -------------------------------------------------------------------------
  Role                    Responsibilities
  ----------------------- -------------------------------------------------
  ISMS Board              Approve the policy, ensure resources for
                          implementation, and review compliance annually.

  Head of Security        Compliance monitoring, and annual review.

  Asset owners            Identify risks, classify assets, ensure
                          appropriate protection, and review asset status
                          regularly.

  IT/Network              Report new assets, adhere to handling procedures,
  Operations/Field        and support inventory updates.
  Operations              

  All                     Comply with acceptable use rules and report
  employees/contractors   asset-related incidents.
  and suppliers           
  -------------------------------------------------------------------------

###  {#section .Heading-3_Green}

### General Information {#general-information .Heading-3_Green}

**This document meets the following clauses:**

- Information Security Management System BS EN ISO/IEC 27002:2022 -- A
  5.9 Inventory of information and other associated assets

- Information Security Management System BS EN ISO/IEC 27002:2022 -- A
  5.11 -- Return of Assets

- The Electronic Communications (Security Measures) Regulations 2022:
  Regulation 6 (4): maintain records of the type, location, software and
  hardware information and identifying information of equipment.

### Scope {#scope .Heading-3_Green}

This policy applies to all assets owned, used, or managed by Community
Fibre within the information security management system scope. Assets
include information, hardware, software, network equipment, data
storage, virtualised environments, and people involved in network
technology, operations, and field activities. It covers public
electronic communications networks and services, including customer
premises equipment, management planes, signalling planes, and supply
chain components.

### Policy {#policy .Heading-3_Green}

All information assets shall be identified and documented in a central
asset register. Asset registers shall include:

- Identified assets relevant to the secure operation of essential
  function(s)

- Inventories shall include suitable levels of detail e.g., location,
  hardware, software, firmware, supplier, EOL date.

- Dependencies on supporting infrastructure (e.g. power, cooling etc)

- Ownership and custodianship.

- Assets relevant to security-critical functions or sensitive data shall
  be managed with cyber security in mind throughout their lifecycle,
  from creation through to eventual decommissioning or disposal.

- New assets shall be added to the associated inventory before use.

- Inventories shall be reviewed at least annually or following
  significant changes.

- Asset management systems shall integrate with monitoring tools to
  detect anomalies and support threat hunting.

##### Asset ownership

All information assets shall have a designated owner responsible for its
lifecycle management, including assessing regulatory and data protection
requirements and capabilities with support from associated suppliers and
Security Operations.

Information asset owners shall:

- Appropriately classification and protect assets in accordance with
  [ISP037-Information Classification and Handling
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP037-Information%20Classification%20and%20Handling%20Policy.pdf?csf=1&web=1&e=BgtbsF)
  and [ISP043-Information Backup
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP043-Information%20Backup%20Policy.pdf?csf=1&web=1&e=rm3BfU)
  .

- Ensure proper handling when the asset is reused or disposed of in
  accordance with [ISP044-Secure Disposal
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/CFL-006%20-%20Process%20Document%20-%20Change%20Management%20-%20Copy.pdf?csf=1&web=1&e=NmIYK1).

- Owners shall periodically assess risks, including those from incoming
  signals.

- Periodically review access restrictions considering applicable access
  control policies and supply chain vulnerabilities.

##### Classification of information assets

Information assets shall be classified based on sensitivity and
criticality in line with the [ISP037-Information Classification and
Handling
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP037-Information%20Classification%20and%20Handling%20Policy.pdf?csf=1&web=1&e=BgtbsF):

- **Public**: no restrictions.

- **Confidential**: high value, requiring encryption and access
  controls.

- **Strictly Confidential**: sensitive data or related to
  security-critical functions, with strict protections against
  compromises.

Classification shall consider regulatory definitions, such as sensitive
data or content of signals. Assets shall be labelled accordingly, using
electronic metadata or physical tags where applicable.

##### 

##### Acceptable use and handling

Assets shall be used only for authorised purposes in line with the
[ISP030-Acceptable Use
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP030-Acceptable%20Use%20Policy.pdf?csf=1&web=1&e=sbqeg4)

- Prohibiting unauthorised modifications to network equipment or
  functions.

- Ensuring secure protocols for management access, with multi-factor
  authentication.

- Protecting assets from exposure to untrusted networks or incoming
  signals.

- Handling sensitive data with encryption and monitoring for
  compromises.

Field operations teams shall follow secure procedures for asset
deployment and maintenance, avoiding reliance on external persons or
equipment where risks are identified.

##### Return and disposal of assets

Upon termination of use, assets shall be returned or disposed of
securely in line with [ISP044-Secure Disposal
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/CFL-006%20-%20Process%20Document%20-%20Change%20Management%20-%20Copy.pdf?csf=1&web=1&e=NmIYK1).

Procedures include:

- Erasing sensitive data to prevent recovery.

- Documenting disposal in the asset register.

- For network equipment, ensuring no residual risks to operations.

1.  
2.  
3.  
4.  

###  {#section-2 .Heading-3_Green}

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

  ----------------------------------------------------------------------------
  Version   Date         Author        Changes
  --------- ------------ ------------- ---------------------------------------
  0.1       28/08/2025   Head of       Initial Draft
                         Security      

  1.0       11/09/2025   Head of       Major version update, released for
                         Security      approval.
  ----------------------------------------------------------------------------

### Approvals {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     03/10.2025     1.0       [CISP-101528](https://communityfibre.atlassian.net/browse/CISP-101528)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
