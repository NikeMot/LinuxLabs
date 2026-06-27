# Bash Script Portfolio

### Purpose

This folder will hold reusable Bash scripts created during LinuxLabs.

The scripts should demonstrate practical Linux administration skill.

### Rule

Scripts should be added as they are created during labs and drills.

Do not add large script collections before they are needed.

### Planned Script Types

| Script | Purpose |
| --- | --- |
| `health-check.sh` | Summarise uptime, CPU, memory, disk, and important services |
| `user-audit.sh` | Report users, groups, shells, and admin group membership |
| `disk-report.sh` | Report disks, mounts, filesystem usage, and LVM status |
| `service-check.sh` | Check status, enablement, logs, and listening ports for a service |
| `network-check.sh` | Check IP address, routes, DNS, ports, and connectivity |
| `package-audit.sh` | Report installed packages, updates, package owners, and repo status |
| `log-summary.sh` | Extract useful log windows for incidents |
| `baseline-check.sh` | Check common baseline settings and produce evidence |
| `backup-check.sh` | Verify backup files, timestamps, permissions, and restore readiness |
| `samba-check.sh` | Check Samba service, share config, permissions, and access assumptions |
| `nfs-check.sh` | Check NFS exports, mounts, firewall exposure, and permissions |

### Script Quality Standard

Every script should:

* have a clear purpose
* be readable
* include comments where useful
* avoid destructive defaults
* use safe quoting
* handle missing commands or files where practical
* return meaningful exit codes where practical
* print useful evidence
* work on both Ubuntu and RHEL-family systems where practical
* explain any distribution-specific logic

### Header Standard

Use this header pattern:

```bash
#!/usr/bin/env bash
# Script: script-name.sh
# Purpose: Describe what this script checks or changes.
# Supported: Ubuntu/Debian-family and RHEL-family where practical.
# Safety: Describe whether the script is read-only or changes system state.
```

### AI Review Rule

AI may review scripts for readability, safety, portability, and missed edge cases.

AI-generated scripts must be reviewed, tested on disposable systems, and verified with command output before being treated as working evidence.
