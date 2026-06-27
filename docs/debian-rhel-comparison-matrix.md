# Debian/Ubuntu vs RHEL-Family Comparison Matrix

### Purpose

This document captures recurring differences between Debian-family and RHEL-family Linux systems.

It should be used when writing lab evidence, troubleshooting notes, and RHEL vs Ubuntu comparison sections.

### Core Comparison

| Area | Debian/Ubuntu | RHEL-family | Lab relevance |
| --- | --- | --- | --- |
| Package manager | `apt`, `apt-get`, `dpkg` | `dnf`, `rpm` | Software installation, updates, package ownership |
| Repository config | `/etc/apt/sources.list`, `/etc/apt/sources.list.d/` | `/etc/yum.repos.d/` | Repository trust and troubleshooting |
| Package query | `dpkg -l`, `dpkg -S`, `apt-cache`, `apt show` | `rpm -qa`, `rpm -qf`, `dnf info` | Package verification and dependency checks |
| Service manager | systemd | systemd | Mostly common, but unit names and defaults may differ |
| Firewall | often `ufw` or raw nftables/iptables | commonly `firewalld` | Network exposure and service access |
| Mandatory access control | AppArmor | SELinux | Security troubleshooting and hardening |
| Network config | Netplan, NetworkManager, systemd-networkd depending on version | NetworkManager, `nmcli` | Static IP, DNS, routes, interface management |
| Admin group | `sudo` | `wheel` | Privileged account setup |
| Web user | `www-data` often used | `apache` often used | Web service permissions |
| Log files | `/var/log/syslog`, journald, service logs | `/var/log/messages`, journald, service logs | Incident reconstruction |
| SSH service | `ssh` | `sshd` | Service status checks and hardening |
| Apache package | `apache2` | `httpd` | Web service deployment and troubleshooting |
| Apache config | `/etc/apache2/` | `/etc/httpd/` | Config path comparison |
| NGINX config | `/etc/nginx/` | `/etc/nginx/` | Mostly similar, package defaults may differ |
| Default filesystem | often ext4 | often XFS | Storage labs and recovery planning |
| LVM tooling | LVM tools available when installed | LVM commonly used | Storage management |
| Cron paths | `/etc/cron.*`, user crontabs | `/etc/cron.*`, user crontabs | Scheduled jobs |
| Time sync | `systemd-timesyncd` or chrony | chrony commonly used | Time drift and scheduling |
| Security updates | `unattended-upgrades` | `dnf-automatic` | Patch automation awareness |
| Kernel package naming | Debian/Ubuntu naming | RHEL-style kernel RPMs | Boot and update troubleshooting |

### Command Comparison Cheatsheet

| Task | Debian/Ubuntu | RHEL-family |
| --- | --- | --- |
| Update package metadata | `sudo apt update` | `sudo dnf check-update` |
| Upgrade packages | `sudo apt upgrade` | `sudo dnf upgrade` |
| Install package | `sudo apt install <package>` | `sudo dnf install <package>` |
| Remove package | `sudo apt remove <package>` | `sudo dnf remove <package>` |
| Find package owning file | `dpkg -S <path>` | `rpm -qf <path>` |
| List installed packages | `dpkg -l` | `rpm -qa` |
| Enable service | `sudo systemctl enable --now <service>` | `sudo systemctl enable --now <service>` |
| Check logs | `journalctl`, `/var/log/syslog` | `journalctl`, `/var/log/messages` |
| Add admin user to admin group | `sudo usermod -aG sudo <user>` | `sudo usermod -aG wheel <user>` |
| Check firewall | `sudo ufw status` or `sudo nft list ruleset` | `sudo firewall-cmd --list-all` |
| Open firewall port | `sudo ufw allow <port>` | `sudo firewall-cmd --add-port=<port>/tcp --permanent && sudo firewall-cmd --reload` |
| Check MAC status | `aa-status` | `getenforce`, `sestatus` |
| Configure network | Netplan YAML or NetworkManager | `nmcli`, NetworkManager profiles |

### Documentation Rule

Every lab comparison should answer:

1. What command or path differed?
2. Why did it differ?
3. Did the outcome differ or only the implementation?
4. What would an engineer need to remember in production?
5. What evidence proves both implementations worked?

### Safety Rule

Never assume the RHEL-family command is the same as the Ubuntu command.

Always verify package names, service names, firewall behaviour, security controls, logs, and config paths on the actual system.
