# LinuxLabs 8-Lab Drill Series Map

### Purpose

This document defines the 8-lab drill series that follows the 15 chapter-led LinuxLabs programme.

The chapter-led series teaches and practises the material. The drill series tests whether the learner can combine the material under realistic operational pressure.

### Core Rule

```text
15 chapter-led labs first
8 integration drills after
23 labs total
```

### Drill Philosophy

The drills should not feel like tutorials.

Each drill should feel like operational work:

* a ticket or incident arrives
* the system is partially broken or incomplete
* the learner must investigate
* the learner must make safe changes
* the learner must prove the final state
* the learner must answer seven reflection questions
* the final documentation is produced and uploaded after completion

### Drill Series

| Drill | Folder | Main theme | Skills combined |
| --- | --- | --- | --- |
| 01 | `drills/01-baseline-and-access-rebuild/` | Baseline and access rebuild | install validation, CLI, users, sudo, SSH, shell customisation, documentation |
| 02 | `drills/02-network-and-service-recovery/` | Network and service recovery | IP, DNS, routing, firewall, SSH, systemd, logs, service verification |
| 03 | `drills/03-storage-pressure-and-restore/` | Storage pressure and restore | disks, filesystems, fstab, LVM, swap, cleanup, backup and restore evidence |
| 04 | `drills/04-permissions-identity-and-samba/` | Permissions, identity, and Samba | users, groups, ACLs, umask, Samba, shared directories, cross-platform access |
| 05 | `drills/05-patching-software-and-rollback/` | Patching, software, and rollback | apt, dnf, dependencies, source installs, update risk, package verification |
| 06 | `drills/06-monitoring-performance-and-capacity/` | Monitoring, performance, and capacity | sysstat, CPU, memory, disk, I/O, process investigation, capacity notes |
| 07 | `drills/07-security-hardening-and-incident-response/` | Security hardening and incident response | root protection, SSH hardening, firewalling, account review, logs, suspicious activity response |
| 08 | `drills/08-full-linux-operations-capstone/` | Full Linux operations SRE capstone | service ownership, SLIs, SLOs, monitoring, alerting, incident response, postmortem, runbook, toil reduction, Bash automation, dual-distro recovery |

### Drill 08 SRE Standard

Drill 08 must be SRE-relevant.

It should simulate operating a small Linux-backed service and proving reliability through:

* service overview
* SLI definitions
* SLO target
* monitoring checks
* alert candidates
* incident timeline
* root cause analysis
* recovery evidence
* post-reboot verification
* blameless postmortem
* runbook
* toil-reduction note
* Bash automation evidence
* Debian/Ubuntu evidence
* RHEL-family evidence
* RHEL vs Ubuntu comparison

### Expected Difficulty

The drills should be harder than the chapter labs.

They should require recall across chapters rather than giving a direct sequence of commands.

Drill 08 should require SRE-style thinking, not only Linux command execution.

### Documentation Rule

The learner solves the drill first. Documentation is produced after evidence and reflection answers are provided.

### Seven Reflection Questions

Ask exactly seven questions at the end of each drill:

1. What problem did this drill simulate?
2. What commands, files, or services mattered most in solving it?
3. What evidence proves your solution worked?
4. What broke, confused you, or required troubleshooting?
5. What would be risky about doing this in production?
6. Where did AI help, if at all, and what did you verify yourself?
7. What would you improve, automate, or monitor next time?

### Upload Rule

Final drill write-ups must be uploaded under the matching `drills/NN-drill-name/` folder.
