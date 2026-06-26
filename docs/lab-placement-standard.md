# Lab Placement Standard

### Purpose

Every LinuxLabs lab must be placed in the correct numbered topic folder.

### Topic Folder Naming

Use this format:

```text
01-topic-name-written-lowercase
```

Rules:

* use two-digit numbering
* use lowercase words
* separate words with hyphens
* keep folders topic-based
* do not place labs at the repository root

### Lab File Naming

Use this format:

```text
lab-01-short-lab-title.md
```

Example:

```text
01-linux-foundations/lab-01-build-and-baseline-linux-servers.md
```

### Placement Rules

| Lab focus | Folder |
| --- | --- |
| Linux basics, shell, filesystem, baseline build | `01-linux-foundations/` |
| Users, groups, sudo, permissions, ACLs | `02-users-groups-and-permissions/` |
| apt, dnf, repositories, updates | `03-software-management/` |
| systemd, boot, timers, services | `04-systemd-and-services/` |
| disks, filesystems, mounts, swap, LVM | `05-storage-and-filesystems/` |
| IP, routes, DNS, Netplan, NetworkManager | `06-networking/` |
| SSH hardening, firewalls, SELinux, AppArmor | `07-security-and-hardening/` |
| journald, logs, incident reconstruction | `08-logging-and-troubleshooting/` |
| backup, restore, recovery testing | `09-backup-and-recovery/` |
| CPU, memory, disk, process pressure | `10-performance-and-capacity/` |
| Bash, Ansible, cloud-init, drift | `11-automation-and-configuration-management/` |
| capstone and multi-server operations | `12-linux-estate-operations/` |
| AI-assisted Linux operations | `13-ai-assisted-linux-operations/` |

If a lab covers several areas, place it in the folder for the primary skill being tested and mention the supporting skills inside the lab.

AI may also appear as a supporting section inside another topic lab when it helps with explanation, review, documentation, or troubleshooting.
