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
- Read `14-detection-and-incident-response.md`
- Complete selected activities from `15-course-6-activities-and-practice.md`
- Complete the log-analysis lab in `16-log-analysis-tutorial-data.md`
- Read `17-python-for-security-automation.md`
- Complete selected activities from `18-course-7-python-activities.md`
- Read `09-linux-and-permissions.md`
- Read `10-sql-for-security-analysis.md`
- Practice explaining why evidence handling matters

### Pass 3: Think like an auditor

- Read `04-controls-frameworks-compliance.md`
- Read `06-botium-toys-case-study.md`
- Read `11-assets-risk-and-threat-modeling.md`
- Read `13-course-5-activities-and-portfolio.md`
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
| Day 6 | SIEM, IDS/IPS, EDR, phishing triage, packet analysis, and evidence handling |
| Day 7 | Networking, Linux permissions, SQL basics, log-analysis practice, Course 6 activity practice, Python automation preview, and glossary review |

## Two-week deeper plan plus response day

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
| Day 12 | Log filtering and SQL basics | Use `grep`, `sort`, and `uniq -c` on tutorial logs, then write `SELECT`, `FROM`, `WHERE`, and `ORDER BY` queries |
| Day 13 | SQL joins, assets, and risk | Explain joins, classify assets, and score a risk register |
| Day 14 | Course 5 activities and Botium Toys review | Turn one worksheet into a portfolio artifact and connect findings to business impact |
| Day 15 | Course 6 detection and response | Complete `15-course-6-activities-and-practice.md`: phishing ticket, hash investigation, Wireshark/tcpdump comparison, Suricata review, journal entry, and final report outline |
| Day 16 | Course 7 Python automation | Complete `18-course-7-python-activities.md`: data types, conditionals, loops, functions, regex, file parsing, allow-list update, debugging, and portfolio code notes |

## Course 5 portfolio sprint

Use this sprint after the two-week plan if you want practical work samples.

| Sprint task | Output |
| --- | --- |
| Asset inventory | Build a small table with asset, owner, network access, location, notes, and sensitivity |
| Risk register | Score at least five risks with likelihood, severity, priority, and a recommended response |
| USB scenario | Write contents, attacker mindset, and risk-analysis paragraphs with technical, operational, and managerial controls |
| Data leak worksheet | Map the incident to least privilege, NIST CSF Protect, and NIST SP 800-53 AC-6 |
| Access control worksheet | Use log evidence and directory evidence to identify a stale or overprivileged account |
| PASTA worksheet | Create a DFD, attack tree, threat list, vulnerability list, and control recommendations |

## Course 6 incident-response sprint

Use this sprint when you want hands-on detection and response practice.

For templates, scenarios, and answer keys, use `15-course-6-activities-and-practice.md`.

| Sprint task | Output |
| --- | --- |
| Phishing alert ticket | Write severity, key evidence, escalation decision, and closure or escalation notes |
| Incident handler's journal | Record date, entry number, tools, 5 W's, evidence, questions, and next steps |
| File-hash investigation | Search the hash, record vendor reputation, malware family if known, indicators, and cautions |
| Packet analysis comparison | Explain when to use Wireshark, tcpdump, and TShark |
| PCAP workflow | Identify endpoints, ports, protocols, filters, and suspicious indicators |
| Final report outline | Draft executive summary, timeline, findings, actions taken, recommendations, and lessons learned |

## Log-analysis tutorial sprint

Use this sprint with `16-log-analysis-tutorial-data.md`.

| Sprint task | Output |
| --- | --- |
| Log inventory | List each log file, line count, system, and question it can answer |
| SSH failure review | Count failed passwords, invalid users, repeated source IPs, and nearby successful sessions |
| Web error review | Count `400` and `500` range status codes and group errors by source IP, path, and time |
| Vendor sales review | Count code values while masking full account identifiers |
| Analyst summary | Write scope, evidence, conclusion, and next steps without exposing sensitive raw fields |

## Course 7 Python automation sprint

Use this sprint with `17-python-for-security-automation.md` and `18-course-7-python-activities.md`.

| Sprint task | Output |
| --- | --- |
| Python basics | Explain data types, variables, conditionals, loops, and functions with security examples |
| String/list practice | Normalize usernames, update approved-user lists, and explain indexing/slicing |
| Regex practice | Extract IP addresses or other indicators from log-like text |
| File parsing | Read file text, split it into a list, join it back into text, and explain file modes |
| Allow-list update | Write and explain the full Python algorithm for removing unauthorized IP addresses |
| Debugging practice | Fix syntax, indentation, type, and logic problems |
| Portfolio code note | Present code clearly with scenario, algorithm, output, and sensitive-data masking |

## Interview-ready prompts

- Explain the CIA triad with an example from a real business.
- What is the difference between risk, threat, and vulnerability?
- How is phishing different from social engineering?
- What is the difference between preventive and detective controls?
- What would you do first after receiving a suspicious alert?
- Why is chain of custody important?
- What is the difference between an event, alert, and incident?
- How would you triage a phishing email with a suspicious attachment?
- Why should you search a file hash before opening a suspicious file?
- When would you use Wireshark instead of tcpdump?
- What belongs in an incident handler's journal?
- How would you search logs for repeated failed SSH login attempts?
- Why should account identifiers and session IDs be masked before public sharing?
- How would you automate an allow-list update in Python?
- What is the difference between a parameter and an argument?
- How do `.split()` and `.join()` support file parsing?
- How can regular expressions help security analysts parse log text?
- Why is least privilege important for reducing insider risk?
- How would you identify and fix a stale contractor account?
- How can folder-sharing controls prevent a data leak?
- How do source IP, destination IP, port, and protocol help explain a network alert?
- Why is HTTPS safer than HTTP?
- What is the difference between a firewall, proxy, and VPN?
- How do you read a Linux permission string?
- What is the difference between Linux filtering and SQL filtering?
- How would you prioritize a risk register entry?
- What are the stages of PASTA?
- What evidence belongs in a portfolio-ready worksheet answer?

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
- Tie your recommendation to evidence from the scenario

### If you freeze in a hands-on lab

- Restate the exact question being asked
- Identify the file, directory, table, or column involved
- Run a read-only inspection command first
- Make the smallest needed change
- Verify the result with another command
- Document what changed and why
