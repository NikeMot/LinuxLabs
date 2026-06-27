# LinuxLabs 15-Lab Series Map

### Purpose

This document defines the canonical LinuxLabs structure.

The series follows the 15 chapters of *Practical Linux System Administration*. Each chapter becomes one lab. The other Linux, operating systems, cloud administration, and system administration books are used to deepen the labs.

### Core Rule

```text
1 chapter = 1 lab
15 chapters = 15 labs
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
| Practical Linux System Administration | Primary chapter sequence and lab spine |
| The Practice of System and Network Administration | Execution standard: operational discipline, documentation, repeatability, change control, service ownership, incident thinking |
| The Practice of Cloud System Administration | Reliability, automation, scalable operations, cloud-style admin habits |
| The Linux Command Line | Command-line depth, shell fluency, text processing, filesystem navigation |
| Learning Modern Linux | Modern Linux concepts, cloud-native context, observability, containers, modern tooling |
| Modern Operating Systems / Operating System Concepts | Underlying OS theory: processes, memory, filesystems, I/O, concurrency, security |
| AI-assisted operations notes | Prompting, command review, log summarisation, runbook drafting, hypothesis generation, safety checks |

### Lab Map

| Lab | Folder | Practical Linux chapter | Main outcome | Augmentation focus |
| --- | --- | --- | --- | --- |
| 01 | `01-getting-started-with-linux/` | Getting Started with Linux | Build, access, baseline, inspect, reboot, and document Linux servers on both families | CLI fluency, filesystem basics, OS boot concepts, operational baseline standards |
| 02 | `02-working-with-permissions-and-privileged-accounts/` | Working with Permissions and Privileged Accounts | Implement least-privilege local access and explain permission decisions on both families | POSIX permissions, sudo risk, root safety, auditability |
| 03 | `03-customizing-the-user-experience/` | Customizing the User Experience | Standardise shell startup, prompts, skeleton files, and login behaviour on both families | Shell environment, startup files, usability vs standardisation |
| 04 | `04-managing-users/` | Managing Users | Manage users, groups, expiry, password lifecycle, and service accounts on both families | Identity lifecycle, account governance, group-based access |
| 05 | `05-connecting-to-a-network/` | Connecting to a Network | Configure and troubleshoot host networking and SSH exposure on both families | TCP/IP, DNS, routing, network service exposure, secure remote access |
| 06 | `06-installing-and-uninstalling-software/` | Installing and Uninstalling Software | Manage software via repositories, packages, dependencies, and source builds on both families | Package trust, dependency chains, update risk, rollback thinking |
| 07 | `07-managing-storage/` | Managing Storage | Add, mount, extend, monitor, and safely decommission storage on both families | Filesystem theory, block devices, LVM, swap, fstab, data lifecycle |
| 08 | `08-maintaining-system-health/` | Maintaining System Health | Keep systems clean, patched, governed, and periodically reviewed on both families | Housekeeping, quotas, patch processes, account retention, health reporting |
| 09 | `09-monitoring-your-system/` | Monitoring Your System | Monitor CPU, memory, disk, process, and I/O behaviour with evidence on both families | Performance theory, sysstat, bottleneck diagnosis, capacity thinking |
| 10 | `10-scripting-and-automation/` | Scripting and Automation | Create safe scripts and scheduled tasks for repeatable administration on both families | Bash safety, cron, timers, NTP/time drift, automation judgement |
| 11 | `11-deploying-samba-for-windows-compatibility/` | Deploying Samba for Windows Compatibility | Build and secure a Samba-backed shared directory service on both families | Cross-platform access, permissions layering, client compatibility, network storage |
| 12 | `12-troubleshooting-linux/` | Troubleshooting Linux | Diagnose OS, software, firewall, hardware, and log-driven issues on both families | Incident response, hypothesis testing, log reconstruction, break/fix discipline |
| 13 | `13-securing-your-system/` | Securing Your System | Harden Linux host access, services, accounts, tools, and incident response on both families | Attack surface reduction, security controls, policy, breach response, AI safety review |
| 14 | `14-continuing-your-education/` | Continuing Your Education | Convert learning into a sustained professional development system using both families | Certification planning, deliberate practice, documentation quality, knowledge management |
| 15 | `15-making-career-moves/` | Making Career Moves | Turn the lab series into portfolio evidence and role-readiness material across both families | Communication, career positioning, remote work, operational storytelling, CV evidence |

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
* requirements and constraints
* implementation tasks
* Debian/Ubuntu implementation evidence
* RHEL-family implementation evidence
* RHEL vs Ubuntu comparison
* verification evidence
* post-reboot verification where applicable
* break/fix or troubleshooting element where applicable
* AI-assisted operations notes where relevant
* seven reflection answers
* final documentation uploaded to the correct folder

### Learner Workflow

The learner solves the lab. Documentation is completed after the learner provides evidence and answers the seven reflection questions.
