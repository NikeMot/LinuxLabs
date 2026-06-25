# LinuxLabs

### Overview

The LinuxLabs repository contains my hands-on Linux system administration labs aimed at developing practical Linux, infrastructure, and SRE operations skills.

The lab series focuses on administering both **RHEL** and **Ubuntu** systems. The goal is not just to learn commands, but to build production-style operational judgement: build, verify, troubleshoot, document, recover, compare distributions, and explain decisions.

The major skills covered in this repository are:

* Linux foundations
* Users, groups, sudo, and permissions
* Software and repository management
* systemd, boot, and service management
* Storage, filesystems, swap, and LVM
* Linux networking and name resolution
* Security hardening, firewalls, SELinux, and AppArmor
* Logging, troubleshooting, and incident reconstruction
* Backup, restore, and recovery testing
* Performance and capacity investigation
* Bash automation, Ansible, and configuration management
* Linux estate operations and capstone scenarios

Each lab should be documented with requirements, constraints, implementation notes, commands used, verification evidence, issues encountered, decisions made, production considerations, and reflection questions.

### Goals

The goals of this repository are:

* Build repeatable Linux administration skills through hands-on labs
* Practise RHEL and Ubuntu administration side by side
* Develop production-grade troubleshooting habits
* Document technical decisions clearly
* Create evidence of operational thinking, verification, and recovery
* Prepare for Linux system administrator, infrastructure engineer, SRE, and platform engineering roles

### Skills Covered

| Area | Status | Topics |
| --- | --- | --- |
| Linux foundations | Not started | shell, filesystem, documentation, baseline inventory |
| Users, groups, and permissions | Not started | local users, sudo, groups, ACLs, umask |
| Software management | Not started | apt, dnf, repositories, package ownership, updates |
| systemd and services | Not started | units, targets, timers, journald, service recovery |
| Storage and filesystems | Not started | partitions, filesystems, fstab, swap, LVM |
| Networking | Not started | IP, routes, DNS, Netplan, NetworkManager, troubleshooting |
| Security and hardening | Not started | firewalls, SSH hardening, SELinux, AppArmor, audit checks |
| Logging and troubleshooting | Not started | journalctl, logs, incident timelines, break/fix evidence |
| Backup and recovery | Not started | tar, rsync, restore testing, permissions, recovery runbooks |
| Performance and capacity | Not started | CPU, memory, disk, processes, limits, bottlenecks |
| Automation and configuration management | Not started | Bash health checks, Ansible, idempotency, drift control |
| Linux estate operations | Not started | multi-server operations, capstone incidents, runbooks |

### Repository Structure

| Path | Purpose |
| --- | --- |
| `docs/` | General documentation, standards, templates, and repository decisions |
| `01-linux-foundations/` | Shell, filesystem, baseline build, documentation, and investigation labs |
| `02-users-groups-and-permissions/` | Local identity, sudo, permissions, ACLs, and shared directory labs |
| `03-software-management/` | Package management, repositories, updates, and rollback labs |
| `04-systemd-and-services/` | systemd units, boot targets, timers, journald, and service recovery labs |
| `05-storage-and-filesystems/` | Partitions, filesystems, mounts, swap, LVM, and storage failure labs |
| `06-networking/` | IP configuration, routing, DNS, firewalls, and network troubleshooting labs |
| `07-security-and-hardening/` | SSH hardening, firewalls, SELinux, AppArmor, and baseline audit labs |
| `08-logging-and-troubleshooting/` | Log investigation, incident reconstruction, and break/fix evidence labs |
| `09-backup-and-recovery/` | Backup design, restore testing, and recovery runbook labs |
| `10-performance-and-capacity/` | CPU, memory, disk, process, and service capacity investigation labs |
| `11-automation-and-configuration-management/` | Bash automation, Ansible, cloud-init, and drift management labs |
| `12-linux-estate-operations/` | Multi-server production simulation and capstone operational labs |

### Naming Convention

Topic folders use this format:

```text
01-topic-name-written-lowercase
```

Lab files inside topic folders should use this format:

```text
lab-01-short-lab-title.md
```

Example:

```text
01-linux-foundations/lab-01-build-and-baseline-linux-servers.md
```

### How to Use This Repository

Each lab folder or lab file should include:

* Scenario
* Reference material
* Requirements
* Constraints
* Assumptions
* Implementation tasks
* Key commands used
* Files created or changed
* Verification evidence
* RHEL vs Ubuntu comparison
* Break/fix scenario
* Post-reboot verification
* Issues encountered
* Decisions made
* Security and production considerations
* Final outcome
* What I learned
* What I would improve in production
* References used
* Completion checklist
* Reflection questions

Start with `01-linux-foundations` and progress numerically.

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

### Lab Upload Rule

Every new Linux lab should be committed to the correct numbered topic folder. Labs should not be placed at the repository root.
