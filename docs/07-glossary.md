# 07 Glossary

This glossary is a curated quick-reference built from the supplied course notes and glossary document. Definitions are intentionally short and study-focused.

## Governance, risk, and security basics

| Term | Definition |
| --- | --- |
| Asset | Anything the organization values and must protect |
| Availability | Authorized users can access systems and data when needed |
| Compliance | Following internal standards and external requirements |
| Confidentiality | Only authorized access is allowed |
| Integrity | Data remains accurate, authentic, and reliable |
| Risk | Potential harm when a threat can exploit a weakness |
| Security control | A safeguard used to reduce risk |
| Security framework | A structured model for managing security work |
| Security posture | The organization’s ability to defend, detect, and respond |
| Threat | Any event or condition that could cause harm |
| Threat actor | A person or group that creates security risk |
| Vulnerability | A weakness that can be exploited |

## Identity and access

| Term | Definition |
| --- | --- |
| Authentication | Verifying who someone is |
| Authorization | Granting approved access to resources |
| Biometrics | Physical traits used to help verify identity |
| Deprovisioning | Removing or disabling access when a user, contractor, or service no longer needs it |
| Least privilege | Giving only the access needed to do the job |
| Password attack | An attempt to gain access through password compromise |
| RBAC | Role-based access control, where permissions are assigned through roles instead of one user at a time |

## Attacks and adversaries

| Term | Definition |
| --- | --- |
| Adversarial AI | Using or manipulating AI and ML for attack advantage |
| BEC | A phishing attack impersonating a trusted source for financial gain |
| Hacktivist | A threat actor motivated by political or social goals |
| Malware | Software designed to harm, spy on, or extort |
| Phishing | Digital deception used to steal data or trigger unsafe action |
| Physical attack | An attack that affects physical as well as digital environments |
| Removable media | Portable storage such as USB drives or external hard drives |
| Session hijacking | Taking over or misusing a valid user session |
| Social engineering | Exploiting human trust or behavior to gain access |
| Spear phishing | Highly targeted phishing against a person or group |
| Supply-chain attack | Compromising a vendor, dependency, or delivery path |
| USB baiting | Leaving a malicious USB device for someone to use |
| Vishing | Voice-based phishing |
| Watering hole attack | Compromising a site often used by the target group |
| Worm | Self-spreading malware |

## Tools and operations

| Term | Definition |
| --- | --- |
| Chronicle | A cloud-native platform for retaining and searching security data |
| IDS | A system that detects suspicious or unauthorized activity |
| Incident response | The organized process for handling security incidents |
| Log | A recorded event from a system or device |
| Packet sniffer | A tool that captures and analyzes network traffic |
| Playbook | A documented procedure for repeatable security tasks |
| SIEM | A platform that collects and analyzes security event and log data |

## Networking and protocols

| Term | Definition |
| --- | --- |
| Application layer | TCP/IP layer where user-facing network services operate |
| ARP | Protocol that maps IP addresses to MAC addresses on a local network |
| Client | Device or application that requests a service |
| Cloud-based firewall | Firewall service hosted or delivered through a cloud provider |
| Controlled zone | Filtered network segment between untrusted and internal resources |
| DHCP | Protocol that automatically assigns IP configuration to devices |
| DNS | Protocol that translates domain names into IP addresses |
| Encapsulation | Wrapping traffic inside another packet, often for tunneling |
| Firewall | Network security control that monitors and filters traffic |
| Forward proxy | Proxy that handles internal client requests to external resources |
| Hub | Network device that repeats traffic to all connected ports |
| HTTPS | Secure web protocol that uses TLS encryption |
| ICMP | Protocol used for network error reporting and connectivity checks |
| IMAP | Protocol used to read and synchronize email from a server |
| Internet layer | TCP/IP layer that routes traffic between networks using IP addresses |
| IP address | Network address used to route traffic to a host or network |
| IPSec | VPN protocol suite used to authenticate and encrypt packets |
| MAC address | Hardware address used for local network delivery |
| NAT | Process that maps private internal IP addresses to a public IP address |
| Network access layer | TCP/IP layer for local delivery through hardware, MAC addresses, Wi-Fi, Ethernet, and ARP |
| Network protocol | Rule set that defines how network devices communicate |
| Network segmentation | Dividing a network into smaller controlled parts |
| OSI model | Seven-layer conceptual model for discussing network communication |
| Port filtering | Allowing or blocking traffic based on port number |
| POP3 | Protocol used to retrieve email from a server |
| Proxy server | Server that forwards requests between clients and other services |
| Reverse proxy | Proxy that handles external requests to internal services |
| Router | Network device that forwards packets between networks using IP addresses |
| SDN | Software-defined networking, where network behavior is controlled through software |
| Security zone | Network segment with defined trust and control boundaries |
| Server | System that provides services or information to clients |
| SFTP | Secure file transfer protocol that commonly uses SSH |
| SMTP | Protocol used to send and route email |
| SNMP | Protocol used to monitor and manage network devices |
| Stateful firewall | Firewall that tracks connection state |
| Stateless firewall | Firewall that checks packets against rules without remembering connection state |
| Subnet | Logical subdivision of an IP network |
| Switch | Network device that forwards local traffic using MAC addresses |
| TCP | Connection-oriented transport protocol |
| TCP/IP model | Four-layer model for organizing network communication |
| Telnet | Insecure remote shell protocol that sends data in clear text |
| TLS | Encryption protocol used to protect data in transit |
| Transport layer | TCP/IP layer where TCP, UDP, and ports organize host-to-host delivery |
| UDP | Connectionless transport protocol |
| Uncontrolled zone | Network area outside organizational control, such as the public internet |
| VPN | Encrypted tunnel over an untrusted network |
| WAF | Web application firewall that filters web application traffic |
| Wi-Fi | Wireless networking based on IEEE 802.11 standards |
| WireGuard | Modern VPN protocol designed for simpler setup and strong performance |
| WPA | Wi-Fi security protocol family |

## Frameworks and standards

| Term | Definition |
| --- | --- |
| CIS Controls | A practical set of defensive security controls |
| CTF | Cyber Threat Framework; common language for describing cyber threat activity |
| GDPR | EU data protection regulation |
| HIPAA | US law protecting health information |
| ISO/IEC 27001 | International standard for an information security management system |
| NIST CSF | A risk-management framework built around core security functions |
| NIST RMF | A lifecycle framework for selecting and managing controls |
| PCI DSS | Standard for protecting payment card data |
| SOC 1 and SOC 2 | Audit reports focused on controls and trust areas |

## Evidence and handling

| Term | Definition |
| --- | --- |
| Chain of custody | Documented record of evidence possession and control |
| Evidence preservation | Protecting evidence from change or loss during investigation |
| Order of volatility | The priority order for capturing volatile data before it disappears |

## Linux and permissions

| Term | Definition |
| --- | --- |
| Absolute file path | Full path starting from the root directory |
| Argument | Information supplied to a command |
| Bash | Common Linux shell used to run commands |
| chmod | Linux command used to change permissions |
| Command-line interface | Text-based interface for interacting with a computer |
| Execute permission | Permission to run a file or enter/search a directory |
| Filesystem Hierarchy Standard | Linux directory organization beginning at `/` |
| Group | Owner category used to grant permissions to multiple users |
| Hidden file | File whose name begins with a period |
| Kernel | Core of the operating system that manages resources |
| Linux | Open-source operating system widely used in security work |
| Package manager | Tool used to install, manage, and remove software packages |
| Read permission | Permission to view file contents or list directory contents |
| Relative file path | Path interpreted from the current directory |
| Shell | Command interpreter between user and operating system |
| Write permission | Permission to change a file or create/delete entries in a directory |

## SQL and application security

| Term | Definition |
| --- | --- |
| Aggregate function | SQL function such as `COUNT`, `AVG`, or `SUM` that summarizes values |
| Database | Organized collection of information |
| Foreign key | Column that connects one table to another |
| Full outer join | Join that returns records from both tables, matched or unmatched |
| Inner join | Join that returns matching records from both tables |
| Input validation | Checking that user input meets expected rules |
| Left join | Join that returns all records from the first table and matching records from the second |
| Prepared statement | Coding technique that separates SQL code from user-provided data |
| Primary key | Column that uniquely identifies a record |
| Query | Request for data from a database |
| Right join | Join that returns all records from the second table and matching records from the first |
| Row or record | One entry in a database table |
| SQL | Query language used to interact with databases |
| SQL injection | Attack that executes unexpected database queries |
| Table | Database structure made of rows and columns |

## Assets, data, and vulnerability management

| Term | Definition |
| --- | --- |
| Asset classification | Labeling assets based on sensitivity and importance |
| Asset inventory | Catalog of assets that need to be protected |
| Asset management | Tracking assets and risks that affect them |
| Attack surface | All potential places where an attacker could try to exploit a system |
| Attack tree | Diagram that maps possible attack paths to an asset |
| Attack vector | Path or method used by an attacker |
| Data breach | Confirmed unauthorized access, disclosure, or compromise of information |
| Data leak | Unintended exposure of information to someone who should not have access |
| Data loss prevention | Tools or processes that detect, block, or alert on sensitive data leaving approved locations |
| CISA KEV catalog | Known Exploited Vulnerabilities catalog maintained by CISA |
| CVE | Public identifier for a known vulnerability |
| CVSS | System for scoring vulnerability severity |
| Data at rest | Data that is stored and not actively moving |
| Data custodian | Person or system responsible for safe handling, storage, and transport of data |
| Data in transit | Data moving between systems or locations |
| Data in use | Data currently being accessed or processed |
| Data owner | Person who decides who can access, use, edit, or destroy data |
| Defense in depth | Layered security approach that reduces risk |
| Encryption | Converting readable data into encoded data |
| Exploit | Method of taking advantage of a vulnerability |
| Exposure | Mistake or condition that can be exploited by a threat |
| Information privacy | Protecting people from unauthorized access or distribution of their data |
| Information security | Keeping data in all states away from unauthorized users |
| MFA | Authentication that requires at least two forms of verification |
| PASTA | Risk-centric threat modeling framework |
| Privilege creep | Access accumulation beyond what a user currently needs |
| Access review | Periodic check that user permissions still match job duties and business need |
| Account change audit | Review of account creations, permission changes, disabling, and deletion |
| Security assessment | Review of current resilience against threats |
| Security audit | Review of controls, policies, and procedures against expectations |
| Security hardening | Strengthening a system to reduce vulnerability and attack surface |
| Service account | Account used by an application or automated process |
| STRIDE | Threat modeling framework covering spoofing, tampering, repudiation, information disclosure, denial of service, and elevation of privilege |
| Threat modeling | Identifying assets, vulnerabilities, and exposure to threats |
| Vulnerability management | Finding, prioritizing, fixing, and monitoring vulnerabilities |
| Vulnerability scanner | Tool that compares systems against known weaknesses |
| Zero-day | Exploit or vulnerability known before a fix is available |

## Study advice

- Learn these terms with an example.
- Link each term to an analyst action.
- Revisit the glossary after each topic section instead of memorizing it all at once.
