# Bash and Shell Progression

### Purpose

Bash and shell usage must be taught throughout LinuxLabs, not only in the scripting chapter.

The goal is to become confident enough to use Bash for investigation, administration, automation, reporting, and safe operational changes in a Linux system administrator role.

### Shells Covered

| Shell | Role in the programme |
| --- | --- |
| Bash | Primary shell for daily Linux administration and scripting |
| POSIX sh | Portability baseline and script compatibility awareness |
| KornShell | Awareness for enterprise UNIX environments such as AIX and Solaris estates |
| Z shell | Awareness only, mainly for interactive shell comparison |

### Progression Model

The learner should build shell skill in layers:

1. Interactive navigation and inspection
2. Safe command composition
3. Text processing and filtering
4. Variables, quoting, expansion, and exit codes
5. Loops and conditionals
6. Functions and script structure
7. Error handling and logging
8. Scheduled execution
9. Operational reporting
10. Cross-platform shell awareness
11. AI-assisted script review with independent verification

### Chapter Lab Integration

| Lab | Shell focus |
| --- | --- |
| 01 | CLI navigation, command history, help, man pages, redirection, pipes, aliases |
| 02 | Permission inspection, safe use of sudo, ownership checks, `find` with permission filters |
| 03 | Bash startup files, login vs non-login shells, environment variables, prompts, `/etc/skel` |
| 04 | User and group audit commands, loops for account reporting, safe parsing of `/etc/passwd` and `/etc/group` |
| 05 | Network inspection with Bash pipelines, SSH command execution, connectivity test scripts |
| 06 | Package inventory scripts, dependency checks, update logs, install verification commands |
| 07 | Disk and filesystem reporting, mount validation, fstab checks, LVM evidence collection |
| 08 | Cleanup scripts, retention checks, account review scripts, patch status reports |
| 09 | Monitoring loops, `sar` report parsing, CPU/memory/disk threshold checks |
| 10 | Full Bash scripting lab: structure, functions, arguments, exit codes, logs, scheduling |
| 11 | Samba share checks, permission validation scripts, client access verification notes |
| 12 | Troubleshooting scripts, log extraction, service checks, incident timeline generation |
| 13 | Security audit scripts, SSH config checks, firewall checks, account risk reports |
| 14 | Personal shell toolkit, reusable snippets, learning log automation, command journal |
| 15 | Portfolio script index, evidence packaging, role-readiness Bash examples |

### Drill Integration

| Drill | Shell focus |
| --- | --- |
| 01 | Rebuild baseline using shell-only inspection and setup notes |
| 02 | Network and service recovery using shell pipelines and log filters |
| 03 | Storage pressure investigation and restore evidence collection |
| 04 | User, permission, ACL, and Samba validation scripts |
| 05 | Package and rollback decision support scripts |
| 06 | Performance sampling and report generation |
| 07 | Security audit and incident response helper scripts |
| 08 | End-to-end operational Bash toolkit under capstone pressure |

### Required Bash Competencies

By the end of the 23-lab programme, the learner should be able to:

* navigate and inspect Linux systems quickly from the CLI
* combine commands with pipes and redirection
* use `grep`, `awk`, `sed`, `cut`, `sort`, `uniq`, `xargs`, and `find`
* understand quoting, globbing, variables, expansion, and command substitution
* read and use exit codes
* write scripts with clear structure and comments
* use functions, arguments, and conditionals
* handle errors safely
* log script output
* avoid unsafe destructive commands
* schedule jobs with cron and systemd timers
* write system health checks
* parse logs and produce evidence summaries
* review AI-generated commands before execution
* explain what a script does line by line

### Production Standard

Every script must be treated as an operational change.

Scripts should be:

* readable
* tested on disposable systems first
* idempotent where practical
* safe to rerun where practical
* logged
* reviewed before use
* documented
* verified with real command output

### AI Review Rule

AI may be used to review scripts, suggest improvements, or explain syntax.

AI-generated shell commands or scripts must not be trusted blindly. The learner must explain the command, test it safely, and verify the result independently.
