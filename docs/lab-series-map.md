# LinuxLabs 15-Lab Series Map

### Purpose

This document defines the canonical LinuxLabs structure.

The series follows the 15 chapters of *Practical Linux System Administration*. Each chapter becomes one lab. The other Linux, operating systems, cloud administration, and system administration books are used to deepen the labs.

### Core Rule

```text
1 chapter = 1 lab
15 chapters = 15 labs
```

### Two-Part Lab Rule

Every chapter lab must have two parts:

```text
Part 1 - New Chapter Content
Part 2 - Cumulative Repetition of All Previous Topics
```

Part 1 uses the current full chapter as the main learning unit.

Part 2 repeats and combines all topics learned in earlier labs.

### Break/Fix Rule

Break/fix is mandatory in every lab.

```text
No break/fix = lab not complete.
```

Every lab must include a controlled failure, evidence-led diagnosis, safe repair, recovery verification, and a prevention note.

Minimum standard:

```text
At least one controlled break/fix scenario per lab.
```

Preferred standard from Lab 05 onward:

```text
One break/fix scenario in Part 1 and one break/fix scenario in Part 2.
```

### Distribution Rule

Every applicable lab must be completed on both:

* a Debian-family system, normally Ubuntu Server LTS
* a RHEL-family system, such as RHEL, Rocky Linux, AlmaLinux, or CentOS Stream

The final lab write-up must include implementation evidence for both families and a comparison of differences.

A lab is incomplete if only one family is attempted, unless the lab explicitly marks the other family out of scope and explains why.

### Reference Roles

| Reference | Role in the lab series |
| --- | --- |
| Practical Linux System Administration | Primary chapter sequence and lab spine; use full chapters |
| The Practice of System and Network Administration | Execution standard: operational discipline, documentation, repeatability, change control, service ownership, incident thinking |
| The Practice of Cloud System Administration | Reliability, automation, scalable operations, cloud-style admin habits |
| The Linux Command Line | Command-line depth, shell fluency, text processing, filesystem navigation; use full relevant chapters |
| Learning Modern Linux | Modern Linux concepts, cloud-native context, observability, containers, modern tooling; use full relevant chapters |
| Modern Operating Systems / Operating System Concepts | Underlying OS theory: processes, memory, filesystems, I/O, concurrency, security; use full relevant chapters |
| AI-assisted operations notes | Prompting, command review, log summarisation, runbook drafting, hypothesis generation, safety checks |

### Lab Map

| Lab | Folder | Practical Linux chapter | Part 1 new content | Part 2 cumulative repetition |
| --- | --- | --- | --- | --- |
| 01 | `01-getting-started-with-linux/` | Getting Started with Linux | Build, access, baseline, inspect, reboot, and document Linux servers on both families | No previous topics; repeat baseline commands until fluent |
| 02 | `02-working-with-permissions-and-privileged-accounts/` | Working with Permissions and Privileged Accounts | Implement least-privilege local access and explain permission decisions on both families | Lab 01 baseline and CLI checks |
| 03 | `03-customizing-the-user-experience/` | Customizing the User Experience | Standardise shell startup, prompts, skeleton files, and login behaviour on both families | Labs 01-02 baseline, CLI, sudo, permissions |
| 04 | `04-managing-users/` | Managing Users | Manage users, groups, expiry, password lifecycle, and service accounts on both families | Labs 01-03 baseline, CLI, sudo, permissions, shell environment |
| 05 | `05-connecting-to-a-network/` | Connecting to a Network | Configure and troubleshoot host networking and SSH exposure on both families | Labs 01-04 baseline, CLI, sudo, permissions, shell environment, users and groups |
| 06 | `06-installing-and-uninstalling-software/` | Installing and Uninstalling Software | Manage software via repositories, packages, dependencies, and source builds on both families | Labs 01-05 plus networking and SSH verification |
| 07 | `07-managing-storage/` | Managing Storage | Add, mount, extend, monitor, and safely decommission storage on both families | Labs 01-06 plus package and network checks |
| 08 | `08-maintaining-system-health/` | Maintaining System Health | Keep systems clean, patched, governed, and periodically reviewed on both families | Labs 01-07 plus storage and package checks |
| 09 | `09-monitoring-your-system/` | Monitoring Your System | Monitor CPU, memory, disk, process, and I/O behaviour with evidence on both families | Labs 01-08 plus maintenance and health checks |
| 10 | `10-scripting-and-automation/` | Scripting and Automation | Create safe scripts and scheduled tasks for repeatable administration on both families | Labs 01-09 plus monitoring and maintenance checks |
| 11 | `11-deploying-samba-for-windows-compatibility/` | Deploying Samba for Windows Compatibility | Build and secure a Samba-backed shared directory service on both families | Labs 01-10 plus Bash automation, storage, users, permissions, networking |
| 12 | `12-troubleshooting-linux/` | Troubleshooting Linux | Diagnose OS, software, firewall, hardware, and log-driven issues on both families | Labs 01-11 plus service, storage, networking, Samba, Bash evidence |
| 13 | `13-securing-your-system/` | Securing Your System | Harden Linux host access, services, accounts, tools, and incident response on both families | Labs 01-12 plus troubleshooting, logs, services, users, permissions, networking |
| 14 | `14-continuing-your-education/` | Continuing Your Education | Convert learning into a sustained professional development system using both families | Labs 01-13 plus knowledge base, scripts, evidence, weak-area review |
| 15 | `15-making-career-moves/` | Making Career Moves | Turn the lab series into portfolio evidence and role-readiness material across both families | Labs 01-14 plus full role-readiness review and portfolio evidence |

### Coverage Rule

By the end of Lab 15, the series must have covered on both Debian-family and RHEL-family systems where applicable:

* Linux installation and first setup
* CLI navigation and shell fluency
* permissions and privilege management
* shell customisation and user environment standards
* user and group lifecycle management
* networking and SSH access
* package management and source builds
* storage, filesystems, swap, and LVM
* housekeeping, patching, quotas, and account retention
* monitoring, performance, capacity, and sysstat-style evidence
* Bash scripting and scheduled automation
* Samba and cross-platform shared storage
* log-driven troubleshooting and break/fix recovery
* Linux security hardening and incident response
* professional learning, certification planning, portfolio evidence, and communication
* responsible AI-assisted operations
* OS theory behind the practical work
* operational standards from system and network administration practice

### Execution Standard

Every lab should be run like operational work, not like a passive tutorial.

Each lab must include:

* a realistic scenario or ticket
* Part 1 new chapter content
* Part 2 cumulative repetition
* mandatory controlled break/fix practice
* baseline state before failure
* symptoms and diagnosis evidence
* repair and recovery evidence
* prevention note
* requirements and constraints
* implementation tasks
* Debian/Ubuntu implementation evidence
* RHEL-family implementation evidence
* RHEL vs Ubuntu comparison
* verification evidence
* post-reboot verification where applicable
* AI-assisted operations notes where relevant
* seven reflection answers
* final documentation uploaded to the correct folder

### Learner Workflow

The learner solves the lab. Documentation is completed after the learner provides evidence and answers the seven reflection questions.
