# 04 Controls, Frameworks, and Compliance

## Big picture

Controls, frameworks, and compliance are related but not interchangeable.

- Controls are the safeguards.
- Frameworks organize how security is managed.
- Compliance is the requirement to meet rules and standards.

## Control categories

| Category | Purpose | Examples |
| --- | --- | --- |
| Administrative or managerial | Govern people, policy, and process | Password policies, separation of duties, training |
| Technical | Enforce security through technology | Firewalls, IDS, antivirus, encryption |
| Physical or operational | Restrict physical access and environmental exposure | Locks, CCTV, badge readers |

## Control types

| Type | Purpose |
| --- | --- |
| Preventive | Stop an incident before it happens |
| Detective | Identify that an incident has happened or is happening |
| Corrective | Restore or recover after an incident |
| Deterrent | Discourage bad behavior or attacks |

## NIST framing

### NIST CSF

The notes emphasize the CSF as a risk-management structure. NIST CSF 2.0 organizes the core around six functions:

- Govern
- Identify
- Protect
- Detect
- Respond
- Recover

Govern was added in CSF 2.0 to make leadership, policy, oversight, and risk strategy explicit. In beginner terms: governance decides what security must accomplish, and the other functions help carry it out.

### NIST RMF

The glossary notes reference these RMF stages:

- Prepare
- Categorize
- Select
- Implement
- Assess
- Authorize
- Monitor

## Compliance and standards to know

| Standard or regulation | Main use |
| --- | --- |
| GDPR | Protects EU personal data and breach transparency |
| PCI DSS | Protects payment card processing environments |
| HIPAA | Protects health information in the US |
| FedRAMP | Standardizes US federal cloud assessment and authorization |
| FERC-NERC | Power grid and critical infrastructure obligations |
| CIS Controls | Action-oriented defensive controls |
| ISO | International standards across management and technology |
| SOC 1 and SOC 2 | Audit reporting on controls and trust areas |

## Additional frameworks to recognize

| Framework | Plain meaning | How an analyst might use it |
| --- | --- | --- |
| Cyber Threat Framework (CTF) | A common language for describing cyber threat activity | Helps teams describe tactics, techniques, and threat activity consistently |
| ISO/IEC 27001 | International standard for an information security management system | Helps organizations manage security risks through policies, controls, and continual improvement |

CTF is useful when communicating what a threat actor is doing. ISO/IEC 27001 is useful when discussing whether an organization has a structured security management program.

## Security principles that guide control design

Security principles help analysts judge whether a control is sensible, not just whether a tool exists.

| Principle | Beginner meaning | Example |
| --- | --- | --- |
| Minimize attack surface | Reduce the number of places an attacker can target | Disable unused services and close unused ports |
| Least privilege | Give only the access needed | Remove group read access from a restricted file |
| Defense in depth | Use layers of controls | MFA plus firewall plus monitoring plus backups |
| Separation of duties | Split critical tasks between people or roles | One person requests a payment and another approves it |
| Keep security simple | Avoid needless complexity | Use clear firewall rules that can be reviewed |
| Fix security issues correctly | Address root cause, not only symptoms | Patch vulnerable code and test the fix |
| Secure defaults | Make the default state safe | New accounts start with minimal access |
| Fail securely | If a control fails, it should fail into a safer state | A firewall blocks traffic if its rule engine fails |
| Do not trust services blindly | Verify third-party and internal service data | Validate vendor data before using it in customer-facing systems |
| Avoid security by obscurity | Do not rely on secrecy as the main protection | Protect an app with authentication, authorization, logging, and testing, not hidden URLs alone |

These principles are practical during reviews. If a design is hard to explain, grants broad access by default, or depends on nobody discovering a weakness, it probably needs stronger control design.

## Security audits and assessments

Audits and assessments both review security, but they answer different questions.

| Activity | Main question | Common timing |
| --- | --- | --- |
| Security audit | Are controls, policies, and procedures meeting a required standard? | Often annual or tied to compliance |
| Security assessment | How resilient are current systems against threats? | Often more frequent, such as every three to six months |

Example: A regulation might require MFA for administrator accounts. An audit checks whether MFA is enabled. An assessment might also test whether weak passwords, privilege creep, or misconfigured alerts still create risk.

## Least privilege as a control

The principle of least privilege gives users and services only the access required to complete a task. It supports confidentiality by limiting who can view data, integrity by reducing unauthorized changes, and availability by lowering the chance of accidental damage.

Least privilege is maintained through:

- Baseline access by role
- Privileged account restrictions
- Usage audits
- Privilege audits
- Account change audits
- Timely removal of access that is no longer needed

## How to think about the relationship

```mermaid
flowchart LR
    A["Business asset"] --> B["Risk assessment"]
    B --> C["Framework selection"]
    C --> D["Control design"]
    D --> E["Compliance alignment"]
    E --> F["Monitoring and review"]
```

## Botium Toys control lens

The assignment materials point to a common audit pattern:

- Identify assets first
- Compare current controls to expected controls
- Record gaps
- Map gaps to risk and business continuity impact
- Recommend prioritized remediation

## What to memorize

- Control category versus control type
- NIST CSF versus NIST RMF
- When to mention GDPR, HIPAA, and PCI DSS
- Why compliance is not the same as full security

## Quick self-test

1. Is encryption a control category or a technical control?
2. What is the difference between a preventive control and a detective control?
3. Why can an organization be compliant but still insecure?
