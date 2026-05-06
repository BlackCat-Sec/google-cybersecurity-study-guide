# 08 Study Plan

## Four-pass revision strategy

### Pass 1: Build the mental model

- Read `01-foundations.md`
- Read `02-threats-and-attacks.md`
- Create your own one-line definitions for CIA, risk, threat, and control

### Pass 2: Think like an analyst

- Read `03-threat-actors-and-ethics.md`
- Read `05-analyst-toolkit.md`
- Read `12-networking-and-network-security.md`
- Read `09-linux-and-permissions.md`
- Read `10-sql-for-security-analysis.md`
- Practice explaining why evidence handling matters

### Pass 3: Think like an auditor

- Read `04-controls-frameworks-compliance.md`
- Read `06-botium-toys-case-study.md`
- Read `11-assets-risk-and-threat-modeling.md`
- Practice mapping controls to business risk

### Pass 4: Memorize what matters

- Use `07-glossary.md`
- Review `docs/references.md`
- Write short answers to the self-test questions in each document

## One-week focused plan

| Day | Focus |
| --- | --- |
| Day 1 | Foundations and CIA triad |
| Day 2 | Phishing, malware, and social engineering |
| Day 3 | Threat actors, ethics, and legal boundaries |
| Day 4 | Controls, categories, and NIST frameworks |
| Day 5 | Compliance regulations and use cases |
| Day 6 | SIEM, IDS, playbooks, and evidence handling |
| Day 7 | Networking, Linux permissions, SQL basics, and glossary review |

## Two-week deeper plan

| Day | Focus | Practice |
| --- | --- | --- |
| Day 1 | Foundations | Explain CIA, risk, threat, and vulnerability in your own words |
| Day 2 | Analyst skills | Map a SIEM alert to evidence, escalation, and documentation |
| Day 3 | Threats | Classify phishing, malware, physical, and supply-chain scenarios |
| Day 4 | Threat actors and ethics | Write a short ethical response to a suspected attacker |
| Day 5 | Controls | Sort controls by administrative, technical, physical, preventive, detective, and corrective |
| Day 6 | Frameworks | Explain CSF Govern, Identify, Protect, Detect, Respond, and Recover |
| Day 7 | Compliance | Compare GDPR, HIPAA, PCI DSS, and SOC 2 use cases |
| Day 8 | Network architecture | Explain clients, servers, switches, routers, firewalls, and access points |
| Day 9 | Protocols and ports | Memorize TCP/IP layers and common ports |
| Day 10 | Linux navigation | Practice `pwd`, `ls -la`, `cd`, `cat`, `head`, `tail`, and `less` |
| Day 11 | Linux permissions | Decode `-rw-rw-r--` and write `chmod` changes for least privilege |
| Day 12 | SQL basics | Write `SELECT`, `FROM`, `WHERE`, and `ORDER BY` queries |
| Day 13 | SQL joins, assets, and risk | Explain joins, classify assets, and score a risk register |
| Day 14 | Botium Toys review | Connect findings to business impact and remediation order |

## Interview-ready prompts

- Explain the CIA triad with an example from a real business.
- What is the difference between risk, threat, and vulnerability?
- How is phishing different from social engineering?
- What is the difference between preventive and detective controls?
- What would you do first after receiving a suspicious alert?
- Why is chain of custody important?
- Why is least privilege important for reducing insider risk?
- How do source IP, destination IP, port, and protocol help explain a network alert?
- Why is HTTPS safer than HTTP?
- What is the difference between a firewall, proxy, and VPN?
- How do you read a Linux permission string?
- What is the difference between Linux filtering and SQL filtering?
- How would you prioritize a risk register entry?
- What are the stages of PASTA?

## Fast recall sheet

### If you forget the order of thinking

1. What asset is at risk?
2. What threat or actor is involved?
3. What weakness is being used?
4. What control should reduce the risk?
5. What should be documented or escalated?

### If you forget a framework concept

- CSF is a high-level operating model.
- RMF is a lifecycle for selecting, assessing, authorizing, and monitoring controls.

### If you freeze in an assessment

- Identify the asset
- Identify the missing control
- Explain the business impact
- Recommend the next control or process improvement

### If you freeze in a hands-on lab

- Restate the exact question being asked
- Identify the file, directory, table, or column involved
- Run a read-only inspection command first
- Make the smallest needed change
- Verify the result with another command
- Document what changed and why
