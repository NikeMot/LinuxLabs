# Break/Fix Standard

### Purpose

Break/fix is the most important practical skill in LinuxLabs.

Every lab and drill should include a controlled failure, evidence-led diagnosis, safe repair, and verification.

The goal is to build operational confidence: when something fails, the learner can stay calm, gather evidence, form a hypothesis, fix safely, and prove recovery.

### Core Rule

```text
Every lab must include controlled break/fix practice.
```

A lab is not complete until the learner has:

* captured the working state before the failure
* introduced or encountered a controlled failure
* diagnosed the failure using evidence
* explained the likely cause
* repaired the issue
* verified the repair
* confirmed the fix survives reboot where relevant
* documented what happened

### Safety Rules

Break/fix must be done only in disposable lab systems.

Do not perform break/fix practice on:

* employer systems
* production systems
* shared systems
* systems containing personal or sensitive data
* internet-facing systems unless the lab explicitly requires safe exposure

Before breaking anything:

* take a snapshot or checkpoint
* record the baseline state
* know how to roll back
* avoid irreversible destructive changes unless the lab is specifically about restore practice

### Break/Fix Method

Use this sequence:

1. Baseline
2. Break
3. Observe symptoms
4. Gather evidence
5. Form hypothesis
6. Fix
7. Verify
8. Reboot test where relevant
9. Document
10. Improve or automate

### Evidence Required

Each break/fix exercise should capture:

| Stage | Evidence |
| --- | --- |
| Baseline | service status, config check, connectivity check, filesystem state, or user/access state |
| Break | what was changed or what failure appeared |
| Symptoms | what stopped working and how it was detected |
| Diagnosis | commands, logs, status output, config inspection, comparison with baseline |
| Fix | exact change made to restore service |
| Verification | proof that the service, user access, storage, network, or security control works again |
| Persistence | post-reboot proof where relevant |
| Prevention | monitoring, documentation, automation, or safer change process |

### Suitable Failure Types

Use failures that are realistic for Linux administration:

| Area | Example failure |
| --- | --- |
| Service management | service disabled, stopped, failed unit, wrong config path |
| SSH/access | wrong permission, bad config, firewall blocking access |
| Users/groups | missing group membership, locked account, wrong shell |
| Permissions | wrong owner, mode, ACL, or sudo rule |
| Networking | bad DNS, wrong route, closed port, hostname resolution issue |
| Packages | missing package, wrong package name, broken dependency, failed update |
| Storage | full filesystem, failed mount, bad fstab entry, missing directory |
| Logs/monitoring | missing log evidence, unclear alert, service failure not detected |
| Security controls | AppArmor or SELinux behaviour affecting service access |
| Automation | Bash script fails due to quoting, path, permission, or missing command |
| File sharing | Samba or NFS access blocked by permissions, service, or firewall |

### Distribution Requirement

Where practical, the same class of failure should be practised on both:

* Debian/Ubuntu
* RHEL-family

The learner must document how the diagnosis and fix differed.

Examples:

* `ssh` service name on Ubuntu vs `sshd` on RHEL-family
* AppArmor vs SELinux
* `ufw` or nftables vs firewalld
* `apt` vs `dnf`
* `/var/log/syslog` vs `/var/log/messages`

### SRE Capstone Requirement

The final capstone must include at least one reliability incident.

It should include:

* service impact
* detection method
* incident timeline
* root cause analysis
* recovery evidence
* postmortem
* runbook update
* toil-reduction improvement
* alerting or monitoring improvement

### Documentation Rule

The final write-up must clearly separate:

```text
What was broken
How it was detected
How it was diagnosed
How it was fixed
How recovery was proven
What would prevent recurrence
```

### Reflection Link

The seven reflection questions must always capture what broke, what confused the learner, what evidence proved recovery, and what would be improved next time.
