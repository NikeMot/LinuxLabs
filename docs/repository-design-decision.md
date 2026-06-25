# Repository Design Decision

### Purpose

This document explains why LinuxLabs is organised by Linux system administration topic rather than by tool name alone.

The repository is intended to show progression from basic Linux administration into production operations, troubleshooting, automation, and estate management.

### Decision

LinuxLabs will use numbered topic folders at the repository root.

Folder names use this format:

```text
01-topic-name-written-lowercase
```

Lab files inside each topic folder use this format:

```text
lab-01-short-lab-title.md
```

Example:

```text
01-linux-foundations/lab-01-build-and-baseline-linux-servers.md
```

### Reason

A Linux administrator does not work by tool category alone. They work across operational domains such as identity, permissions, storage, networking, security, services, logs, backups, patching, automation, and incident recovery.

The topic-based folder structure makes the repository easier to navigate and easier to review as a portfolio.

### Topic Folder Structure

| Folder | Purpose |
| --- | --- |
| `01-linux-foundations/` | Shell, filesystem, baseline build, documentation, and investigation labs |
| `02-users-groups-and-permissions/` | Local identity, sudo, groups, ACLs, and shared directory labs |
| `03-software-management/` | Package management, repositories, updates, and rollback labs |
| `04-systemd-and-services/` | systemd units, boot targets, timers, journald, and service recovery labs |
| `05-storage-and-filesystems/` | Partitions, filesystems, mounts, swap, LVM, and storage failure labs |
| `06-networking/` | IP configuration, routing, DNS, Netplan, NetworkManager, and troubleshooting labs |
| `07-security-and-hardening/` | SSH hardening, firewalls, SELinux, AppArmor, and baseline audit labs |
| `08-logging-and-troubleshooting/` | Log investigation, incident reconstruction, and break/fix evidence labs |
| `09-backup-and-recovery/` | Backup design, restore testing, and recovery runbook labs |
| `10-performance-and-capacity/` | CPU, memory, disk, process, and service capacity investigation labs |
| `11-automation-and-configuration-management/` | Bash automation, Ansible, cloud-init, and drift management labs |
| `12-linux-estate-operations/` | Multi-server production simulation and capstone operational labs |

### Documentation Folder

The `docs/` folder stores repository-wide standards and supporting material.

Examples:

* commit strategy
* lab output template
* repository design decision
* lab placement standard
* RHEL vs Ubuntu comparison notes
* reference map

### Lab Placement Rule

Every lab must be uploaded to the correct numbered topic folder.

Examples:

| Lab Type | Correct Folder |
| --- | --- |
| Shell, filesystem, baseline build | `01-linux-foundations/` |
| Users, groups, sudo, ACLs | `02-users-groups-and-permissions/` |
| apt, dnf, repositories, updates | `03-software-management/` |
| systemd, boot, timers, services | `04-systemd-and-services/` |
| LVM, fstab, swap, filesystem recovery | `05-storage-and-filesystems/` |
| IP, DNS, routes, Netplan, NetworkManager | `06-networking/` |
| SSH hardening, firewalling, SELinux, AppArmor | `07-security-and-hardening/` |
| journald, logs, incident reconstruction | `08-logging-and-troubleshooting/` |
| backup, restore, disaster recovery | `09-backup-and-recovery/` |
| performance, capacity, bottlenecks | `10-performance-and-capacity/` |
| Bash, Ansible, cloud-init, drift | `11-automation-and-configuration-management/` |
| capstone, multi-server estate operations | `12-linux-estate-operations/` |

### Production Relevance

This structure mirrors how operational work is divided in real infrastructure teams. A hiring manager or senior engineer should be able to review the repository and quickly understand which Linux administration areas have been practised, documented, and verified.
