**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISP044**

**Secure Disposal Policy**

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

[Procedures [4](#procedures)](#procedures)

[Recommendations by media type
[5](#recommendations-by-media-type)](#recommendations-by-media-type)

[Revisions Record Sheet
[7](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [7](#approvals)](#approvals)

### Glossary {#glossary .Heading-3_Green}

  ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  Term                  Description                          Reference
  --------------------- ------------------------------------ -------------------------------------------------------------------------------------------------------------------
  **Media**             Any physical or digital storage      The Electronic Communications (Security Measures) Regulations 2022 -- Regulation 2
                        device capable of holding data       
                        (e.g., HDDs, SSDs, USBs, CDs/DVDs,   
                        tapes).                              

  **Equipment**         Hardware used in networks or         
                        services, such as servers, routers,  
                        switches, customer devices, or SIM   
                        cards.                               

  **Sensitive data**    Critical information that controls   
                        security functions or includes       
                        protected content (not just          
                        metadata).                           

  **Security-critical   Any process or service that          
  function**            significantly affects network or     
                        service operations.                  

  **Security            Unauthorised access, interference,   
  compromise**          or related risks.                    

  **Disposal**          Permanently destroying or making     
                        something unusable, e.g., shredding  
                        or incinerating.                     

  **Re-use**            Reassigning items after securely     
                        removing data.                       

  **End-of-Life (EOL)** Equipment no longer supported by the 
                        maker (no updates available).        

  **NIST SP 800-88**    Guidelines for securely erasing data [Guidelines for Media Sanitisation](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-88r1.pdf)

  **Certificate of      Proof that data was securely erased  [Sample \"Certificate of
  Sanitisation**                                             Sanitisation\"](https://csrc.nist.gov/files/pubs/sp/800/88/r1/final/docs/sample-certificate-of-sanitization.docx)
  ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Responsibilities {#responsibilities .Heading-3_Green}

  -------------------------------------------------------------------------
  Role                    Responsibilities
  ----------------------- -------------------------------------------------
  Head of Security        Overall policy ownership, compliance monitoring,
                          and annual review.

  Asset owners            Identify assets for disposal/re-use; ensure
                          classification and risk assessment.

  IT/Network Operations   Execute disposal procedures; maintain records.
  teams                   

  Field operations        Handle on-site disposal of network equipment
                          (e.g., base stations); report to central teams

  Third-party suppliers   Comply with contractual obligations for secure
                          disposal (e.g., certified destruction); provide
                          evidence as per Regulation 13(2)(d).

  All                     Report assets ready for disposal; adhere to
  employees/contractors   procedures
  -------------------------------------------------------------------------

###  {#section .Heading-3_Green}

### General Information {#general-information .Heading-3_Green}

**This document meets the following clauses:**

- ISO/IEC 27002:2022 -- A.7.10 (Storage media) and A.7.14 (Secure
  disposal or re-use of equipment).

- Electronic Communications (Security Measures) Regulations 2022 --
  Regulation 4 (Protect stored data and functions) and Regulation 12
  (Equipment upgrades, including EOL disposal).

Purpose: To securely dispose of or re-use media and equipment,
preventing data leaks and reducing security risks.

### Scope {#scope .Heading-3_Green}

Applies to all media and equipment in our ISMS, including:

- IT assets (e.g., servers, laptops, storage devices).

- Network assets (e.g., routers, switches, base stations, customer
  equipment, SIM cards).

- All storage types (e.g., hard drives, USBs, tapes, SSDs).

- Assets with sensitive data, owned or managed by us or third parties.

### Procedures {#procedures .Heading-3_Green}

All media and equipment must be inventoried per the [Asset Management
Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP011-Information%20Access%20Rights%20Policy.pdf?csf=1&web=1&e=bpST3D).

1.  Prior to disposal or re-use, assess:

<!-- -->

a)  Data classification, does this device contain any Confidential or
    Strictly Confidential data ([ISP037-Information Classification and
    Handling
    Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP037-Information%20Classification%20and%20Handling%20Policy.pdf?csf=1&web=1&e=T37cfC)).

b)  Check and update asset inventory including device details, data,
    software, location.

<!-- -->

2.  Storage media no longer required must be disposed of using formal
    procedures to prevent data recovery. This includes storage media
    contained within any hardware devices.

3.  Methods (selected based on data sensitivity and risk
    [NIST.SP.800-88r1](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-88r1.pdf)
    ) :

    a)  **Clear:** Overwrite data with non-sensitive info using standard
        tools (quick but basic protection).

    b)  **Purge:** Use advanced erase commands (e.g., overwrite, block
        erase, or crypto erase) to make recovery impossible.

    c)  **Destroy:** Physically break it down (e.g., shred, incinerate)
        if purge isn\'t possible.

4.  Save non-sensitive data securely first before disposing of storage
    media.

5.  Use tools to check data can\'t be recovered (e.g., random checks).

6.  Reset to factory settings; reconfigure securely.

7.  Destroy high-risk items physically.

8.  For network equipment, remove configs that could reveal secrets
    (e.g., passwords, keys).

9.  For off-site work; use certified vendors and get destruction
    certificates; keep records for 3+ years in asset system.

10. Follow Incident Management Policy to report problems and incident.

### Recommendations by media type {#recommendations-by-media-type .Heading-3_Green}

#### Hard copy (Paper) {#hard-copy-paper .Heading-4_Purple}

- Clear/Purge: Not applicable.

- Destroy: Shred with a crosscut shredder.

#### Networking Devices (e.g., Routers, Switches) {#networking-devices-e.g.-routers-switches .Heading-4_Purple}

- Clear: Do a full factory reset.

- Purge: Usually not available; use destroy if needed. Check
  manufacturer for advanced erase.

- Destroy: Shred, disintegrate, pulverise, or incinerate via certified
  vendor.

- Notes: Remove removable storage first.

#### Mobile Devices  {#mobile-devices .Heading-4_Purple}

#### Apple iPhone/iPad {#apple-iphoneipad .Heading-4_Purple}

- Clear/Purge: Use \"Erase All Content and Settings\" (Settings \>
  General \> Reset). Assumes encryption is on.

- Destroy: Shred or incinerate via certified vendor.

- Notes: Verify no data remains (check history, files). Backup first.
  Remote wipe is only a clear.

#### Android Devices {#android-devices .Heading-4_Purple}

- Clear: Factory reset via settings (e.g., Backup and Reset \> Factory
  Data Reset).

- Purge: Check manufacturer for secure erase or crypto erase; may vary.

- Destroy: Shred or incinerate via certified vendor.

- Notes: Verify no data remains. Use guides like DISA STIGs for setup.
  Remote wipe is only a clear.

#### ATA Hard Drives {#ata-hard-drives .Heading-4_Purple}

- Clear: Overwrite with a single pass of fixed data (e.g., zeros).

- Purge: Use ATA sanitise commands (e.g., overwrite, crypto erase) or
  security erase.

- Destroy: Shred or incinerate via certified vendor.

- Notes: Verify after action. Backup first.

#### Flash Memory-Based Storage (e.g., SSDs) {#flash-memory-based-storage-e.g.-ssds .Heading-4_Purple}

#### ATA SSDs (PATA, SATA, etc.) {#ata-ssds-pata-sata-etc. .Heading-4_Purple}

- Clear: Overwrite with one pass (may shorten device life); or use
  security erase.

- Purge: Use block erase or crypto erase; verify.

- Destroy: Shred or incinerate.

- Notes: Reset hidden areas first. Not all encryption works for purge;
  check specs. No degaussing.

#### SCSI SSDs (Parallel SCSI, SAS, etc.) {#scsi-ssds-parallel-scsi-sas-etc. .Heading-4_Purple}

- Clear: Overwrite with one pass.

- Purge: Use SCSI sanitise (block/crypto erase); or TCG interface for
  key change.

- Destroy: Shred or incinerate.

- Notes: Verify; reset configs. No degaussing.

#### NVM Express SSDs {#nvm-express-ssds .Heading-4_Purple}

- Clear: Overwrite with one pass.

- Purge: Use format command (user data or crypto erase); or TCG for key
  change.

- Destroy: Shred or incinerate.

- Notes: Verify; no degaussing.

#### USB Removable Media (e.g., Thumb Drives) {#usb-removable-media-e.g.-thumb-drives .Heading-4_Purple}

- Clear: Overwrite with at least two passes (pattern + complement).

- Purge: Often not supported; destroy instead.

- Destroy: Shred or incinerate.

- Notes: For high-risk, always destroy.

**Report incidents (e.g., improper disposal leading to compromise) per
the Incident Management Policy. [ISD003-Incident Reporting and
Management
Framework.pdf](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISD003-Incident%20Reporting%20and%20Management%20Framework.pdf?csf=1&web=1&e=3SKY6F)**

1.  
2.  
3.  
4.  

###  {#section-1 .Heading-3_Green}

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

  ----------------------------------------------------------------------------
  Version   Date         Author        Changes
  --------- ------------ ------------- ---------------------------------------
  0.1       28/08/2025   Head of       Initial Draft
                         Security      

  1.0       03/10/2025   Head of       Major version update, release for
                         Security      approval
  ----------------------------------------------------------------------------

### Approvals {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     03/10/2025     1.0       [CISP-101713](https://communityfibre.atlassian.net/browse/CISP-101713)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
