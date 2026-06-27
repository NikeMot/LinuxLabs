# LinuxLabs Environment Standard

### Purpose

This document defines the standard lab environment for LinuxLabs.

The goal is to make every lab repeatable, comparable, and evidence-based across both Debian-family and RHEL-family systems.

### Required Distribution Families

Every applicable lab must be completed on both families:

| Family | Default target | Notes |
| --- | --- | --- |
| Debian-family | Ubuntu Server LTS | Used for Debian/Ubuntu administration, `apt`, Netplan, AppArmor, Debian-style paths, and Ubuntu service behaviour |
| RHEL-family | RHEL, Rocky Linux, AlmaLinux, or CentOS Stream | Used for Red Hat-style administration, `dnf`, firewalld, SELinux, XFS/LVM conventions, and RHCSA-style skills |

### Minimum Lab Hosts

Use at least two Linux VMs:

| Hostname | Family | Purpose |
| --- | --- | --- |
| `ubuntu-admin01` | Debian-family | Primary Ubuntu administration host |
| `rhel-admin01` | RHEL-family | Primary RHEL-family administration host |

Recommended later expansion:

| Hostname | Family | Purpose |
| --- | --- | --- |
| `ubuntu-web01` | Debian-family | Web/service testing host |
| `rhel-web01` | RHEL-family | Web/service testing host |
| `ubuntu-storage01` | Debian-family | Storage, Samba, NFS, and backup testing |
| `rhel-storage01` | RHEL-family | Storage, Samba, NFS, and backup testing |

### VM Sizing

Minimum for most labs:

| Resource | Minimum |
| --- | --- |
| CPU | 2 vCPU |
| Memory | 2 GB RAM |
| Disk | 25 GB |
| Network | NAT or bridged network with internet access |

Storage labs may require one or more extra virtual disks.

### Naming Standard

Use this pattern:

```text
<family>-<role><number>
```

Examples:

```text
ubuntu-admin01
rhel-admin01
ubuntu-web01
rhel-web01
```

### User Standard

Use a named non-root administrative account for labs.

Do not work directly as root unless the lab explicitly requires root-shell behaviour.

Recommended account pattern:

```text
labadmin
```

### SSH Standard

Default rule:

* use SSH key-based login where possible
* avoid password-based SSH where possible
* do not commit private keys
* verify SSH access after changes
* record SSH configuration differences between Debian/Ubuntu and RHEL-family systems

### Snapshot Standard

Before each lab:

1. Confirm the current VM state.
2. Take a snapshot or checkpoint.
3. Record the snapshot name in the lab evidence.

Recommended naming:

```text
pre-lab-01-baseline
pre-lab-02-permissions
```

After a successful lab:

1. Perform post-reboot verification.
2. Take a known-good snapshot if useful.
3. Record what changed.

### Baseline Package Standard

Install only basic administrative tools at the beginning.

Examples:

| Tool | Purpose |
| --- | --- |
| `curl` | HTTP testing and downloads |
| `wget` | downloads |
| `vim` or `nano` | text editing |
| `tree` | filesystem inspection |
| `man-db` / man pages | local documentation |
| `bash-completion` | shell usability |
| `rsync` | file copy and backup tasks |
| `unzip` | archive extraction |
| `git` | documentation and version control workflow |

Do not install large stacks before they are needed.

### Evidence Storage Standard

For every lab, capture evidence in the final write-up rather than committing raw sensitive logs.

Evidence should include:

* command used
* relevant output
* hostname
* distribution family
* date or session context
* pass/fail result

Redact secrets, private IPs if required, tokens, keys, account names from real employers, and any sensitive data.

### Reset Standard

If a lab becomes too broken to recover:

1. Record the failure.
2. Explain what went wrong.
3. Revert to the pre-lab snapshot.
4. Repeat the lab.
5. Document the recovery decision.

Failure is useful if it is recorded and understood.

### Completion Standard

A lab is complete only when:

* Debian/Ubuntu work is verified or explicitly out of scope
* RHEL-family work is verified or explicitly out of scope
* differences are documented
* post-reboot checks are complete where applicable
* final evidence is captured
* seven reflection questions are answered
