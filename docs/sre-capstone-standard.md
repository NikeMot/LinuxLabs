# SRE Capstone Standard

### Purpose

The final LinuxLabs capstone must be SRE-relevant.

It should prove that the learner can operate Linux systems as part of a reliability-focused production service, not merely complete isolated administration tasks.

### Capstone Position

The SRE capstone is:

```text
Drill 08 - Full Linux Operations SRE Capstone
```

It comes after:

* 15 chapter-led Linux administration labs
* 7 integration drills

### Core Scenario

The learner operates a small Linux-backed service across Debian-family and RHEL-family systems.

The service should include:

* at least one application or web service
* Linux host administration
* users and permissions
* package and service management
* networking and firewall exposure
* storage or logs with capacity risk
* monitoring evidence
* incident response
* recovery and verification
* documentation good enough for another engineer

### SRE Focus Areas

The capstone should include:

| Area | Requirement |
| --- | --- |
| Service ownership | Define what service is being supported and what good looks like |
| SLIs | Define measurable indicators such as availability, latency, error rate, or saturation |
| SLOs | Set simple reliability targets for the lab service |
| Monitoring | Collect CPU, memory, disk, process, service, port, and log evidence |
| Alerting | Define what should alert and why |
| Incident response | Diagnose and restore service after a simulated failure |
| Error budget thinking | Explain whether the failure would burn reliability budget |
| Postmortem | Write a blameless incident review |
| Runbook | Produce recovery steps another engineer can follow |
| Toil reduction | Identify at least one manual task to automate |
| Automation | Use Bash and optionally Ansible to reduce repeat manual work |
| Capacity planning | Identify disk, CPU, memory, or service limits |
| Change safety | Use rollback thinking before risky changes |
| Production readiness | Explain risks, gaps, and next improvements |

### Required SRE Artefacts

The final capstone write-up must include:

* service overview
* architecture or service diagram
* SLI definitions
* SLO target
* monitoring checks
* alert candidates
* incident timeline
* root cause analysis
* recovery evidence
* post-reboot verification
* rollback notes
* blameless postmortem
* runbook
* toil-reduction note
* Bash automation evidence
* Debian/Ubuntu evidence
* RHEL-family evidence
* RHEL vs Ubuntu comparison

### Example Failure Modes

Suitable capstone failures include:

* service down after reboot
* incorrect firewall rule
* broken package update
* disk pressure affecting logs or service operation
* permission problem blocking service access
* DNS or host resolution issue
* monitoring gap that delays detection
* configuration drift between Ubuntu and RHEL-family systems
* expired or disabled user access needed for support

### SRE-Style Questions

The capstone should force the learner to answer:

1. What service is being supported?
2. What does reliable mean for this service?
3. What indicators prove the service is healthy?
4. What broke?
5. How was it detected?
6. How was it restored?
7. What evidence proves recovery?
8. What would have alerted earlier?
9. What manual work should be automated?
10. What would reduce recurrence?

### Bash Requirement

The capstone must include Bash evidence.

At minimum, Bash should be used for one of:

* service health check
* log summary
* disk or capacity report
* network check
* user or permission audit
* recovery verification
* incident evidence collection

### Optional Ansible Requirement

Ansible may be used after the Bash/manual approach is understood.

Suitable Ansible use:

* install required package
* ensure service is enabled and running
* deploy a simple config
* create a directory with correct ownership
* collect facts from both systems

Ansible must not hide lack of Linux understanding. The learner must still verify the result with normal Linux commands.

### Completion Standard

The capstone is complete only when the learner can:

* restore the service on both Debian-family and RHEL-family systems
* explain the incident clearly
* provide monitoring and recovery evidence
* produce a useful runbook
* write a short blameless postmortem
* identify a toil-reduction improvement
* explain how the service could be made more reliable
