# Linux Lab Output Template

Use this template for every LinuxLabs lab. Keep it evidence-based, operational, and production-focused.

The learner should focus on solving the lab. Documentation, formatting, evidence organisation, and GitHub upload are handled after the learner provides command output, observations, issues encountered, and answers to the seven reflection questions.

Every applicable lab must be attempted on both a Debian-family system, normally Ubuntu Server LTS, and a RHEL-family system. A lab is not complete until both implementations have evidence, unless one family is explicitly marked out of scope with a reason.

Every chapter lab has two parts:

1. **Part 1 — New Chapter Content**
2. **Part 2 — Cumulative Repetition of All Previous Topics**

When a book chapter is used as a reference, use the full chapter as the reference unit, not isolated extracts.

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

| Area | Suggested reference | Chapter usage |
| --- | --- | --- |
| Linux command-line usage | The Linux Command Line | Use full relevant chapter |
| Modern Linux concepts | Learning Modern Linux | Use full relevant chapter |
| Linux administration tasks | Practical Linux System Administration | Use full current chapter |
| Operating system concepts | Modern Operating Systems / Operating System Concepts | Use full relevant chapter |
| Operational thinking | The Practice of System and Network Administration | Use full relevant chapter or section-level operational principle only where no chapter mapping exists |
| Cloud operations thinking | The Practice of Cloud System Administration | Use full relevant chapter where used |
| RHEL-specific guidance | Red Hat documentation | Use official task guidance |
| Ubuntu-specific guidance | Ubuntu documentation | Use official task guidance |
| AI-assisted operations | Lab notes, official product documentation, and verified system evidence | AI is not evidence |

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
* Do not use isolated book extracts as the lab reference when a full chapter is available.

---

## 6. Assumptions

Record assumptions here.

Examples:

* The lab is performed on both Debian/Ubuntu and RHEL-family systems unless stated otherwise.
* The systems are disposable lab machines.
* The work must survive a reboot.
* Documentation should be good enough for another engineer to follow.
* Part 2 repeats all topics previously learned in the series.

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
| Part 1 evidence | Proves the new chapter content was completed |
| Part 2 evidence | Proves previous topics were repeated and combined |
| Debian/Ubuntu evidence | Proves the work succeeded on Ubuntu or another Debian-family system |
| RHEL-family evidence | Proves the work succeeded on RHEL, Rocky, AlmaLinux, or CentOS Stream |
| RHEL vs Ubuntu notes | Captures distribution differences |
| Break/fix notes | Records troubleshooting and recovery |
| AI-assisted operations notes | Records where AI helped and what was verified independently |
| Runbook notes | Captures repeatable operational procedure |

---

## 9. Part 1 — New Chapter Content

Part 1 focuses on the current full chapter.

### New Content Tasks

| Task | Debian/Ubuntu requirement | RHEL-family requirement | Evidence required |
| --- | --- | --- | --- |
| Task 1 | | | |
| Task 2 | | | |
| Task 3 | | | |

### Part 1 Evidence

| Check | Debian/Ubuntu evidence | RHEL-family evidence | Result |
| --- | --- | --- | --- |
| | | | Passed / Failed |
| | | | Passed / Failed |

---

## 10. Part 2 — Cumulative Repetition of All Previous Topics

Part 2 repeats all topics learned before this lab.

For Lab 01, repeat the baseline checks until fluent.

For Lab 02 onward, include practical repetition from every earlier lab.

### Previous Topics to Repeat

| Previous lab/topic | Debian/Ubuntu task | RHEL-family task | Evidence required |
| --- | --- | --- | --- |
| Lab 01 baseline/CLI | | | |
| Lab 02 permissions/sudo | | | |
| Lab 03 shell environment | | | |
| Lab 04 users/groups | | | |
| Lab 05 networking/SSH | | | |
| Lab 06 software/packages | | | |
| Lab 07 storage/filesystems | | | |
| Lab 08 system health | | | |
| Lab 09 monitoring/performance | | | |
| Lab 10 scripting/automation | | | |
| Lab 11 Samba/file sharing | | | |
| Lab 12 troubleshooting | | | |
| Lab 13 security | | | |
| Lab 14 learning system | | | |

Remove rows that are not yet applicable.

### Part 2 Evidence

| Check | Debian/Ubuntu evidence | RHEL-family evidence | Result |
| --- | --- | --- | --- |
| | | | Passed / Failed |
| | | | Passed / Failed |

---

## 11. Key Commands Used

Record important commands only.

| Command | Part | Debian/Ubuntu purpose | RHEL-family purpose |
| --- | --- | --- | --- |
| | Part 1 / Part 2 | | |
| | Part 1 / Part 2 | | |

---

## 12. Files Created or Changed

| Path | Part | Debian/Ubuntu | RHEL-family | Purpose |
| --- | --- | --- | --- | --- |
| | Part 1 / Part 2 | | | |
| | Part 1 / Part 2 | | | |

---

## 13. Debian/Ubuntu Implementation Evidence

This section proves the lab worked on Ubuntu or another Debian-family system.

| Check | Part | Evidence | Result |
| --- | --- | --- | --- |
| | Part 1 / Part 2 | | Passed / Failed |
| | Part 1 / Part 2 | | Passed / Failed |

---

## 14. RHEL-Family Implementation Evidence

This section proves the lab worked on RHEL, Rocky Linux, AlmaLinux, or CentOS Stream.

| Check | Part | Evidence | Result |
| --- | --- | --- | --- |
| | Part 1 / Part 2 | | Passed / Failed |
| | Part 1 / Part 2 | | Passed / Failed |

---

## 15. RHEL vs Ubuntu Comparison

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

## 16. Break/Fix Scenario

Describe what was deliberately broken or what failure was simulated.

| Failure | Part | Family affected | Cause | Diagnosis | Fix | Evidence |
| --- | --- | --- | --- | --- | --- | --- |
| | Part 1 / Part 2 | | | | | |

---

## 17. Post-Reboot Verification

Nothing counts unless it survives reboot.

| Check | Part | Debian/Ubuntu evidence | RHEL-family evidence | Result |
| --- | --- | --- | --- | --- |
| Service/state persisted after reboot | Part 1 / Part 2 | | | Passed / Failed |
| Network/storage/security configuration persisted after reboot | Part 1 / Part 2 | | | Passed / Failed |
| Documentation updated after final verification | Part 1 / Part 2 | | | Passed / Failed |

---

## 18. AI-Assisted Operations Notes

Use this section when AI was used during the lab.

| AI use | Part | What it helped with | What was independently verified | Evidence |
| --- | --- | --- | --- | --- |
| | Part 1 / Part 2 | | | |

If AI was not used, write:

> AI was not used for this lab.

---

## 19. Diagram

Add a diagram if useful.

If no diagram is required, write:

> No diagram required for this lab.

---

## 20. Issues Encountered

| Issue | Part | Family affected | Cause | Fix |
| --- | --- | --- | --- | --- |
| | Part 1 / Part 2 | | | |

If there were no issues, write:

> No major issues encountered.

---

## 21. Decisions Made

| Decision | Part | Reason |
| --- | --- | --- |
| | Part 1 / Part 2 | |
| | Part 1 / Part 2 | |

---

## 22. Security and Production Considerations

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
* cumulative repetition and skill retention

---

## 23. Final Outcome

State clearly whether Part 1 and Part 2 were completed on both Debian/Ubuntu and RHEL-family systems.

---

## 24. What I Learned

Summarise the learner's reflection answers into 3–6 bullet points.

---

## 25. What I Would Improve in Production

Summarise production improvements from the learner's reflection answers.

---

## 26. References Used

| Reference | Chapter used | Used for |
| --- | --- | --- |
| | Full chapter / official guidance | |
| | Full chapter / official guidance | |

---

## 27. Completion Checklist

* [ ] Requirements understood
* [ ] Part 1 new chapter content completed
* [ ] Part 2 cumulative repetition completed
* [ ] Full chapter used where a book chapter was referenced
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

## 28. Reflection Questions

Ask exactly seven reflection questions at the end of the lab.

1. What problem did this lab simulate?
2. What new chapter content did you practise, and what previous topics did Part 2 force you to repeat?
3. What commands, files, or services mattered most in solving it on Debian/Ubuntu and RHEL-family systems?
4. What evidence proves your solution worked on both families?
5. What broke, confused you, or required troubleshooting?
6. Where did AI help, if at all, and what did you verify yourself?
7. What would you improve, automate, or monitor next time?
