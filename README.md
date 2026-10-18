# Cybersecurity Portfolio

![Status](https://img.shields.io/badge/status-active-brightgreen)
![Security+](https://img.shields.io/badge/CompTIA%20Security%2B-in%20progress-orange)
![Focus](https://img.shields.io/badge/focus-blue%20team%20%7C%20cloud%20security-blue)

Hands-on labs, investigations and write-ups from my path into cybersecurity and cloud security. Everything here is built and tested in my own lab, and documented as I learn, including what went wrong.

## About me
I'm a second-year university student working toward a career in cybersecurity and cloud security. I'm studying for **CompTIA Security+** (exam planned before the end of December 2026) and building practical projects alongside it, so I can show my skills and not only list them.

## Why this repo exists
Certifications show I can pass an exam. Projects show I can do the work. This repo is where I:
- build real skills by doing, not just reading
- practise writing clearly about technical work, which is a core part of security jobs
- keep an honest record of my progress, mistakes included

## What's inside
Work is grouped by domain, so the repo can grow for years without turning into a mess.

| Folder | Focus | Status |
|---|---|---|
| `00-labs` | Lab environment: virtualization, baseline VMs, snapshots | In progress |
| `01-foundations` | Linux, networking, scripting | In progress |
| `02-blue-team` | Detection, incident investigations, vulnerability management, hardening | Planned |
| `03-offensive` | Web app security, Active Directory, pentest reports, CTF write-ups | Planned |
| `04-cloud-security` | AWS security baseline, posture management, automated response | In progress |
| `05-devsecops` | Secrets hygiene, secure pipelines | Planned |
| `06-grc` | Risk assessments, policies, threat models | Planned |
| `07-tools` | Small security tools and scripts | Planned |

Folders appear here as I complete the work in them.

## Progress

**Done**
- [x] GitHub repo, SSH authentication and git workflow
- [x] VirtualBox lab with an Ubuntu Server VM and snapshots → [`00-labs/hypervisor-setup`](00-labs/hypervisor-setup/)
- [x] Break-and-restore practice (deleted SSH config, filled the disk) → [`snapshot-practice.md`](00-labs/hypervisor-setup/snapshot-practice.md)
- [x] AWS account setup: billing alerts and budget, root user MFA, non-root admin user → [`04-cloud-security/01-aws/01-account-setup`](04-cloud-security/01-aws/01-account-setup/)

**In progress**
- [ ] CompTIA Security+ (exam planned December 2026)
- [ ] OverTheWire Bandit, levels 0 to 20 (currently on level 4) → [`01-foundations/01-linux/01-bandit`](01-foundations/01-linux/01-bandit/)

**Next**
- [ ] Harden the Ubuntu VM (SSH keys, firewall, fail2ban, auditd) with before and after Lynis scores
- [ ] Network traffic analysis and malware pcap investigations
- [ ] Home SOC and detection lab (SIEM, ATT&CK-mapped detections)

## How I document projects
Every project follows the same layout, so it's easy to skim:

```
project-name/
├── README.md     problem, setup, results, what broke, next steps
├── docs/         design notes, runbooks, reports
├── src/          scripts, configs, rules
└── assets/       screenshots and diagrams
```

I include the **problems I hit and how I fixed them**, because debugging is most of the job.

## Lab safety and ethics
- All scanning, attacks and testing happen on systems I own, inside an isolated lab.
- Malware samples are only handled in isolated VMs without network access.
- No passwords, keys, tokens or real personal data are ever committed here.
- Techniques are documented for learning and defence.

## Tools and technologies
Linux (Ubuntu), VirtualBox, Git and GitHub, SSH, Bash. More will be added here as I use them (Wazuh/Elastic, Wireshark, Suricata, AWS, Python).

Feedback is welcome, especially if you spot a mistake or a better approach.