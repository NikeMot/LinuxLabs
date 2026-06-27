# DXC Linux System Administrator Readiness Map

### Purpose

This document maps LinuxLabs to the Linux System Administrator role described for DXC Technology in Manchester.

The goal is to make the 15 chapter-led labs and 8 drill labs produce evidence for first and second level support, incident handling, monitoring, documentation, compliance, process improvement, shell scripting, networking, storage, automation, and production operations.

### Role Themes

| Job requirement | LinuxLabs coverage |
| --- | --- |
| First and second level technical support | Labs 01-13, especially troubleshooting and drills |
| Incidents and problems | Lab 12, Drill 02, Drill 07, Drill 08 |
| Monitor system performance | Lab 09, Drill 06 |
| Ensure smooth system functionality | Labs 08-13, Drill 08 |
| Create, maintain, and utilise documentation | All labs, learner workflow, final write-ups |
| Compliance with processes and policies | Labs 08, 13, 14, Drill 07 |
| ITIL best-practice mindset | Incident, problem, change, root cause, evidence, and documentation sections in every lab |
| Root cause thinking | Break/fix scenarios, troubleshooting notes, reflection questions |
| Knowledge sharing | Final documentation, runbooks, evidence summaries |
| Risk and problem identification | Security, monitoring, maintenance, and drill phases |

### Technical Skills Mapping

| DXC desirable skill | LinuxLabs coverage |
| --- | --- |
| Red Hat and Debian Linux | RHEL vs Ubuntu comparison across labs |
| Solaris and AIX awareness | POSIX shell and KornShell awareness; UNIX portability notes |
| Bash scripting | Bash progression across all labs; full scripting in Lab 10; drills reinforce it |
| KornShell | Awareness and comparison in shell progression notes |
| Ansible, Terraform, Puppet, Chef | Ansible awareness in automation extension notes; Terraform/Puppet/Chef treated as optional stretch after core Linux |
| Process and job control | Lab 10, cron, at, systemd timers, process monitoring |
| TCP/IP, DNS, DHCP, NFS, SSH, FTP | Lab 05, Lab 11, Drill 02, Drill 04 |
| Filesystem management | Lab 07, Drill 03 |
| LVM, ext4, XFS, ZFS | Lab 07; ZFS awareness as stretch/UNIX storage comparison |
| Performance tuning and monitoring | Lab 09, Drill 06 |
| top, vmstat, iostat, sar, netstat | Lab 09, Drill 06 |
| Automation software exposure | Lab 10 and drill automation tasks |
| Bash, Python, Git | Bash throughout, Python optional automation stretch, Git via documentation workflow |
| AWS exposure | Cloud operations notes and optional stretch in later drills |
| KVM, VMware, Docker, Podman | Modern Linux and optional virtualisation/container stretch tasks |

### Bash Readiness Target

By the end of LinuxLabs, the learner should be able to use Bash to:

* inspect system state
* collect incident evidence
* parse logs
* report users and groups
* validate permissions
* check services
* check network reachability
* report package and patch status
* monitor CPU, memory, disk, and I/O
* automate health checks
* schedule jobs
* generate repeatable evidence for documentation

### Support Readiness Target

By the end of the 23 labs, the learner should be able to handle support scenarios such as:

* a user cannot SSH into a server
* a service is down after reboot
* DNS works from one host but not another
* disk usage is high and the application is failing
* a package update changed service behaviour
* a user has incorrect access to a shared directory
* a Samba share is visible but access is denied
* a cron job did not run
* performance is degraded and evidence is needed
* suspicious login activity appears in logs
* security hardening blocks a service and needs safe remediation

### Operational Behaviour Target

The learner should show evidence of:

* organised work
* time-aware troubleshooting
* documenting decisions
* using change-style notes before risky changes
* finding likely root causes
* improving repeatable processes
* sharing knowledge through runbooks
* identifying risks before they become incidents
* validating every fix with command output

### Gap Handling

Some job technologies are broader than the core Practical Linux book.

They should be handled as follows:

| Skill | Treatment |
| --- | --- |
| Solaris and AIX | Awareness through POSIX/KornShell notes; optional later UNIX lab if needed |
| ZFS | Awareness in storage lab; optional stretch task |
| Ansible | Introduce after Bash foundations; optional stretch inside Lab 10 or Drill 08 |
| Terraform | Mention as IaC awareness; not core to Linux administration labs |
| Puppet/Chef | Awareness only unless a later dedicated config management lab is added |
| AWS | Optional stretch for Linux on cloud instances after local Linux fundamentals |
| Docker/Podman | Optional stretch in modern Linux notes after process, networking, storage, and security foundations |

### Final Readiness Standard

The learner is ready for this type of Linux System Administrator role when they can complete the 8 drills with minimal prompting, capture useful evidence, explain their decisions, and document the outcome clearly enough for another engineer to follow.
