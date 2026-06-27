# LinuxLabs

### Overview

The LinuxLabs repository contains my hands-on Linux system administration labs aimed at developing practical Linux, infrastructure, SRE operations, and AI-assisted operations skills.

The canonical LinuxLabs programme is a **15-lab chapter-led series** based on *Practical Linux System Administration* by Kenneth Hess. Each lab maps to one full chapter of that book and expands it with material from the other Linux and operating systems books in my Drive.

Every chapter lab has two parts:

1. **Part 1 — New Chapter Content**
2. **Part 2 — Cumulative Repetition of All Previous Topics**

After the 15 chapter-led labs, LinuxLabs continues with an **8-lab drill series**. The drill series is designed to force recall, integration, troubleshooting, and production-style execution across everything learned in the first 15 labs.

The final drill is an **SRE-style Linux operations capstone**. It must test service ownership, SLIs, SLOs, monitoring, alerting, incident response, postmortem writing, runbook quality, toil reduction, Bash automation, and recovery on both Debian-family and RHEL-family systems.

Controlled break/fix practice is the most important practical mechanism in LinuxLabs. Every lab and drill should include a controlled failure, evidence-led diagnosis, safe repair, verification, and prevention note.

Bash and shell skill are taught throughout the whole programme. Bash is the primary shell. POSIX shell and KornShell awareness are included where relevant for enterprise UNIX/Linux environments.

Every applicable lab must be completed on both a Debian-family system, normally Ubuntu Server LTS, and a RHEL-family system. Differences between the two must be documented as part of the final lab evidence.

The goal is not just to learn commands, but to build production-style operational judgement: build, verify, troubleshoot, document, recover, compare distributions, script safely, use AI responsibly, and explain decisions.

### Core Rule

Main series:

```text
15 chapters = 15 labs
```

Every chapter lab:

```text
Part 1 = new full-chapter content
Part 2 = cumulative repetition of all previous topics
Controlled break/fix = mandatory
```

Drill series:

```text
8 integration drills
```

Total programme:

```text
23 labs total
```

By the end of Lab 15, the LinuxLabs series should have covered the practical administration content from *Practical Linux System Administration* and the relevant supporting concepts from the other Linux, operating systems, cloud administration, and system administration books.

By the end of Drill 08, the learner should be able to combine those skills under realistic SRE-style operational pressure on both Debian-family and RHEL-family systems.

### Full-Chapter Reference Rule

When a lab references a book chapter, the whole chapter should be used as the reference unit.

Do not build labs from isolated fragments. Use the full chapter to understand the topic, context, warnings, commands, and operational implications. Final lab write-ups must remain original and must not copy book material.

### Cumulative Repetition Rule

Part 1 of each chapter lab introduces the current chapter's new content.

Part 2 of each chapter lab repeats and combines all topics learned in previous labs.

The later the lab, the heavier Part 2 becomes.

Example:

```text
Lab 05 Part 1 = networking
Lab 05 Part 2 = baseline, CLI, sudo, permissions, shell environment, users and groups
```

### Break/Fix Rule

Every lab and drill must include controlled break/fix practice.

The required pattern is:

```text
baseline -> break -> observe -> diagnose -> fix -> verify -> reboot test where relevant -> document -> improve
```

Break/fix work must be performed only on disposable lab systems, with snapshots or checkpoints where appropriate.

### Distribution Standard

The default target systems are:

| Family | Default lab target | Purpose |
| --- | --- | --- |
| Debian-family | Ubuntu Server LTS | Debian/Ubuntu administration, `apt`, Netplan, AppArmor, Debian-style paths and logs |
| RHEL-family | RHEL, Rocky Linux, AlmaLinux, or CentOS Stream | Red Hat-style administration, `dnf`, firewalld, SELinux, XFS/LVM conventions, RHCSA-style skills |

A lab is not complete until the relevant work has been attempted, verified, and documented on both families, unless the lab explicitly states that one family is out of scope and explains why.

### Primary Reference

| Role | Reference |
| --- | --- |
| Main lab sequence | Practical Linux System Administration |
| Execution standard | The Practice of System and Network Administration |
| Cloud operations mindset | The Practice of Cloud System Administration |
| Command-line depth | The Linux Command Line |
| Modern Linux depth | Learning Modern Linux |
| Operating system theory | Modern Operating Systems / Operating System Concepts |
| Bash and shell progression | Bash, POSIX shell, and KornShell awareness |
| Role-readiness target | DXC Linux System Administrator readiness map |
| SRE capstone target | SRE capstone standard |
| AI support | Responsible AI-assisted operations notes and verified system evidence |

### Lab Series

| Lab | Folder | Practical Linux chapter | Status |
| --- | --- | --- | --- |
| 01 | `01-getting-started-with-linux/` | Getting Started with Linux | Not started |
| 02 | `02-working-with-permissions-and-privileged-accounts/` | Working with Permissions and Privileged Accounts | Not started |
| 03 | `03-customizing-the-user-experience/` | Customizing the User Experience | Not started |
| 04 | `04-managing-users/` | Managing Users | Not started |
| 05 | `05-connecting-to-a-network/` | Connecting to a Network | Not started |
| 06 | `06-installing-and-uninstalling-software/` | Installing and Uninstalling Software | Not started |
| 07 | `07-managing-storage/` | Managing Storage | Not started |
| 08 | `08-maintaining-system-health/` | Maintaining System Health | Not started |
| 09 | `09-monitoring-your-system/` | Monitoring Your System | Not started |
| 10 | `10-scripting-and-automation/` | Scripting and Automation | Not started |
| 11 | `11-deploying-samba-for-windows-compatibility/` | Deploying Samba for Windows Compatibility | Not started |
| 12 | `12-troubleshooting-linux/` | Troubleshooting Linux | Not started |
| 13 | `13-securing-your-system/` | Securing Your System | Not started |
| 14 | `14-continuing-your-education/` | Continuing Your Education | Not started |
| 15 | `15-making-career-moves/` | Making Career Moves | Not started |

### Drill Series

| Drill | Folder | Purpose | Status |
| --- | --- | --- | --- |
| 01 | `drills/01-baseline-and-access-rebuild/` | Rebuild baseline access, shell, users, sudo, SSH, and documentation from memory | Not started |
| 02 | `drills/02-network-and-service-recovery/` | Recover a broken networked service using DNS, routing, firewall, service, and log evidence | Not started |
| 03 | `drills/03-storage-pressure-and-restore/` | Diagnose storage pressure, repair mounts, extend capacity, and prove restore readiness | Not started |
| 04 | `drills/04-permissions-identity-and-samba/` | Repair user, group, permission, and Samba access issues across Linux and client workflows | Not started |
| 05 | `drills/05-patching-software-and-rollback/` | Handle package changes, update risk, broken dependencies, and rollback decisions | Not started |
| 06 | `drills/06-monitoring-performance-and-capacity/` | Investigate CPU, memory, disk, process, and I/O pressure with monitoring evidence | Not started |
| 07 | `drills/07-security-hardening-and-incident-response/` | Harden a host, investigate suspicious activity, and document response actions | Not started |
| 08 | `drills/08-full-linux-operations-capstone/` | SRE-style Linux operations capstone: service ownership, SLIs/SLOs, monitoring, alerting, incident response, postmortem, runbook, toil reduction, and dual-distro recovery | Not started |

### Supporting Standards

| Document | Purpose |
| --- | --- |
| `docs/lab-series-map.md` | Maps the 15 chapter-led labs |
| `docs/drill-series-map.md` | Maps the 8 integration drills |
| `docs/cumulative-repetition-standard.md` | Defines the two-part lab structure and cumulative review rule |
| `docs/break-fix-standard.md` | Defines mandatory controlled failure, diagnosis, repair, verification, and prevention practice |
| `docs/environment-standard.md` | Defines hosts, snapshots, baseline packages, and evidence rules |
| `docs/debian-rhel-comparison-matrix.md` | Tracks recurring Debian/Ubuntu vs RHEL-family differences |
| `docs/bash-and-shell-progression.md` | Defines how Bash and shell skills progress across all labs |
| `docs/dxc-linux-admin-readiness-map.md` | Maps LinuxLabs to the DXC Linux System Administrator role |
| `docs/sre-capstone-standard.md` | Defines the SRE-style final capstone requirements |
| `docs/itil-operations-templates.md` | Provides incident, problem, change, rollback, RCA, and restoration templates |
| `docs/assessment-gates.md` | Defines pass/fail readiness gates |
| `docs/network-filesharing-protocols.md` | Makes NFS, SSH/SFTP, FTP awareness, and Samba coverage explicit |
| `docs/ansible-mini-layer.md` | Adds a lightweight Ansible layer after Bash foundations |
| `docs/learner-workflow.md` | Defines the solve-first, document-after workflow |
| `docs/lab-output-template.md` | Defines the final lab documentation format |
| `scripts/README.md` | Defines the Bash script portfolio structure |

### Naming Convention

Chapter folders use this format:

```text
01-topic-name-written-lowercase
```

Drill folders use this format:

```text
drills/01-drill-name-written-lowercase
```

Lab files inside folders use this format:

```text
lab-01-short-lab-title.md
```

Example:

```text
01-getting-started-with-linux/lab-01-bootstrap-and-baseline-linux-server.md
```

Drill example:

```text
drills/01-baseline-and-access-rebuild/lab-drill-01-baseline-and-access-rebuild.md
```

### How to Use This Repository

Each chapter lab should include:

* Part 1 — New Chapter Content
* Part 2 — Cumulative Repetition of All Previous Topics
* Controlled break/fix scenario
* Scenario
* Reference material using full chapters where books are used
* Requirements
* Constraints
* Assumptions
* Implementation tasks
* Key commands used
* Files created or changed
* Verification evidence
* Bash or shell usage notes
* Debian/Ubuntu implementation evidence
* RHEL-family implementation evidence
* RHEL vs Ubuntu comparison
* Break/fix scenario
* Post-reboot verification
* AI-assisted operations notes, where relevant
* ITIL-style artefact where relevant
* Issues encountered
* Decisions made
* Security and production considerations
* Final outcome
* What I learned
* What I would improve in production
* References used
* Completion checklist
* Seven reflection questions

### Learner Workflow

The learner solves the lab. Documentation, formatting, evidence organisation, and GitHub upload are handled after the lab is solved.

The learner provides command output, observations, issues, final verification evidence, and answers to seven reflection questions.

### Security and Privacy Notes

The repository must not contain:

* Passwords
* API keys
* SSH private keys
* `.env` files
* Cloud credentials
* Company data
* Screenshots containing private tenant, account, or user information
* Book PDFs or EPUBs
* Copyrighted training material
* Sensitive logs
* Private IP addressing or hostnames from a real employer environment

### AI Usage Rule

AI may be used as a learning and operations assistant, but it must not replace verification.

Use AI for explanation, planning, command review, log summaries, runbook drafts, comparison notes, and checklists. Always validate AI suggestions with real command output, logs, documentation, and post-reboot testing.

### Lab Upload Rule

Every new Linux lab must be committed to the correct numbered chapter folder or drill folder. Labs should not be placed at the repository root.
