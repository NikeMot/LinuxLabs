# Network File Sharing and Transfer Protocol Coverage

### Purpose

This document makes NFS, SSH/SFTP, FTP awareness, and Samba coverage explicit in LinuxLabs.

These topics support Linux administrator readiness for environments that include mixed Linux, UNIX, and Windows-compatible services.

### Protocol Coverage

| Protocol/service | Required depth | Labs/drills |
| --- | --- | --- |
| SSH | Hands-on | Lab 05, Lab 13, Drill 01, Drill 02, Drill 07 |
| SFTP | Hands-on through OpenSSH | Lab 05, Lab 13, Drill 02 |
| FTP | Awareness plus optional hardened `vsftpd` exercise | Lab 05, Drill 02 |
| NFS | Hands-on where environment allows | Lab 07, Lab 11, Drill 03, Drill 04 |
| Samba/SMB | Hands-on | Lab 11, Drill 04 |

### SSH and SFTP

The learner should be able to:

* explain the difference between SSH shell access and SFTP file transfer
* verify the SSH service name on both Ubuntu and RHEL-family systems
* inspect `sshd_config`
* test local and remote access
* review logs for failed and successful login attempts
* understand firewall impact on SSH/SFTP
* avoid weakening SSH for convenience

### FTP Awareness

Classic FTP should be treated as a legacy and risk-sensitive protocol.

The learner should understand:

* FTP sends data differently from SSH-based SFTP
* plain FTP can expose credentials if not protected
* FTP may require additional firewall considerations
* anonymous FTP is risky if misconfigured
* SFTP is generally preferred for secure file transfer in Linux administration

Optional exercise:

* install and configure `vsftpd` on disposable lab systems
* restrict access
* verify firewall rules
* document why SFTP is usually preferred

### NFS

The learner should be able to:

* install NFS server and client packages
* export a directory
* mount an NFS share from another Linux host
* configure persistent mounts
* verify UID/GID and permissions behaviour
* test firewall requirements
* compare NFS behaviour on Ubuntu and RHEL-family systems
* document production risks such as over-broad exports

### Samba

The learner should be able to:

* install Samba
* configure a shared directory
* map Linux users/groups to Samba access
* verify access from Linux and, where possible, Windows/macOS clients
* troubleshoot permission layering
* document firewall and service requirements

### Security Requirements

For every protocol exercise, document:

* listening ports
* firewall exposure
* authentication method
* filesystem permissions
* service status
* logs checked
* post-reboot persistence
* risks and safer alternatives

### Placement Rule

NFS, SFTP, FTP awareness, and Samba should be included inside existing labs and drills rather than becoming separate primary labs.

This keeps the canonical structure at 15 chapter-led labs plus 8 integration drills.
