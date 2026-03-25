# 02 Threats and Attacks

## High-level view

Attack classification matters because different attacks require different detection methods, controls, and escalation paths.

## Common attack families

### Phishing

Phishing uses digital communication to trick someone into revealing data or performing unsafe actions.

| Type | Description |
| --- | --- |
| BEC | Impersonates a trusted sender for financial gain |
| Spear phishing | Targets a specific person or team |
| Whaling | Targets executives or senior staff |
| Vishing | Uses phone or voice channels |
| Smishing | Uses text messages |

### Malware

Malware is software built to damage systems, steal data, or create unauthorized access.

| Type | Description |
| --- | --- |
| Virus | Needs user action to execute and spread |
| Worm | Self-replicates across systems without user action |
| Ransomware | Encrypts data and demands payment |
| Spyware | Secretly collects information |

### Social engineering

Social engineering exploits human trust and decision-making rather than technical weaknesses alone.

| Type | Description |
| --- | --- |
| Social media phishing | Builds a target profile from public data |
| Watering hole | Compromises a site the target group often visits |
| USB baiting | Tricks a user into plugging in a malicious device |
| Physical social engineering | Uses impersonation to gain physical access |

## Why social engineering works

- Authority
- Intimidation
- Social proof
- Scarcity
- Familiarity
- Trust
- Urgency

## Additional attack types from the notes

| Attack type | Example | Useful classification |
| --- | --- | --- |
| Password attack | Brute force, rainbow table | Communication and network security |
| Physical attack | Malicious USB cable, card skimming | Asset security |
| Adversarial AI | Manipulating AI or ML systems | Network plus identity concerns |
| Supply-chain attack | Compromised vendor software or hardware | Cross-domain risk |
| Cryptographic attack | Birthday, collision, downgrade | Communication and network security |

## Practical analyst cues

### Signs of phishing

- Unusual sender or tone
- Urgent requests for action
- Link mismatch
- Unexpected attachments
- Requests for credentials, money, or access

### Signs of malware impact

- Sudden encryption or file lockout
- Unexpected outbound traffic
- Slower systems
- New processes or services
- Unauthorized changes to files

## Attack triage shortcut

```mermaid
flowchart TD
    A["Suspicious event"] --> B{"Human trickery involved?"}
    B -->|Yes| C["Check phishing or social engineering"]
    B -->|No| D{"Malicious code or unauthorized execution?"}
    D -->|Yes| E["Check malware or exploit path"]
    D -->|No| F{"Physical device or access involved?"}
    F -->|Yes| G["Check physical attack path"]
    F -->|No| H["Check password, cryptographic, or supply-chain angle"]
```

## What to memorize

- The difference between phishing, malware, and social engineering
- The major phishing subtypes
- The reasons social engineering succeeds
- The analyst value of attack classification

## Quick self-test

1. How is a worm different from a virus?
2. Why is USB baiting a social engineering attack?
3. What makes BEC different from general phishing?
