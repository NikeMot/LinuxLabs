# ITIL-Style Operations Templates

### Purpose

This document provides lightweight ITIL-style templates for LinuxLabs.

These are not intended to replace a real ITSM platform. They are used to practise operational thinking, evidence capture, incident handling, problem analysis, change control, rollback planning, and knowledge sharing.

### Incident Record Template

Use when something is broken or service is degraded.

```text
Incident ID:
Date/time opened:
Reported by:
Affected host(s):
Distribution family:
Service affected:
Impact:
Urgency:
Priority:
Symptoms:
Initial checks:
Actions taken:
Evidence captured:
Resolution:
Date/time resolved:
Post-fix verification:
Related problem record:
Knowledge article needed: Yes/No
```

### Problem Record Template

Use when looking for root cause or recurring issue patterns.

```text
Problem ID:
Related incident(s):
Affected service or area:
Known symptoms:
Suspected root cause:
Confirmed root cause:
Evidence:
Workaround:
Permanent fix:
Risk if not fixed:
Prevention action:
Owner:
Status:
```

### Change Note Template

Use before making a planned or risky change.

```text
Change ID:
Change title:
Reason for change:
Affected host(s):
Distribution family:
Risk level:
Pre-change state:
Implementation plan:
Validation plan:
Rollback plan:
Maintenance window:
Approval required: Yes/No
Result:
Post-change evidence:
Lessons learned:
```

### Known Error Template

Use when root cause is known but a permanent fix is not yet applied.

```text
Known Error ID:
Related problem:
Affected system/service:
Root cause:
Symptoms:
Workaround:
Permanent fix status:
Risk:
Detection method:
Documentation link:
```

### Rollback Plan Template

Use before changes that could break access, services, networking, storage, or security.

```text
Change being rolled back:
Rollback trigger:
Backup/snapshot available:
Files to restore:
Commands to reverse change:
Service restart required:
Reboot required:
Validation after rollback:
Owner:
```

### Root Cause Analysis Template

Use after a major incident or drill.

```text
Summary:
Timeline:
Impact:
Detection method:
Immediate cause:
Root cause:
Contributing factors:
What worked well:
What failed:
Corrective actions:
Preventive actions:
Monitoring improvements:
Documentation improvements:
Automation opportunities:
```

### Service Restoration Evidence Template

Use to prove a fix worked.

```text
Host:
Distribution family:
Service:
Command evidence:
Log evidence:
Connectivity evidence:
User/access evidence:
Post-reboot evidence:
Remaining risks:
```

### Lab Usage Rule

Every lab does not need every template.

Use the artefact that matches the scenario:

| Scenario | Template |
| --- | --- |
| Service is down | Incident Record |
| Issue keeps recurring | Problem Record |
| Planned config change | Change Note |
| Known workaround exists | Known Error |
| Risky change | Rollback Plan |
| Major break/fix drill | Root Cause Analysis |
| Fix completed | Service Restoration Evidence |

### Documentation Standard

Operational records should be concise, factual, and evidence-led.

Avoid vague statements such as:

```text
Fixed the issue.
```

Prefer evidence-based statements such as:

```text
Restarted sshd after correcting the configuration. Verified with systemctl status sshd, journalctl -u sshd, and successful SSH login from the admin workstation.
```
