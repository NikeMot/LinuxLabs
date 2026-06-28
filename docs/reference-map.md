# Reference Map

### Purpose

This file maps the LinuxLabs programme to the reference books, operational thinking sources, online documentation sources, and AI-assisted operations standards.

The canonical structure follows the 15 chapters of *Practical Linux System Administration*.

### Reference Roles

| Source | Used for |
| --- | --- |
| Practical Linux System Administration | Primary 15-chapter lab spine |
| The Practice of System and Network Administration | Operational execution standard: documentation, repeatability, service ownership, incident thinking, change discipline |
| The Practice of Cloud System Administration | Reliability, automation, scalable operations, cloud-style administration, production readiness |
| The Linux Command Line | Shell fluency, filesystem navigation, text processing, scripting fundamentals |
| Learning Modern Linux | Modern Linux concepts, cloud-native context, containers, observability, modern tooling |
| Modern Operating Systems / Operating System Concepts | Processes, memory, filesystems, I/O, security, concurrency, and OS theory |
| Red Hat documentation | Current RHEL-specific implementation and administration guidance |
| Ubuntu documentation | Current Ubuntu-specific implementation and administration guidance |
| Debian documentation | Debian-family administration guidance and package behaviour |
| Project documentation | Current systemd, Ansible, Samba, OpenSSH, Linux kernel, and related project behaviour |
| Local man pages and package documentation | Installed-system truth for command options, config files, service behaviour, and package versions |
| AI-assisted operations notes | Prompting, command review, log summaries, runbook drafts, comparison notes, and safety checks |

### Full-Chapter Reference Rule

When a LinuxLabs lab references a book chapter, the whole chapter should be treated as the reference unit.

Do not cherry-pick isolated paragraphs or tiny fragments as the basis of a lab.

Use the full chapter to understand:

* the main topic
* supporting concepts
* related commands
* warnings and limitations
* operational context
* chapter summary or conclusions

The final lab must still be original work. Do not copy book text into the repository.

### Online Documentation Rule

Books provide structure and depth. Online documentation provides current implementation detail.

Every lab must check current online documentation where commands, package names, service names, configuration paths, security controls, release behaviour, or tool syntax may have changed.

Prefer official vendor or project documentation, then local man pages and package documentation from the lab system.

### Two-Part Lab Rule

Every chapter lab has two parts:

```text
Part 1 - New Chapter Content
Part 2 - Cumulative Repetition of All Previous Topics
```

Part 1 uses the current full chapter.

Part 2 repeats and combines all topics learned in earlier labs.

### Coverage Rule

By the end of Lab 15, the series must cover the practical administration content from *Practical Linux System Administration* and the relevant supporting concepts from the other Linux and operating systems references.

### Chapter-to-Lab Rule

| Chapter | Lab |
| --- | --- |
| 1. Getting Started with Linux | Lab 01 |
| 2. Working with Permissions and Privileged Accounts | Lab 02 |
| 3. Customizing the User Experience | Lab 03 |
| 4. Managing Users | Lab 04 |
| 5. Connecting to a Network | Lab 05 |
| 6. Installing and Uninstalling Software | Lab 06 |
| 7. Managing Storage | Lab 07 |
| 8. Maintaining System Health | Lab 08 |
| 9. Monitoring Your System | Lab 09 |
| 10. Scripting and Automation | Lab 10 |
| 11. Deploying Samba for Windows Compatibility | Lab 11 |
| 12. Troubleshooting Linux | Lab 12 |
| 13. Securing Your System | Lab 13 |
| 14. Continuing Your Education | Lab 14 |
| 15. Making Career Moves | Lab 15 |

### Supporting Standards

| Standard | Purpose |
| --- | --- |
| `docs/cumulative-repetition-standard.md` | Defines the two-part lab structure and cumulative review rule |
| `docs/break-fix-standard.md` | Defines mandatory controlled failure, diagnosis, repair, verification, and prevention practice |
| `docs/online-documentation-standard.md` | Defines how current official online documentation is checked and recorded |
| `docs/environment-standard.md` | Defines hosts, snapshots, baseline tools, and evidence rules |
| `docs/debian-rhel-comparison-matrix.md` | Tracks recurring Ubuntu vs RHEL-family differences |
| `docs/bash-and-shell-progression.md` | Defines Bash and shell progression across all labs |
| `docs/itil-operations-templates.md` | Provides incident, problem, change, rollback, RCA, and restoration templates |
| `docs/assessment-gates.md` | Defines pass/fail readiness gates |
| `docs/network-filesharing-protocols.md` | Makes NFS, SSH/SFTP, FTP awareness, and Samba coverage explicit |
| `docs/ansible-mini-layer.md` | Adds a lightweight Ansible layer after Bash foundations |
| `scripts/README.md` | Defines the Bash script portfolio structure |

### Distribution Rule

Labs should compare **Debian/Ubuntu** and **RHEL-family** systems.

A lab is incomplete if only one family is attempted, unless the lab explicitly marks the other family out of scope and explains why.

### AI Usage Rule

AI can be used to support explanation, planning, documentation, comparison, and troubleshooting.

AI output should not be treated as evidence. Every important result must be verified using local system evidence, official documentation, logs, or command output.

### Reference Usage Rule

Do not copy book material or large sections of online documentation into the repository.

Use full chapters to understand book-based tasks. Use online documentation to confirm current implementation details. Then write original notes, evidence, and reflections.
