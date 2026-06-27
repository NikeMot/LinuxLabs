# LinuxLabs Assessment Gates

### Purpose

Assessment gates define when the learner is ready to move forward.

Completing a lab means little unless the learner can repeat, explain, troubleshoot, and verify the work with limited prompting.

### Gate 1 — Core Access and Baseline

**Timing:** after Lab 05.

**Coverage:** Labs 01-05.

The learner should be able to:

* identify OS version, kernel, hostname, IP address, storage, memory, and running services
* navigate the filesystem confidently
* use man pages and local help
* create and verify users and groups
* configure sudo safely
* inspect and modify permissions
* explain shell startup files and environment variables
* configure or troubleshoot SSH
* perform basic network checks
* compare Ubuntu and RHEL-family differences

**Pass standard:** rebuild access and baseline evidence on both Ubuntu and RHEL-family systems with minimal prompting.

### Gate 2 — System Administration Core

**Timing:** after Lab 10.

**Coverage:** Labs 01-10.

The learner should be able to:

* manage packages with `apt` and `dnf`
* identify package owners and dependencies
* add and verify storage
* mount filesystems persistently
* work with swap and LVM
* apply health maintenance tasks
* inspect system performance
* use `top`, `vmstat`, `iostat`, `sar`, and process tools
* write safe Bash scripts
* schedule jobs with cron or systemd timers
* collect repeatable evidence

**Pass standard:** complete a maintenance and monitoring scenario on both families with Bash-generated evidence.

### Gate 3 — Services, Troubleshooting, and Security

**Timing:** after Lab 13.

**Coverage:** Labs 01-13.

The learner should be able to:

* deploy and verify a network service
* troubleshoot service failures using logs and systemd
* repair firewall and access issues
* diagnose permissions and account problems
* configure and troubleshoot Samba
* explain AppArmor vs SELinux behaviour
* harden SSH and privileged access
* create incident, problem, change, and rollback notes
* prove post-reboot persistence

**Pass standard:** recover a broken service on both families and produce evidence good enough for another engineer to follow.

### Gate 4 — Learning, Portfolio, and Role Readiness

**Timing:** after Lab 15.

**Coverage:** Labs 01-15.

The learner should be able to:

* explain the full lab series as professional evidence
* describe operational decisions clearly
* identify remaining gaps
* maintain a learning log
* organise scripts and runbooks
* communicate Linux troubleshooting stories using evidence
* map lab outcomes to Linux administrator job requirements

**Pass standard:** produce a role-readiness summary backed by lab evidence, not generic claims.

### Gate 5 — Drill Readiness

**Timing:** after Drill 04.

**Coverage:** Drills 01-04.

The learner should be able to combine:

* baseline rebuild
* user and sudo recovery
* network troubleshooting
* service recovery
* storage repair
* restore evidence
* permissions and Samba troubleshooting

**Pass standard:** complete mixed incidents without a command-by-command walkthrough.

### Gate 6 — Final SRE-Style Linux Operations Readiness

**Timing:** after Drill 08.

**Coverage:** all 23 labs.

The learner should be able to:

* provide first and second level Linux support
* monitor system performance
* use Bash for evidence and automation
* troubleshoot incidents and problems
* document actions clearly
* work to ITIL-style process discipline
* handle both Ubuntu and RHEL-family systems
* define simple SLIs and SLOs for a Linux-backed service
* collect service health and saturation evidence
* identify alert candidates
* restore service after a simulated reliability incident
* produce a blameless postmortem
* write a recovery runbook
* identify toil and propose automation
* explain reliability risks and next improvements

**Pass standard:** complete the final SRE-style capstone with minimal prompting, restore the service on both distribution families, capture useful reliability evidence, explain decisions, produce a runbook and postmortem, and document the outcome clearly enough for another engineer to continue support.

### Scoring Model

Use this simple score at each gate:

| Score | Meaning |
| --- | --- |
| 0 | Not attempted |
| 1 | Attempted but not working |
| 2 | Works with heavy prompting |
| 3 | Works with light prompting |
| 4 | Works independently with evidence |
| 5 | Works independently, explains clearly, and documents production considerations |

Target score before moving forward:

```text
4 or higher
```

A score below 4 means the learner should repeat or drill the weak area before continuing.
