# Linux Lab Output Template

Use this template for every LinuxLabs lab. Keep it evidence-based, operational, and production-focused.

The learner should focus on solving the lab. Documentation, formatting, evidence organisation, and GitHub upload are handled after the learner provides command output, observations, issues encountered, and answers to the seven reflection questions.

Every applicable lab must be attempted on both a Debian-family system, normally Ubuntu Server LTS, and a RHEL-family system. A lab is not complete until both implementations have evidence, unless one family is explicitly marked out of scope with a reason.

---

# Lab Title

## 1. Lab Summary

**Lab:**

**Date completed:**

**Topic area:**

**Difficulty:**

**Status:** Not started / In progress / Completed / Blocked

**Debian/Ubuntu status:** Not started / In progress / Completed / Out of scope

**RHEL-family status:** Not started / In progress / Completed / Out of scope

### Objective

State the purpose of the lab in 2–4 lines.

---

## 2. Scenario

Describe the real-world Linux administration situation this lab simulates.

The scenario should read like a ticket or operational request, not just a tutorial.

---

## 3. Reference Material

| Area | Suggested reference |
| --- | --- |
| Linux command-line usage | The Linux Command Line |
| Modern Linux concepts | Learning Modern Linux |
| Linux administration tasks | Practical Linux System Administration |
| Operating system concepts | Modern Operating Systems |
| Operational thinking | The Practice of System and Network Administration |
| Cloud operations thinking | The Practice of Cloud System Administration |
| RHEL-specific guidance | Red Hat documentation |
| Ubuntu-specific guidance | Ubuntu documentation |
| AI-assisted operations | Lab notes, official product documentation, and verified system evidence |

---

## 4. Requirements

| ID | Requirement | Debian/Ubuntu status | RHEL-family status |
| --- | --- | --- | --- |
| R1 | | Not started | Not started |
| R2 | | Not started | Not started |
| R3 | | Not started | Not started |

---

## 5. Constraints

Record anything the learner must not do.

Examples:

* Do not disable security controls permanently just to make the lab work.
* Do not commit secrets, SSH private keys, credentials, PDFs, EPUBs, or company data.
* Do not rely on commands that cannot be explained.
* Do not mark the lab complete without post-reboot verification.
* Do not treat AI output as proof without local verification.
* Do not mark a lab complete if only one distribution family has been attempted, unless the other is explicitly out of scope with a reason.

---

## 6. Assumptions

Record assumptions here.

Examples:

* The lab is performed on both Debian/Ubuntu and RHEL-family systems unless stated otherwise.
* The systems are disposable lab machines.
* The work must survive a reboot.
* Documentation should be good enough for another engineer to follow.

---

## 7. Expected Lab Structure

Use a structure appropriate for the lab.

Example:

```text
01-getting-started-with-linux/
└── lab-01-bootstrap-and-baseline-linux-server.md
```

---

## 8. Deliverables

| Deliverable | Purpose |
| --- | --- |
| Lab write-up | Records requirements, implementation, evidence, and reflection |
| Debian/Ubuntu evidence | Proves the work succeeded on Ubuntu or another Debian-family system |
| RHEL-family evidence | Proves the work succeeded on RHEL, Rocky, AlmaLinux, or CentOS Stream |
| RHEL vs Ubuntu notes | Captures distribution differences |
| Break/fix notes | Records troubleshooting and recovery |
| AI-assisted operations notes | Records where AI helped and what was verified independently |
| Runbook notes | Captures repeatable operational procedure |

---

## 9. Implementation Tasks

Use these tasks as a guide, not as a full walkthrough.

The learner solves the lab. The final documentation is produced after the learner provides evidence and reflection answers.

### Task 1 — Task name

Describe what must be done and what must be proven on both Debian/Ubuntu and RHEL-family systems.

### Task 2 — Task name

Describe what must be done and what must be proven on both Debian/Ubuntu and RHEL-family systems.

### Task 3 — Task name

Describe what must be done and what must be proven on both Debian/Ubuntu and RHEL-family systems.

---

## 10. Key Commands Used

Record important commands only.

| Command | Debian/Ubuntu purpose | RHEL-family purpose |
| --- | --- | --- |
| | | |
| | | |

---

## 11. Files Created or Changed

| Path | Debian/Ubuntu | RHEL-family | Purpose |
| --- | --- | --- | --- |
| | | | |
| | | | |

---

## 12. Debian/Ubuntu Implementation Evidence

This section proves the lab worked on Ubuntu or another Debian-family system.

| Check | Evidence | Result |
| --- | --- | --- |
| | | Passed / Failed |
| | | Passed / Failed |

---

## 13. RHEL-Family Implementation Evidence

This section proves the lab worked on RHEL, Rocky Linux, AlmaLinux, or CentOS Stream.

| Check | Evidence | Result |
| --- | --- | --- |
| | | Passed / Failed |
| | | Passed / Failed |

---

## 14. RHEL vs Ubuntu Comparison

| Area | RHEL-family | Debian/Ubuntu | Notes |
| --- | --- | --- | --- |
| Package management | | | |
| Service management | | | |
| Networking | | | |
| Security controls | | | |
| Logs | | | |
| Config paths | | | |
| Filesystems/storage | | | |
| Shell/user environment | | | |

---

## 15. Break/Fix Scenario

Describe what was deliberately broken or what failure was simulated.

| Failure | Family affected | Cause | Diagnosis | Fix | Evidence |
| --- | --- | --- | --- | --- | --- |
| | | | | | |

---

## 16. Post-Reboot Verification

Nothing counts unless it survives reboot.

| Check | Debian/Ubuntu evidence | RHEL-family evidence | Result |
| --- | --- | --- | --- |
| Service/state persisted after reboot | | | Passed / Failed |
| Network/storage/security configuration persisted after reboot | | | Passed / Failed |
| Documentation updated after final verification | | | Passed / Failed |

---

## 17. AI-Assisted Operations Notes

Use this section when AI was used during the lab.

| AI use | What it helped with | What was independently verified | Evidence |
| --- | --- | --- | --- |
| | | | |

If AI was not used, write:

> AI was not used for this lab.

---

## 18. Diagram

Add a diagram if useful.

If no diagram is required, write:

> No diagram required for this lab.

---

## 19. Issues Encountered

| Issue | Family affected | Cause | Fix |
| --- | --- | --- | --- |
| | | | |

If there were no issues, write:

> No major issues encountered.

---

## 20. Decisions Made

| Decision | Reason |
| --- | --- |
| | |
| | |

---

## 21. Security and Production Considerations

Explain the production relevance of the lab.

Cover where relevant:

* access control
* auditability
* rollback and recovery
* repeatability
* least privilege
* reliability
* monitoring
* operational risk
* documentation quality
* distro differences
* responsible AI usage

---

## 22. Final Outcome

State clearly whether the lab was completed on both Debian/Ubuntu and RHEL-family systems.

---

## 23. What I Learned

Summarise the learner's reflection answers into 3–6 bullet points.

---

## 24. What I Would Improve in Production

Summarise production improvements from the learner's reflection answers.

---

## 25. References Used

| Reference | Used for |
| --- | --- |
| | |
| | |

---

## 26. Completion Checklist

* [ ] Requirements understood
* [ ] Debian/Ubuntu implementation completed or explicitly marked out of scope with a reason
* [ ] RHEL-family implementation completed or explicitly marked out of scope with a reason
* [ ] Debian/Ubuntu verification evidence captured
* [ ] RHEL-family verification evidence captured
* [ ] RHEL vs Ubuntu comparison completed
* [ ] Break/fix scenario completed
* [ ] Post-reboot verification completed for both applicable families
* [ ] AI-assisted operations notes completed or marked not used
* [ ] Issues documented
* [ ] Decisions documented
* [ ] Security and production considerations documented
* [ ] Diagram added if useful
* [ ] Seven reflection answers captured
* [ ] Work committed with a clear message
* [ ] Work uploaded to the correct topic folder
* [ ] No secrets or private data committed

---

## 27. Reflection Questions

Ask exactly seven reflection questions at the end of the lab.

1. What problem did this lab simulate?
2. What commands, files, or services mattered most in solving it on Debian/Ubuntu and RHEL-family systems?
3. What evidence proves your solution worked on both families?
4. What broke, confused you, or required troubleshooting?
5. What would be risky about doing this in production?
6. Where did AI help, if at all, and what did you verify yourself?
7. What would you improve, automate, or monitor next time?
