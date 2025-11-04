**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISP035**

**Cryptographic Controls Policy**

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

[Policy on the use of cryptographic controls
[3](#policy-on-the-use-of-cryptographic-controls)](#policy-on-the-use-of-cryptographic-controls)

[1. General principles [3](#general-principles)](#general-principles)

[2. Encryption of data in transit
[3](#encryption-of-data-in-transit)](#encryption-of-data-in-transit)

[Key management [3](#key-management)](#key-management)

[1. Roles and responsibilities
[4](#roles-and-responsibilities)](#roles-and-responsibilities)

[2. Regulation of cryptographic controls
[4](#regulation-of-cryptographic-controls)](#regulation-of-cryptographic-controls)

[Revisions Record Sheet
[5](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [5](#approvals)](#approvals)

### General Information {#general-information .Heading-3_Green}

### Document Objective {#document-objective .Heading-3_Purple}

The policy below is designed to ensure that cryptographic controls
(i.e., the use of encryption technologies) is applied in a consistent,
adequate, and proportionate manner and that key material is formally
managed.

**This document meets the following clauses:**

- Information Security Management System BS EN ISO/IEC 27001:2022 --
  A.8.24 Use of cryptography

### Policy on the use of cryptographic controls {#policy-on-the-use-of-cryptographic-controls .Heading-3_Green}

The purpose of this policy is to protect the confidentiality, integrity,
and availability of Community Fibre's Information by applying
appropriate levels of Cryptographic control.

### General principles {#general-principles .Heading-3_Purple}

1.  All critical or sensitive data transferred outside of Community
    Fibre must be encrypted.

2.  All removable media, including memory sticks, must be encrypted.

3.  Laptop hard drives must be encrypted.

4.  All remote access must take place via a secure tunnel protocol or
    encrypted terminal.

### Encryption of data in transit {#encryption-of-data-in-transit .Heading-3_Purple}

1.  Data classified as "Strictly Confidential" must be encrypted in
    transit.

2.  Data classified as "Confidential" should be encrypted wherever
    possible and practical.

3.  Data classified as "Public" may be sent unencrypted.

> Reference: Information Classification and Handling Policy
> ([ISP037-Information Classification and Handling
> Policy.pdf](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP037-Information%20Classification%20and%20Handling%20Policy.pdf?csf=1&web=1&e=KYcTIa))

### Key management {#key-management .Heading-3_Green}

1.  Encryption keys must be securely managed, preferably in a central
    location, such that all information encrypted by the organisation
    can be decrypted if required.

2.  Rules relating to encryption on removable media are contained within
    [ISP039-Remote Working
    Policy.pdf](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP039-Remote%20Working%20Policy.pdf?csf=1&web=1&e=SzRjAA)
    (Management of removable media)

3.  The strength of encryption to be used must be considered against the
    risks associated with the assets to be encrypted and a minimum of
    128 bits encryption is strongly recommended.

4.  Some technologies for VPN or TLS use AES 256-bit encryption and this
    is viewed as sufficiently secure.

### Key repository {#key-repository .Heading-3_Purple}

Public keys for persons accessing our services are managed within a key
repository. All modifications to public keys are traceable.

Access to this repository is limited the Community Fibre\'s technical
employees. The Head of Security or authorised delegate is responsible
for the maintenance of the repository. It\'s crucial that the integrity
of the key information is preserved, as such the Head of Security or
authorised delegate will be responsible for reviewing changes to the
repository and signing known good states.

### Key addition {#key-addition .Heading-3_Purple}

- request made to Head of Security or authorised delegate to add key;

- Head of Security or authorised delegate verifies that key meets the
  key specification;

- if key meets specification, then the key is added to the key
  repository;

- if the key does not meet specification, then the requester must
  provide a key that does meet specification.

### Key revocation {#key-revocation .Heading-3_Purple}

- Owner of the key being revoked advises Head of Security or authorised
  delegate;

- Head of Security or authorised delegate marks the key as revoked in
  authoritative key records and removes the key from all services;

- Owner supplies Head of Security or authorised delegate with new key;

- Head of Security or authorised delegate adds a new key to the
  authoritative key records;

- Head of Security or authorised delegate ensures that all services use
  the new public key.

### Key removal {#key-removal .Heading-3_Purple}

- request made to Head of Security or authorised delegate to remove key;

- Head of Security or authorised delegate removes the key from the
  repository.

### Key specifications {#key-specifications .Heading-3_Purple}

The key must be of the type RSA and be 2048 bits. The private key must
have a passphrase which at least conforms to the minimum requirements
for passwords.

### Key storage {#key-storage .Heading-3_Purple}

- Private keys must be stored in encrypted form on a local device.

- Keys themselves are stored in an encrypted container that\'s decrypted
  and accessed during the user\'s login session.

### Key backup {#key-backup .Heading-3_Purple}

In order to ensure that information can be retrieved in the event of a
key being lost or forgotten, backups of the keys will be taken and
stored in either an electronic location protected by encryption or in a
physically secure storage facility (e.g. a safe). The type and nature of
such backup storage will be determined by risk assessment.

### Roles and responsibilities {#roles-and-responsibilities .Heading-3_Purple}

1.  

2.  

3.  

4.  

5.  

6.  

7.  

8.  

9.  

10. 1.  Ensuring that the organisation maintains the highest practicable
        standard of encryption is the responsibility of the Head of
        Security.

    2.  Key management responsibility lies with the IT and Network
        Technology administrators.

    3.  All individuals are responsible for ensuring that data is
        suitably encrypted before leaving the Community Fibre's
        premises.

### Regulation of cryptographic controls {#regulation-of-cryptographic-controls .Heading-3_Purple}

For any use of cryptographic controls exported outside of the UK the
following considerations are made:

1.  

2.  

3.  

4.  

5.  

6.  

7.  

8.  

9.  

10. 

11. 1.  Regulatory controls for any country to which data is exported
        outside the UK must be checked to ensure that cryptographic
        legislation will not be contravened.

    2.  Restrictions on import and/or export of computer hardware and
        software for performing cryptographic functions (e.g., under the
        Wassennaar Arrangement for export controls for conventional arms
        and dual-use goods and technologies).

    3.  Restrictions on import and/or export of computer hardware and
        software which is designed to have cryptographic functions added
        to it.

    4.  Restrictions on the usage of encryption; and

    5.  Mandatory or discretionary methods of access by the countries'
        authorities to information encrypted by hardware or software to
        provide confidentiality of content.

#### Consequences of non-compliance with this policy

Any non-compliance with or breach of policy may lead to investigation
and action in line with the organisational Disciplinary Policy
(Community Fibre - Employee Handbook 2023 - v3.pdf).

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

+---------+------------+------------+--------------------------------------+
| Version | Date       | Author     | Changes                              |
+=========+============+============+======================================+
| 0.1     | 29/03/2021 | ISO        | Initial Draft                        |
+---------+------------+------------+--------------------------------------+
| 0.2     | 15/12/2021 | ISO        | Added information handling and       |
|         |            |            | protective measures,                 |
|         |            |            |                                      |
|         |            |            | Added description ("What we do"),    |
|         |            |            | last paragraph, describing handling  |
|         |            |            | requirements.                        |
+---------+------------+------------+--------------------------------------+
| 1.0     | 21/03/2022 | ISO        | Major version number update to 1.0   |
|         |            |            | ready for approvals                  |
+---------+------------+------------+--------------------------------------+
| 1.1     | 09/09/2022 | ISO        | Updated business address and         |
|         |            |            | document classification, formatting  |
+---------+------------+------------+--------------------------------------+
| 1.2     | 07/11/2023 | Head of    | Document template update, employee   |
|         |            | Security   | handbook version update              |
+---------+------------+------------+--------------------------------------+
| 1.4     | 17/09/2024 | Head of    | Standard version update, TOC added,  |
|         |            | Security   | no other changes                     |
+---------+------------+------------+--------------------------------------+
| 1.5     | 15/08/2025 | Head of    | Standard version update, key         |
|         |            | Security   | management provisions added.         |
+---------+------------+------------+--------------------------------------+

### Approvals {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     15/09/2025     1.5       [CISP-101362](https://communityfibre.atlassian.net/browse/CISP-101362)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
