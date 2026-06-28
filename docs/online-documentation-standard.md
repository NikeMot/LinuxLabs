# Online Documentation Standard

### Purpose

LinuxLabs uses books for structured learning, but online documentation is required so lab decisions stay current.

Books provide depth and sequence. Official online documentation provides current implementation detail, package behaviour, version differences, security guidance, and vendor-specific commands.

### Core Rule

```text
Every lab must check current online documentation where implementation details could change.
```

Use online documentation for:

* package names
* service names
* configuration paths
* firewall commands
* security controls
* release-specific behaviour
* deprecations
* storage and networking syntax
* Ansible module behaviour
* known limitations
* break/fix verification

### Source Priority

Use sources in this order:

1. Official vendor or project documentation.
2. Distribution documentation for the exact OS family.
3. Local man pages and package-provided documentation on the lab system.
4. Trusted community documentation only when official documentation is incomplete.
5. Blogs and forum posts only as hints, never as final authority.

### Required Official Sources

| Area | Preferred online source | URL |
| --- | --- | --- |
| RHEL administration | Red Hat Enterprise Linux documentation | `https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/` |
| Ubuntu Server | Ubuntu Server documentation | `https://ubuntu.com/server/docs/` |
| Debian administration | Debian Administrator's Handbook | `https://www.debian.org/doc/manuals/debian-handbook/` |
| systemd | systemd project documentation and manual pages | `https://systemd.io/` |
| Linux kernel | Linux kernel documentation | `https://docs.kernel.org/` |
| Ansible | Ansible community documentation | `https://docs.ansible.com/ansible/latest/` |
| Samba | Samba documentation | `https://www.samba.org/samba/docs/` |
| OpenSSH | OpenSSH manual pages | `https://www.openssh.com/manual.html` |
| Ubuntu security | Ubuntu security documentation | `https://documentation.ubuntu.com/security/` |
| Red Hat security | RHEL security documentation | `https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/` |

### Local Documentation Requirement

Online documentation must be combined with local system documentation.

Use local commands such as:

```bash
man systemctl
man sshd_config
man fstab
man sudoers
systemctl --help
apt show <package>
dnf info <package>
rpm -qf <path>
dpkg -S <path>
```

### Lab Documentation Requirement

Every final lab write-up should include an online documentation check.

Record:

| Field | Meaning |
| --- | --- |
| Source used | Official source or local documentation used |
| Topic checked | What was verified |
| Date checked | Date the documentation was checked |
| Version or distribution | OS or tool version the documentation applies to |
| Lab decision affected | What command, path, package, or approach was confirmed |

### Currentness Rule

If a command, package name, service name, firewall method, or security control differs between sources, prefer the documentation that matches the actual lab system version.

Examples:

* use RHEL documentation for RHEL-family behaviour
* use Ubuntu Server documentation for Ubuntu behaviour
* use Ansible documentation matching the Ansible version installed
* use local man pages when they reflect the installed package version

### Break/Fix Rule

For break/fix work, online documentation should help confirm:

* expected working state
* correct configuration path
* correct service name
* correct log source
* supported recovery method
* safe rollback approach

Documentation does not replace evidence. The fix still must be proven with command output, logs, service status, connectivity checks, or post-reboot verification.

### AI Usage Rule

AI may suggest documentation to check, but AI output is not documentation.

When AI suggests a command or diagnosis, verify it against:

* official online documentation
* local man pages
* local command output
* logs
* post-reboot testing

### Repository Rule

Do not copy large sections of online documentation into the repository.

Use links, short notes, original summaries, and lab-specific evidence.

### Completion Standard

A lab is complete only when:

* relevant online documentation has been checked
* local system evidence has been captured
* differences between Debian/Ubuntu and RHEL-family documentation are noted where relevant
* final commands and configuration are verified on the actual lab systems
