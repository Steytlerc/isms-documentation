**INFORMATION SECURITY MANAGEMENT SYSTEM**

**Conforming to:**

**Information Security Management System BS EN ISO/IEC 27001:2022**

**ISP015**

**Network Security Policy**

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

### Contents {#contents .TOC-Heading}

[Glossary [3](#glossary)](#glossary)

[References [4](#references)](#references)

[General Information [4](#general-information)](#general-information)

[Document Objective [4](#document-objective)](#document-objective)

[Policy [4](#policy)](#policy)

[Scope and principles [4](#scope-and-principles)](#scope-and-principles)

[1. Network architecture and segmentation
[5](#network-architecture-and-segmentation)](#network-architecture-and-segmentation)

[2. Management Plane [8](#management-plane)](#management-plane)

[3. Signalling Plane [10](#signalling-plane)](#signalling-plane)

[4. Customer Premises Equipment
[11](#customer-premises-equipment)](#customer-premises-equipment)

[5. Virtualisation [12](#virtualisation)](#virtualisation)

[6. Network oversight functions
[14](#network-oversight-functions)](#network-oversight-functions)

[7. Exposed Edge [16](#exposed-edge)](#exposed-edge)

[8. Retaining national resilience and capability
[17](#retaining-national-resilience-and-capability)](#retaining-national-resilience-and-capability)

[Revisions Record Sheet
[18](#revisions-record-sheet)](#revisions-record-sheet)

[Approvals [18](#approvals)](#approvals)

### Glossary {#glossary .Heading-3_Green}

  -----------------------------------------------------------------------------------
  Ref#         Term               Description                Reference
  ------------ ------------------ -------------------------- ------------------------
  []{#i        Security Critical  Any function of the        [CoP Section 1.3, pages
  .anchor}i                       network or service whose   13]{.underline}
                                  operation is likely to     
                                  have a material impact on  
                                  the proper operation of    
                                  the entire network or      
                                  service or a material part 
                                  of it                      

  ii           Sensitive          Facilities or rooms        
               processing         containing sensitive data  
               areas/facilities   or security critical       
                                  infrastructure.            

  iii          Sited              Fix or build (something)   
                                  in a particular place.     

  []{#iv       Management Plane   System that provides       [CoP Section 2.7, pages
  .anchor}iv                      management information for 17-21]{.underline}
                                  the network elements.      

  []{#v        Signalling Plane   Protocols for control and  [CoP Section 2.70, page
  .anchor}v                       support of the             27-29]{.underline}
                                  transmission plane         
                                  functions, controls the    
                                  access connections to the  
                                  network, controls the      
                                  routing of signalling      
                                  connections                

  []{#vi       Network Oversight  Oversee and control the    [CoP Section 1.6, pages
  .anchor}vi   Functions          security critical          13-15]{.underline}
                                  functions, includes        
                                  network monitoring and     
                                  analysis functions,        
                                  generates, stores or       
                                  processes data necessary   
                                  for the correct            
                                  functioning or             
                                  configuration of security  
                                  critical functions,        
                                  controls access to         
                                  security critical          
                                  functions                  

  vii          Virtualisation     Mesh of interconnected     [CoP Section 2.31, pages
               fabric             (virtual) switches,        22-27]{.underline}
                                  servers and storage as a   
                                  single logical entity,     
                                  enabling resource sharing  
                                  resilience and simplified  
                                  management.                

  viii         Exposed edge       Equipment that is either   [CoP Section 2.88, pages
                                  within customer premises,  30-31]{.underline}
                                  directly addressable from  
                                  customer/user equipment,   
                                  or is physically           
                                  vulnerable. E.g.,          
                                  equipment in road‑side     
                                  cabinets                   
  -----------------------------------------------------------------------------------

### References {#references .Heading-3_Green}

  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
   Ref#   Document                        Reference
  ------- ------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
   **1**  ISO/IEC 27001:2022              [[BS EN ISO_IEC 27001_2023+A1_2024 (7 Apr 2025 9-38am
                                          UTC).pdf]{.underline}](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Standards%20Documentation/27000%20-%202022/BS%20EN%20ISO_IEC%2027001_2023+A1_2024%20(7%20Apr%202025%209-38am%20UTC).pdf?csf=1&web=1&e=oPNJ1I)

   **2**  The Electronic Communications   [[The Electronic Communications (Security Measures) Regulations 2022]{.underline}](https://www.legislation.gov.uk/uksi/2022/933/contents/made)
          Security Measures Regulations   
          2022 (ECR)                      

   **3**  Telecommunications Security     [[Telecommunications Security Code of Practice]{.underline}](https://assets.publishing.service.gov.uk/media/6384d09ed3bf7f7eba1f286c/E02781980_Telecommunications_Security_CoP_Accessible.pdf)
          Code of Practice (CoP)          
  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### General Information {#general-information .Heading-3_Green}

### Document Objective {#document-objective .Heading-3_Green}

> This Network Security Policy establishes requirements for securing
> Community Fibre Limited\'s operational and business networks, ensuring
> the confidentiality, integrity, and availability of information and
> services. The aim is to manage risks associated with unauthorised
> access, data interception, denial-of-service attacks, and signalling
> threats, while supporting resilient telecom operations. This policy
> aligns with NCSC guidance on network security and addresses business
> needs, security risks, and regulatory requirements.
>
> **This document meets the following clauses:**

- Information Security Management System ISO/IEC 27001:2022
  \[[1](#glossary)\]-- A.8.20: Network security; A.8.21: Security of
  network services; A.8.22: Segregation of networks

- The Electronic Communications Security Measures Regulations 2022
  \[[2](#glossary)\]-- Secure network architecture (3. (1)); protect
  data in transit (4. (1)); protect against external threats (5. (1));
  secure by design 3(1)(a)

### Policy {#policy .Heading-3_Green}

### Scope and principles {#scope-and-principles .Heading-3_Green}

> This policy applies to all network components, including managed
> services, hardware, software, connections, and services within
> Community Fibre\'s infrastructure. It encompasses platform services
> like AWS, core networks, edge devices (e.g., CPE, roadside cabinets),
> wireless networks, remote access, and third-party interconnections. It
> covers the full lifecycle of network assets.
>
> Key principles, informed by NCSC guidance and the Telecommunications
> Security Code of Practice:

- Use segmentation, encryption, monitoring, and threat hunting to
  protect against threats, ensuring the network reduces security
  compromises through proactive design, redesign of existing parts, and
  ongoing maintenance.

- Controls selection must be appropriate and proportionate to asset
  sensitivity and risks, with flexibility based on CoP guidance
  (\'shall\' for mandatory solutions, \'should\' for best practices,
  \'may\' for alternatives).

- Verify all access and traffic; deny-by-default.

- Ensure high availability and rapid recovery.

- Align with access controls -[Access Control
  Policy](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISP010-Access%20Control%20Policy.pdf?csf=1&web=1&e=XxV42z)
  and [ISD009-Physical Security
  Standard](https://communityfibre.sharepoint.com/:b:/r/sites/isms/Shared%20Documents/General/ISMS%20Policy%20Documents/Approved/ISD009-Physical%20Security%20Standard.pdf?csf=1&web=1&e=o8Pvcv).

- Maintain national resilience by designing for operation without
  reliance on foreign entities, including reducing dependencies on
  third-party suppliers.

**Overall responsibility for Community Fibre network security is managed
by the Network Technology and IT Technology in collaboration with the
Security Operations team, and oversight from the ISMS Board.**

### Network architecture and segmentation {#network-architecture-and-segmentation .Heading-3_Green}

Objectives are derived from the Telecommunications Security Code of
Practice -- 2. Network Architecture \[3\] and The Electronic
Communications Security Measures Regulations 2022 - Regulation 3
\[[2](#glossary)\]. These objectives aim to ensure that public telecoms
providers design, construct, redesign, and maintain networks in a manner
that reduces the risks of security compromises. They emphasise
segmentation through security zones, the isolation of critical planes
(e.g., signal and management plane \[iv\]), the protection of
security-critical \[[i](#i)\] and oversight functions, and proportionate
risk management. Objectives are categorised for clarity and include
references to relevant document sections for traceability.

1.  **Risk identification and documentation**

<!-- -->

a)  Risks to the network and individual functions shall be identified
    and assessed, and consider factors such as the presence of sensitive
    data, whether the function is security critical \[[i](#i)\],
    equipment location, and exposure to incoming signals. Records of
    these risks are reviewed at least annually; records are retained for
    3 years. (Regulation 3(3)(a)-(b) and (4))

b)  The core and business networks\' exposure to incoming signals should
    be mapped and documented, including interfaces and entry points, to
    minimise unnecessary attack surfaces. (Regulation 3(3)(c) and (4))

    1.  **Secure design and construction principles**

<!-- -->

a)  Core and business networks shall be designed and constructed (and
    redesigned where necessary) to protect security-critical \[[i](#i)\]
    functions, ensuring appropriate equipment placement and safeguards
    against compromises that could materially impact network operation.
    (Regulation 3(1)-(3)(d) \[[2](#glossary)\] and Key Concepts 1.3-1.5
    \[[3](#glossary)\])

b)  Procurement, configuration, management, and testing of equipment
    shall contain measures that prioritise security-by-default and are
    aligned with vendor hardening guides. (Regulation 3(3)(e)
    \[[2](#glossary)\])

c)  Networks should be architected to enable independent risk
    identification and operation without reliance on external (non-UK)
    persons, equipment, or data, in preparation for scenarios where such
    reliance poses a risk. (Regulation 3(3)(f) \[[2](#glossary)\])

    1.  **Segmentation and isolation**

<!-- -->

a)  Core and business networks shall be divided into security zones
    (e.g., corporate, administrative, and operational) using firewalls,
    VLANs, or other isolation techniques to isolate high-risk areas,
    ensuring that compromises in one part (e.g., corporate functions) do
    not propagate to others, such as the operational network.
    (Regulation 3(5) \[[2](#glossary)\] and Key Concepts 2.4, 2.18-2.19
    \[[3](#glossary)\])

b)  The core network management plane \[[iv](#iv)\]shall be isolated
    from corporate or external functions, including the logical or
    physical separation of workstations for office productivity (e.g.,
    email, web access) from those accessing the management plane
    \[[iv](#iv)\]. (Key Concepts paragraphs 2.7-2.20)

c)  Communications within and across planes (e.g., management planes
    \[[iv](#iv)\]) should be restricted to only necessary connections,
    defaulting to allowing outbound connections from administrative
    functions to network equipment while blocking unnecessary inbound
    traffic. (Key Concepts paragraphs 2.24-2.25)

    1.  **Protection of critical functions**

<!-- -->

a)  Network oversight functions \[[vi](#vi)\] (e.g., element managers,
    orchestrators, security gateways, monitoring systems) that control
    or oversee security-critical \[[i](#i)\] functions shall be deployed
    in dedicated and segregated networks or VLANs, rapidly patched,
    monitored in real-time, have minimised attack surfaces, and are
    rebuilt periodically to a known-good state. (Key Concepts 1.6-1.14
    and 1.18\[[3](#glossary)\])

b)  Hypervisors, physical servers, virtual workloads, and orchestration
    software should be classified as security critical \[[i](#i)\] where
    they materially impact operations. Components are isolated and
    segmented; for example, vCenter should be deployed on a dedicated
    host, not hosted on the virtualisation fabric that it manages. (Key
    Concepts 1.15-1.17)

    1.  **Secure administration and access controls**

<!-- -->

a)  All administrative access shall be authorised, time-limited, and
    linked to a specific purpose, and have multi-factor authentication
    enforced with separate devices for token generation, with SMS
    disabled. (Key Concepts 2.21-2.22 \[[3](#glossary)\])

b)  All management traffic shall use secure protocols (e.g., SSH, HTTPS)
    (Key Concepts 2.23 \[[3](#glossary)\])

c)  Third-party administrators or managed service access shall be
    segmented, and security requirements contractually enforced to
    ensure they meet equivalent principles for management plane
    \[[iv](#iv)\] access. (Key Concepts 2.8 and 2.26 \[[3](#glossary)\])

    1.  **Maintenance, monitoring, and resilience**

<!-- -->

a)  Network architecture shall be maintained to continuously reduce
    compromise risks, including regular reviews of segmentation
    effectiveness and adjustments for emerging threats or technologies.
    (Regulation 3(1)(c) \[[2](#glossary)\], Key Concepts 2.3-2.6
    \[[3](#glossary)\], ongoing architectural maturity.)

b)  Monitoring and analysis shall be integrated into the architecture,
    prioritising real-time oversight of network oversight functions
    \[[vi](#vi)\] and anomalous activity detection. (Key Concepts
    1.13-1.14 \[[3](#glossary)\] and cross-references to 5.3-5.23)

c)  For equipment that reaches the end of life or is identified
    explicitly for removal, risk assessments shall be conducted to
    ensure proportionate measures or accelerated replacement. No
    exemptions shall be allowed to undermine overall architecture
    security. (Key Concepts 2.6)

### Management Plane {#management-plane .Heading-3_Green}

The management plane \[[iv](#iv)\] encompasses all systems, interfaces,
and processes used for the configuration, monitoring, administration,
and maintenance of network infrastructure. Controls for unauthorised
access and mitigating risks that could lead to security compromises are
critical.

a)  

b)  1.  **Secure management plane access and operations**

<!-- -->

a)  Network architecture shall be designed so that workstations used for
    significant security changes critical \[i\] functions are shielded
    from direct exposure to incoming signals, unless strictly necessary
    for authorised remote operations. (Regulation 4(4)(a)(i)-(ii))

b)  Segmentation shall be implemented to separate management traffic
    from user or production traffic, using firewalls, VLANs, or VPNs
    where applicable. (CoP M2.04)

c)  Privileged Access Workstations shall be used for high-risk
    privileged access (e.g., Tier 0/1 - ISP013-Privileged Access Rights
    Policy) (CoP M2.03)

d)  Third-party supplier access shall be provisioned via compliant
    physical PAWs authenticated through the Community Fibre's identity
    provider, with remote access restricted to jump boxes. (CoP M2.06)

    1.  **Secure access to the network or service**

<!-- -->

a)  Responsibility for security measures should be assigned to competent
    personnel with a comprehensive understanding of network or service
    operations. They should be trained annually on the risks and
    controls associated with privileged access. (Regulation 8(2)(a))

b)  Multi-factor authentication shall be mandatory for all accounts
    capable of altering security-critical \[[i](#i)\] functions, with
    regular audits to enforce compliance; hardcoded or default
    credentials are prohibited. (Regulation 8(2)(b), 8(5)(c))

c)  Dual approval should be processed for significant or manual
    modifications to security-critical \[i\] functions. Changes must be
    proposed by one authorised individual and approved by another
    responsible party (segregation of duties). (Regulation 8(2)(c))

d)  Default credentials should be treated as publicly known for risk
    assessment and implement compensating controls. (Regulation
    8(2)(d)-(e); CoP M2.05)

e)  All information that could facilitate unauthorised access (e.g.,
    passwords, keys, or configuration files) should be stored in secure
    vaults with automated rotation (e.g., every 30 days for Tier 0),
    using encryption and access controls. (Regulation 8(2)(f), 8(5)(a))

f)  Where practical, automation should be used for changes to
    security-critical \[[i](#i)\] functions. (Regulation 8(2)(g))

g)  Privileged access shall be granted based on business need and risk,
    using Just-In-Time (JIT) and Just-Enough-Administration (JEA) for
    temporary, task-specific elevations; rights shall be granted to
    dedicated privileged accounts, separate from standard user accounts,
    with no credential reuse. (Regulation 8(4), 8(5)(b)-(e), 8(1)-(3),
    ISP013 Sections 2 (Scope and Principles), 4 (Granting and Managing
    Privileged Access Rights), and 9 (Regulatory Requirements).

    1.  **Isolation mechanisms**

<!-- -->

a)  Procedures shall be designed and maintained to isolate
    security-critical \[[i](#i)\] functions from signals deemed unsafe,
    based on reasonable grounds such as source verification or anomaly
    detection. (Regulation 8(3))

b)  Intrusion detection systems or similar tools should be deployed to
    monitor management plane \[[iv](#iv)\] traffic for anomalies. (CoP
    M2.02)

c)  Regularly scheduled testing should be done of isolation capabilities
    through simulations or penetration testing to verify effectiveness.
    (Regulation 8(3))

d)  All privileged sessions (e.g., video/keystrokes for high-risk) shall
    be controlled and recorded, stored away from PAWs to enable session
    replay for investigations. (CoP M2.02, Regulations 8(3) (pages 6-7);
    ISP013 Section 6 (Monitoring, Auditing, and Session Management)

    1.  **Attack surface management**

<!-- -->

a)  All active management protocols shall be documented, and those not
    required for operations shall be disabled, such as Telnet or
    unencrypted HTTP. (CoP M2.04)

b)  Justifications for any retained protocols should be documented,
    reviewed regularly and considered during change management
    processes. (CoP M2.04)

c)  Least-privilege principles should be applied to protocol usage;
    essential services are exposed proportionately to asset sensitivity.
    (CoP M2.04)

    1.  **Management and third-party accountability**

<!-- -->

a)  Responsibilities for managing the Community Fibre infrastructure
    shall be clearly defined, including the regular review and oversight
    of third-party access and compliance with security standards. (CoP
    M2.06)

b)  Contractual clauses shall require suppliers to adhere to equivalent
    security measures, with rights for audits and reporting. (CoP M2.06)

c)  All management tools and services shall be maintained in an asset
    registry and their security posture reviewed periodically.

d)  At least two break glass accounts should be maintained for use in
    emergencies, independent of main authentication, with post-use
    password changes, notifications, audits, and incident response.
    (Regulation 8(1))

e)  Privileged users must report anomalies, use separate accounts for
    elevated tasks, and complete annual specialised training.
    (Regulation 8(5)(e))

### Signalling Plane {#signalling-plane .Heading-3_Green}

The signalling plane \[[v](#v)\] consists of protocols used for the
control and support of transmission plane functions, including enabling
network connections, managing user mobility, setting up calls, and
routing messages. Securing this plane is essential to prevent malicious
signalling attacks, unauthorised access, data leaks, and disruptions to
network availability or performance.

a)  

b)  

c)  1.  **Interfaces, equipment, and impacts**

<!-- -->

a)  All incoming and outgoing signalling interfaces shall be mapped and
    documented (e.g., SIP and BGP) along with equipment that processes
    external signalling and could be impacted by malicious signalling.
    (CoP M3.01- M3.02)

b)  Network equipment and any data that could be compromised through
    malicious signalling shall be identified and risk assessed. (CoP
    M3.02- M3.03)

    1.  **External signalling**

<!-- -->

a)  Incoming signals over direct connections shall be treated as
    untrusted, regardless of source. (CoP M3.04)

b)  Incoming signal with internal source addresses at edge nodes should
    be blocked to prevent spoofing. (CoP M3.05)

c)  Outgoing signals with source addresses not intended to transit
    external networks should be blocked. (CoP M3.09)

d)  External exposure of customer data, identifiers, and network
    topology via signalling protocols should be minimised. (CoP M7.02)

e)  Signalling records containing sensitive data should be protected
    from misuse and encrypted to prevent unauthorised extraction. (CoP
    M12.02)

    1.  **Secure BGP routing**

<!-- -->

a)  BGP updates should be monitored for potential misuse or anomalies.
    (CoP M3.11)

b)  The recipient of Community Fibre outgoing BGP routing updates must
    be able to validate that updates originate from legitimate owners.
    (CoP M7.03)

c)  BGP route updates must be validated to originate from legitimate
    owners, where information is available. (CoP M7.04)

    1.  **Monitoring, analysis and testing**

<!-- -->

a)  Incoming and outgoing signalling traffic shall be monitored and
    analysed for anomalies, integrating with protective monitoring
    systems. (CoP M12.01)

b)  Community Fibre shall alert other providers or authorities of
    malicious signalling. (CoP M12.04)

c)  Community Fibre shall perform security assessments and offensive
    testing on all external signalling interfaces, including new
    equipment before production deployment, and at least annually on
    existing equipment. (CoP M12.05)

### Customer Premises Equipment {#customer-premises-equipment .Heading-3_Green}

a)  

b)  

c)  

d)  1.  **Baseline security**

<!-- -->

a)  A secure default configuration that limits inbound connections by
    default shall be deployed on all CPE. (CoP Key Concepts 3.37)

b)  All CPE shall receive regular security updates throughout the
    device\'s lifetime. (CoP Key Concepts 3.37)

c)  Proactive measures such as enabling auto-update capabilities and
    replacing out-of-support CPE shall be taken. (CoP Key Concepts 3.38)

d)  CPE shall contain credentials that are unique to that CPE and not
    guessable from metadata. (CoP M9.01)

    1.  **Product support**

<!-- -->

a)  Community Fibre shall ensure that all CPE provided to customers is
    still supported by the network equipment supplier. (CoP M9.02)

b)  Customers shall be informed before and once the equipment goes out
    of support and proactively offered a replacement as soon as
    reasonably practicable. (CoP M9.02)

    1.  **Product management**

<!-- -->

a)  CPE management interfaces shall only be accessible from specified
    management locations. (CoP M9.03)

b)  Management of the CPE shall use a secure protocol (e.g. TLS 1.2 or
    newer). (CoP M9.04)

c)  Customer-facing management interfaces shall only be accessible from
    within the customer's network. (CoP M9.04)

    1.  **Product security requirements**

<!-- -->

a)  CPE security should align with the Product Security and
    Telecommunications Infrastructure Act requirements, such as no
    universal default passwords, vulnerability reporting mechanisms, and
    transparency on security update durations. It may include additional
    protections beyond default configurations to mitigate risks from
    customer adjustments. (CoP Key Concepts 3.34)

### Virtualisation {#virtualisation .Heading-3_Green}

Virtualisation encompasses the deployment of virtual network functions
(VNFs), containers, virtual machines and virtualisation fabrics (e.g.,
hypervisors, orchestration tools)

a)  

b)  

c)  

d)  

e)  1.  **Isolation and segregation in virtualisation fabrics**

<!-- -->

a)  Virtualisation fabrics shall enforce separation between trust
    domains using host pools and affinity rules to prevent lateral
    movement. (CoP M13.01)

b)  Physically separate ports shall be used to segregate internal and
    external interface network traffic as part of the fabric. (CoP
    M13.06)

c)  Communication between physical hosts shall be restricted except for
    virtual workloads; host interfaces shall be locked down to allow
    only management or virtualisation function connections. (CoP M13.03)

d)  Containers running on a single host shall be regarded as within a
    single trust domain. (CoP M13.16-17)

e)  Hypervisor cut-throughs shall be used only if all virtual functions
    in the host or host-pool are placed in a single trust domain. (CoP
    Key Concepts page 26.)

    1.  **Host integrity and secure boot**

<!-- -->

a)  Virtualisation fabrics shall support secure boot using hardware
    root-of-trust (TPM) and ensure that only authorised virtual
    functions are enabled and are always fully patched. (CoP M13.01)

b)  Patching of fabrics shall not negatively impact network
    functionality. (CoP M13.02)

c)  Only known physical hosts shall be allowed to be added to the
    virtualisation fabric. (CoP M13.04)

    1.  **Monitoring and anomaly detection**

<!-- -->

a)  Virtualisation fabrics shall allow monitoring of operating system,
    application, and virtual machine processes and flow behaviour, using
    either host-based monitoring or by forwarding OS-level logging data.
    (CoP Key Concepts 5.14)

b)  Real-time monitoring of changes and signs of exploitation in
    virtualised oversight functions should be enabled. (CoP Key Concepts
    1.14)

c)  Manual administration of the virtualisation fabric (e.g., access to
    a command line on host infrastructure) shall produce an immediate
    alert. (CoP M19.07)

    1.  **Secure access controls and administration**

<!-- -->

a)  Host administration shall be monitored and limited to the smallest
    number of trusted administrators, with network interfaces accepting
    only authorised management connections. (CoP Key Concepts 2.47)

b)  Modifications to databases and systems defining network operation
    shall require sign-off by two authorised persons. (CoP M13.05)

c)  Administrative access to virtualised components shall require
    multi-factor authentication, with the second factor delivered via a
    separate device. (CoP Key Concepts 2.21)

    1.  **Secure orchestration and management**

<!-- -->

a)  Orchestration tools managing the fabric shall be treated as network
    oversight functions \[[vi](#vi)\] and not hosted on the fabric they
    operate, for resilience and recovery. (CoP Key Concepts 2.48)

b)  Virtualisation fabric shall be built and updated using automation as
    far as possible, and all automated processes must produce audit
    logs. (CoP M19.04)

c)  Where possible, only automated and verifiable methods of
    configuration shall be used for administration of the virtualisation
    fabric (authorised API calls etc) (CoP M19.05)

d)  Where possible, administration of the virtualisation fabric shall be
    automated during regular operation. (CoP M19.06)

**\**

1.  **Attack surface management**

<!-- -->

a)  Virtual fabric shall be configured with limited exposure of
    workloads (e.g., span ports disabled by default) (CoP M13.07)

<!-- -->

a)  Virtual networks shall not use hardcoded MAC addresses. (CoP M13.08)

<!-- -->

b)  In environments where physical security cannot be guaranteed (data
    centres, exchanges, exposed edge), additional measures should be
    taken, e.g., data encrypted at rest. (CoP M13.09)

    1.  **Secure storage of sensitive data**

<!-- -->

a)  All non-ephemeral secrets (long-lived secrets) like static API keys,
    database passwords, SSH private keys, and root certificates shall be
    stored in hardware-backed secure storage. Where this measure cannot
    be applied to existing networks and services, mitigating steps must
    be documented. Security Operations will provide guidance. (CoP
    M19.01)

### Network oversight functions {#network-oversight-functions .Heading-3_Green}

Systems and processes that monitor, configure, or influence the
operation of the security critical \[[i](#i)\] functions, such as
performance monitoring tools, configuration management databases,
security event management systems, and orchestration platforms. These
functions are essential as their compromise could enable widespread
attacks or disruptions. Examples include:

- element managers;

- virtualisation orchestrators;

- management systems (e.g. jump boxes);

- security functions (e.g. firewalls at the edge of a security zone);

- root authentication services (e.g. Active Directory, LDAP);

- Multi-factor authentication services;

- security gateways (e.g. supporting the management plane
  \[[iv](#iv)\]);

- audit and monitoring systems (including network quality monitoring of
  speech and data); and

- Operational Support Systems (OSS).

a)  

b)  

c)  

d)  

e)  

f)  1.  **Identify all network oversight functions**

<!-- -->

a)  All oversight functions shall be identified, including those that
    monitor or influence network operation (e.g., performance
    monitoring, configuration databases, security tools). (CoP Key
    Concepts 2.85)

b)  Oversight functions shall be classified based on their potential
    impact, prioritising those that could lead to widespread compromise,
    e.g., the compromise of a root identification provider would be
    catastrophic and should be robustly locked down and prioritised for
    patching, logging and monitoring. (CoP Key Concepts 1.9-1.18,
    M15.01)

c)  Where the security of the physical environment (e.g. within the
    exposed edge, or within a shared data centre/exchange) cannot be
    guaranteed, the network oversight functions \[[vi](#vi)\] shall not
    be deployed. (CoP M15.05)

    1.  **Protection from unauthorised or unsafe signals**

<!-- -->

b)  Oversight functions management planes \[[iv](#iv)\] shall be
    isolated from internal and external networks, including other
    management planes \[[iv](#iv)\], unless strictly necessary for
    operations (CoP M15.09)

c)  Where exposure is necessary, signals shall be limited to authorised
    changes only and segmented to shield functions. (CoP M15.09)

d)  Regular risk and at least annual assessments shall be conducted to
    verify isolation effectiveness, updating architectures as needed.
    (CoP M19.06)

    1.  **Secure access to oversight functions**

<!-- -->

a)  General-purpose admin tools (e.g., general-purpose jump box) or
    shared systems (e.g., accessing directly from a general-purpose
    VLAN) shall not be used to manage network oversight functions.
    Dedicated management functions shall be utilised to oversee network
    operations. (CoP M15.08)

b)  Management functions (e.g., jump box) for oversight functions shall
    only be accessible from designated PAWs. (CoP M15.07)

c)  Access controls shall be implemented per ISP010-Access Control
    Policy, ISP013-Privileged Access Rights Policy.

d)  Automation shall be used for changes where possible, with manual
    modifications requiring dual approval. (CoP M15.10)

e)  Privileged access should be reviewed periodically (every 6 months,
    performed by Network and Security Operations), revoking unnecessary
    permissions. (CoP M15.06)

f)  Oversight functions shall be integrated with centralised identity
    management systems for consistent enforcement. (CoP M15.07)

g)  Network oversight functions \[[vi](#vi)\] shall only be managed by a
    minimal set of trusted privileged users. (CoP M15.06)

    1.  **Monitoring and anomaly detection**

<!-- -->

a)  Oversight functions shall be monitored for anomalous or unsafe
    activity, and shall be integrated into monitoring systems (e.g.,
    SIEM tools). (CoP M15.11,12)

b)  Real-time alerts should be enabled for suspicious patterns in
    oversight function logs, with automated response protocols where
    feasible, with procedures to isolate functions from unsafe signals
    upon detection of anomalies. (CoP M15.11,12)

c)  Attack simulations or penetration tests should be conducted at least
    annually on oversight functions to validate monitoring
    effectiveness. (CoP M15.11)

d)  Changes to network oversight functions shall be monitored in
    real-time. (CoP M15.11)

    1.  **Resilience and recovery**

<!-- -->

a)  Oversight functions shall be designed with resilience in mind,
    including redundancy and failover mechanisms to prevent single
    points of failure. The service that runs network oversight functions
    \[vi\] shall be rebuilt to a current, good state every 2 years. PAWs
    and jump-boxes shall be rebuilt every year. (CoP M15.02-03)

b)  Secure backups shall be kept of configurations and data, testable
    for recovery. CoP Key Concepts 1.11)

### Exposed Edge {#exposed-edge .Heading-3_Green}

The exposed edge of the network refers to the equipment that is either
located within customer premises, directly addressable from
customer/user equipment, or is physically vulnerable. Physically
vulnerable equipment includes equipment in roadside cabinets. For
example, the following equipment is typically considered part of the
exposed edge:

- Customer premises equipment (CPE) is equipment supplied to customers
  which is used, or intended to be used, as part of the network or
  service. This excludes consumer electronic devices such as mobile
  phones and tablets, but does include devices such as routers, edge
  firewalls, SD‑WAN equipment, and fixed wireless access kit.

- Optical line terminal (OLT) equipment; and

- Multi‑service access node / digital subscriber line access multiplexer
  (MSAN/DSLAM) equipment.

a)  

b)  

c)  

d)  

e)  

f)  

g)  1.  **Identify all exposed edge equipment**

<!-- -->

a)  Equipment shall be identified and steps taken to ensure that the
    compromise or disruption of parts of the exposed edge would not be a
    significant incident. (CoP Key Concepts 2.89)

b)  The exposed edge shall be physically and logically segregated from
    security-critical \[[i](#i)\] functions and ensure no sensitive data
    is stored on devices. (CoP Key Concepts 2.90)

c)  Equipment in exposed locations shall be protected against physical
    tampering using locks, enclosures, or barriers proportionate to the
    risk. Secure boot mechanisms should be implemented for all network
    elements on the exposed edge to enable restoration to a "known-good"
    state without requiring equipment replacement. (CoP Key Concepts
    2.91)

### Retaining national resilience and capability {#retaining-national-resilience-and-capability .Heading-3_Green}

UK\'s telecommunications networks must withstand disruptions, including
those from supply chain failures, geopolitical events, or cyber threats.
This involves maintaining UK-based capabilities, contingency planning,
secure data management, and robust governance to support ongoing
operations.

a)  

b)  

c)  

d)  

e)  

f)  

g)  

h)  1.  **UK-based technical capability for network operations**

<!-- -->

a)  UK-based technical capability shall be retained to provide subject
    matter expertise on UK network operations and risks. (CoP M21.03)

b)  As far as is reasonably practical, equipment performing network
    oversight functions \[[vi](#vi)\] should be located in the UK and
    operated by UK-based staff. (CoP M21.03)

c)  A UK-based capability shall be used to assess the risks of security
    compromise of the network, which includes (CoP Key Concepts 2.96):

    a.  storing security and audit logs outside the UK

    b.  using overseas staff for procurement of hardware and software

    c.  relying on staff, equipment or data outside the UK

    d.  relying on third-party suppliers to ensure that basic first- and
        second-line support is available from them for the required
        period, where offshored expertise is lost.

    <!-- -->

    1.  **UK-based technical capability for network operations**

<!-- -->

a)  Contingencies should be maintained in the event of further locations
    being added to the Schedule of the Electronic Communications
    (Security Measures) Regulations 2022. (CoP M21.01)

b)  In the event of loss of international connections, including
    fixed/mobile data to UK peering points, mobile voice, and text-based
    mobile messaging, the ability to maintain UK network connectivity
    for one month shall be maintained. (CoP M21.06)

c)  Should international bearers fail, the ability to transfer into the
    UK functions required to maintain an operational service shall be
    maintained. (CoP M21.07)

### Revisions Record Sheet {#revisions-record-sheet .Heading-3_Green}

  ----------------------------------------------------------------------------
  Version   Date         Author         Changes
  --------- ------------ -------------- --------------------------------------
  0.1       05/08/2025   Head of        Initial Draft as supporting policy to
                         Security       ISP010.

  1.0       03/10/2025   Head of        Major version update, release for
                         Security       approval

                                        

                                        

                                        
  ----------------------------------------------------------------------------

### Approvals {#approvals .Heading-3_Green}

  -------------------------------------------------------------------------------------------------------------------------------------
  Name        Role     Signature      Date           Version   Ticket no. 
  ----------- -------- -------------- -------------- --------- ------------------------------------------------------------------------
  Chris       CIO                     03/10/2025     1.0       [CISP-101711](https://communityfibre.atlassian.net/browse/CISP-101711)
  Williams                                                     

  -------------------------------------------------------------------------------------------------------------------------------------
