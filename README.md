# Google Cybersecurity Study Guide

This repository reorganizes personal notes from the Google Cybersecurity Certificate on Coursera into a cleaner study guide. It is designed for review, revision, and interview preparation rather than as a raw archive of course text.

## What this repo covers

- Security fundamentals and analyst skills
- Common attack types and how to classify them
- Threat actors and security ethics
- Controls, frameworks, and compliance
- Security analyst tools and response workflows
- Network architecture, protocols, firewalls, proxies, and VPNs
- Detection, incident response, phishing triage, packet analysis, and investigation documentation
- Linux command-line basics and file permissions
- SQL querying for structured security investigations
- Log analysis practice with tutorial web, authentication, and vendor sales logs
- Python automation for security tasks, including functions, regex, file parsing, debugging, and allow-list updates
- Asset inventories, risk registers, and threat modeling
- Course 5 activity practice: home asset inventories, USB risk analysis, data leak worksheets, access control reviews, and PASTA artifacts
- Course 6 activity practice: phishing tickets, incident journals, hash investigation, packet analysis, Suricata review, and final reports
- The Botium Toys audit case study
- A curated glossary and a practical study plan

## How to use it

1. Start with [docs/01-foundations.md](docs/01-foundations.md).
2. Move through the topics in order.
3. Use [docs/12-networking-and-network-security.md](docs/12-networking-and-network-security.md), [docs/09-linux-and-permissions.md](docs/09-linux-and-permissions.md), [docs/10-sql-for-security-analysis.md](docs/10-sql-for-security-analysis.md), [docs/16-log-analysis-tutorial-data.md](docs/16-log-analysis-tutorial-data.md), and [docs/11-assets-risk-and-threat-modeling.md](docs/11-assets-risk-and-threat-modeling.md) for hands-on practice.
4. Use [docs/13-course-5-activities-and-portfolio.md](docs/13-course-5-activities-and-portfolio.md) to turn course worksheets into portfolio-ready analyst notes.
5. Use [docs/14-detection-and-incident-response.md](docs/14-detection-and-incident-response.md) to learn Course 6 alert triage, phishing response, packet analysis, file-hash investigation, and incident reporting.
6. Use [docs/15-course-6-activities-and-practice.md](docs/15-course-6-activities-and-practice.md) to complete Course 6 activities with blank templates, worked answers, and a capstone.
7. Use [docs/17-python-for-security-automation.md](docs/17-python-for-security-automation.md) and [docs/18-course-7-python-activities.md](docs/18-course-7-python-activities.md) to learn and practice Course 7 Python automation.
8. Use [docs/07-glossary.md](docs/07-glossary.md) as a quick lookup reference.
9. Use [docs/08-study-plan.md](docs/08-study-plan.md) for revision and interview prep.
10. Review [docs/06-botium-toys-case-study.md](docs/06-botium-toys-case-study.md) before any governance, risk, or audit assessment.

## Study map

```mermaid
flowchart LR
    A["Foundations"] --> B["Threats and Attacks"]
    B --> C["Threat Actors and Ethics"]
    C --> D["Controls, Frameworks, and Compliance"]
    D --> E["Analyst Toolkit and Response"]
    E --> F["Networking Practice"]
    F --> G["Linux and SQL Practice"]
    G --> H["Log Analysis Tutorial Data"]
    H --> I["Assets, Risk, and Threat Modeling"]
    I --> J["Course 5 Activity Practice"]
    J --> K["Detection and Incident Response"]
    K --> L["Course 6 Activity Practice"]
    L --> M["Python Security Automation"]
    M --> N["Course 7 Python Activities"]
    N --> O["Botium Toys Case Study"]
    O --> P["Glossary and Revision"]
```

## Repository layout

```text
.
|-- README.md
|-- docs/
|   |-- 01-foundations.md
|   |-- 02-threats-and-attacks.md
|   |-- 03-threat-actors-and-ethics.md
|   |-- 04-controls-frameworks-compliance.md
|   |-- 05-analyst-toolkit.md
|   |-- 06-botium-toys-case-study.md
|   |-- 07-glossary.md
|   |-- 08-study-plan.md
|   |-- 09-linux-and-permissions.md
|   |-- 10-sql-for-security-analysis.md
|   |-- 11-assets-risk-and-threat-modeling.md
|   |-- 12-networking-and-network-security.md
|   |-- 13-course-5-activities-and-portfolio.md
|   |-- 14-detection-and-incident-response.md
|   |-- 15-course-6-activities-and-practice.md
|   |-- 16-log-analysis-tutorial-data.md
|   |-- 17-python-for-security-automation.md
|   |-- 18-course-7-python-activities.md
|   |-- images/
|   `-- references.md
`-- sources/
    `-- source-index.md
```

## Scope note

These notes are paraphrased and reorganized from personal course materials. They are intended as a personal learning aid and reference set, not as an official course replacement.

## Recommended review flow

- Learn the vocabulary in context, not as isolated definitions.
- Tie every concept back to a control, risk, or response action.
- Practice classifying incidents by attack type, control type, and business impact.
- Practice reading network alerts by source, destination, port, protocol, and direction.
- Practice Linux permission interpretation and SQL filters with the worked examples.
- Practice Linux log filtering with the tutorial web, secure, and vendor sales logs.
- Treat every asset, vulnerability, and control as part of a risk story.
- Turn each Course 5 worksheet into a short artifact: scenario, evidence, issue, recommendation, and justification.
- Turn each Course 6 activity into a short artifact: alert, evidence, decision, escalation, journal entry, and final recommendation.
- Turn each Course 7 Python activity into a small automation artifact: scenario, input, algorithm, code, output, debugging notes, and safe portfolio explanation.
- Revisit the Botium Toys case study after each theory section.

## Beginner shortcut

If you are new to cybersecurity, use this simple order:

1. Learn the core language in foundations, threats, and controls.
2. Practice analyst tools with networking, Linux, and SQL.
3. Practice log analysis with the tutorial data chapter.
4. Practice risk thinking with asset inventories and risk registers.
5. Use the Course 5 activity chapter to write portfolio-style answers.
6. Learn Course 6 incident-response concepts.
7. Complete the Course 6 activity workbook.
8. Learn Course 7 Python automation concepts.
9. Complete the Course 7 Python activity workbook.
10. Review the glossary whenever a term slows you down.

## Fast checkpoints

- Can you explain the CIA triad without reading?
- Can you distinguish phishing, malware, and social engineering?
- Can you map a control to administrative, technical, or physical categories?
- Can you explain when a security analyst should defend, escalate, document, and preserve evidence?
- Can you explain what TCP/IP layer a protocol belongs to?
- Can you identify common ports like DNS 53, SSH 22, HTTPS 443, and DHCP 67/68?
- Can you triage a phishing alert by checking sender, recipient, attachment, links, hash, and user action?
- Can you explain when Wireshark, tcpdump, TShark, SIEM, IDS/IPS, EDR, and SOAR are useful?
- Can you complete an incident handler's journal and a final report outline from a scenario?
- Can you read a Linux permission string like `-rw-rw-r--`?
- Can you write a basic SQL query with `SELECT`, `FROM`, `WHERE`, and `ORDER BY`?
- Can you use `grep`, `sort`, and `uniq -c` to find repeated log patterns?
- Can you explain why raw logs should be sanitized before public sharing?
- Can you write a simple Python function, loop, conditional, regex search, and file-update algorithm?
- Can you build a simple risk register using likelihood and severity?
- Can you explain why a former contractor account with admin access is a security issue?
- Can you map a data leak recommendation to least privilege and NIST CSF Protect?

## Official references

See [docs/references.md](docs/references.md) for primary links such as the NIST glossary, NIST frameworks, and CompTIA Security+.
